---
title: Phrase Trail
permalink: /phrase-trail/
description: Tracks language that recurs across statutes, directives, procurement documents and reports.
---

Created Oct 26, 2026. Companion to the [System Registry](../registry/). Tracks language that recurs across statutes and directives, procurement documents and reports, so a reader can see where wording first appears and where it resurfaces. A shared phrase can have innocent explanations (shared industry vocabulary, a common template, text copied from an earlier public source); each entry notes the competing explanations.

**Tiers**
- **A · Authority:** statute, bill, executive order, memo, directive, OLC opinion, agency plan.
- **B · Procurement and notices:** J&A / LSJ / SSJ / JEFO, SOW or PWS, RFI, solicitation, SORN, PIA, Federal Register rule.
- **C · Reports and filings:** court filings and declarations, press releases, official statements, think-tank or advocacy papers.

**Marks:** D primary text read · R reporting · I inference · U unresolved · K general knowledge, verify.

**What an entry is.** One phrase family. Each row in the chain gives the exact quoted words, document, date, tier and mark. Chains are ordered by document date, not by who wrote what. Order of appearance is a lead, not proof that one document drove another.

**Strength of a match** (rate every entry)
- **S1 exact** · identical wording of 4+ words, or 2–3 distinctive words.
- **S2 near** · same distinctive words, different order or inflection.
- **S3 concept** · same idea, different words (e.g., "golden record" vs "one consolidated record"). Useful for mapping, weakest as provenance.

**Genericity** (rate every entry)
- **G1 boilerplate** · acquisition or legal template language ("logical follow-on," "sole source," "interest of economy and efficiency"). Excluded from the ledger unless it appears in a tier-A text.
- **G2 field-common** · common in data, IT or security writing ("seamless," "unified platform," "single source of truth"). Track, but do not read as signal alone.
- **G3 distinctive** · unusual in that field, or tied to a particular advocacy or legal theory ("undiluted," "diluting the votes of citizens"). Highest value.

**Competing explanations (check for every entry)**
- H1 shared industry vocabulary (MDM, NIEM, vendor marketing).
- H2 common template or the same drafter or counsel office.
- H3 vendor-supplied capability text copied into a government justification (this one matters most for tier B).
- H4 borrowed from an earlier public source (advocacy paper, prior EO, think-tank model).
- H5 deliberate carry-through so the paper trail "fits."
No entry below settles any of these. Vendors stay neutral infrastructure: an overlap in a procurement document is not evidence that a company knew of or took part in anything.

**Log rule.** When a new document arrives, search 2–3 of its distinctive phrases in quotes against this file, the research corpus. Add a row, or add a new entry. Record "no earlier hit found" when that is the result. Quote verbatim from the source text or do not quote.

---

## Seed ledger (built from texts already read in the project)

### PT-01 · "undiluted" / "diluting the votes of citizens" / "lawful voter"  [G3, S1–S2]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Jul 7, 2026 | A/C | DOJ (Dhillon) letter to all 50 states | any "intentional act that is aimed at diluting the votes of citizens" | D (secondary summary; verify against the letter) |
| Sept 22, 2026 | A | Hegseth memo, Countering Foreign Threats to 2026 Elections | "ensure that every lawful voter can cast their ballot … we must ensure that their voice remains sovereign, secure, and entirely undiluted" | D |
- **What it shows (I):** a foreign-threat directive using the vocabulary of the noncitizen-voting argument. That is the textual bridge from "foreign interference" to "foreign nationals voting."
- **Checked Oct 26 (D, Federal Register text of EO 14248, summarizer fetch):** §1 uses "dilution" three times ("without illegal dilution"; "guard against dilution by illegal voting, discrimination, fraud…"; "voters from having their ballots voided or diluted by fraudulent votes"). It does NOT contain "votes of citizens," "undiluted" or "lawful voter." So the dilution theme predates the DOJ wording, but the exact phrase does not come from EO 14248 (S3 only). Still to check: EO 14399, SAVE America Act, SAVE SORN, DOJ California complaint.
- **Next:** search "votes of citizens" + "dilut" in the SAVE America Act findings, EO 14248, EO 14399, the USCIS SAVE SORN preamble and Project 2025 election chapters to date the origin (flagged Oct 21, still open).
- Related liability wording from DOJ ("actual notice," "willful blindness") is a different phrase family; log it separately if it starts to recur in tier A or B texts.
- **H check:** H4 (earlier advocacy wording) is the leading alternative to H5.

### PT-02 · One person, one record: "one consolidated record" / "single, trusted source" / "single source of truth" / "person-centric"  [G2, S3]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| (PIA, date U in notes) | B | USCIS PCIS PIA | "a single, trusted source of biographical and biometric information" | D |
| Sept 4, 2025 (posted May 14, 2026) | B | DHS Palantir LSJ FY25-00257 | "deconfliction of data to ensure each subject has one consolidated record" | D |
| Nov 3, 2025 | B | USCIS biometrics proposed rule, FR 2025-19747 | "person-centric model" | D (baseline) |
| date U | C | Booz Allen "Public Safety Fusion Platform" (vendor wording, via Oct 26 fusion note) | "a single source of truth for all law enforcement agents" | R |
- **What it shows (I):** the same concept (resolve many records into one per person) across a USCIS privacy document, a DHS-wide Palantir justification and a vendor product. The words differ, so S3. "Golden record" is master-data-management shorthand for the same idea (confirmed D for the capability in the LSJ).
- **Tier A (partial):** EO 14243 §3(a) uses "the intra- and inter-agency sharing and consolidation of unclassified agency records" (D, fetch summary). "Consolidation" is the nearest authority-tier word to the LSJ's "consolidated record" (S3). The EO text has no "single" or "interoperab" (fetch summary). Still to check: EO 14248 §2.
| Jul 30, 2026 | B | HUD EICAM SORN (FR 2026-15428), an identity-and-access system (covered individuals include tenants and program beneficiaries) | records to be consolidated into the Okta Universal Directory, "the centralized, cloud-based source of truth for all user and device identities"; "EICAM unifies fragmented legacy identities" | D (read via PDF text) |
- CORRECTION (Oct 26 night): an earlier version said this is employee and contractor identity only. The SORN's covered individuals also list state and local partners, public housing authorities, lenders, and tenants and program beneficiaries. It stores a citizenship field and third-party identity-proofing risk scores, and says SSA-provided PII "is not shared with EICAM." It is useful as a base-rate example: "source of truth" and "unifies" are standard identity-management vocabulary across agencies (H1), which lowers the weight of PT-02 as signal.
- **H check:** H1 is strong (master-data-management and zero-trust identity vocabulary, OMB M-19-17).

### PT-03 · "eliminate data silos"  [G2, S2]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Mar 20, 2025 | A | EO 14243 (DCPD-202500382), title and §3 heading | "Stopping Waste, Fraud, and Abuse by Eliminating Information Silos"; §3 heading "Eliminating Information Silos" | D (title via GovInfo; §3 heading via fetch summary, verify against the text before quoting) |
| Sept 4, 2025 (posted May 14, 2026) | B | DHS Palantir LSJ | "This unified approach will eliminate data silos, reduce duplication, and enable real-time insights" | D |
| Sept 29–30, 2026 | B | CISA orders | vendor name "SiloSmashers" on "CISA Unified Data Platform and Integration Support Services" | D (name only; coincidence is likely) |
- **What it shows (I):** the word "silos" appears in the EO only in the title and the §3 heading (fetch summary), so the LSJ's "eliminate data silos" is an echo of the title, not a copy of operative text (S2). Both pair "silos" with efficiency or duplication language (EO §1: "eliminating bureaucratic duplication and inefficiency"; LSJ: "reduce duplication"). The vendor name is not a phrase match; keep it only as a curiosity.
- **H check:** H1 and H4 (EO text copied into a justification) both fit.

### PT-04 · "unified platform"  [G2, S1]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Aug 2025 | B | ICE Clearview J&A-25-0183 | vendor offers a "Unified Platform of identity management" | D |
| Sept 4, 2025 | B | DHS Palantir LSJ | "Unified Platform for Case Management and Analytics" | D |
| Sept 29–30, 2026 | B | CISA order …0039 | "CISA Unified Data Platform and Integration Support Services" | D |
- **Tier A and C gaps:** check the CISA 2026 plan and Peters plan for "platform" wording (neither was read for this phrase).
- **H check:** H1 and H3 (the Clearview wording is vendor-described). Low weight alone.

### PT-05 · "seamless"  [G2, S1, weak]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Sept 4, 2025 | B | DHS Palantir LSJ | "seamless data sharing and integration across all DHS components" | D |
| Aug 2026 | B | USCIS PLANXS P00022 JEFO | "a data hub which integrates and shares seamlessly" | D |
| 2026 | B | ICE VSPTS J&A-26-0230 | "seamless transition" (to Palantir Foundry) | D |
- **What it shows (I):** "data hub" plus "shares seamlessly" in a USCIS data-lake justification and "seamless data sharing" in the DHS-wide Palantir justification describe the same direction of travel. Weak as provenance because the word is everywhere.

### PT-06 · "cross-dataset" / merging unrelated data  [G2, S3]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Oct 29, 2024 | B | USCIS PLANXS II RFI | Tableau can "merge unrelated datasets together with less effort"; graph service "for investigators … 360-degree analytical view" | D |
| 2026 | B | ICE Booz Allen J&A-26-0191 | "advanced multi-vector analytics and cross-dataset exploration" | D |
- **What it shows (I):** both name cross-source joining as the point of the platform. Neither mentions voters.

### PT-07 · "targeting lists" / "targeting"  [G2, S1, decoy risk]
Different senses; keep the sense in the row.
| Date | Tier | Document | Exact words | Sense | Mark |
|---|---|---|---|---|---|
| Apr 25, 2025 | C | CNN on a DOGE "master database" | targeting lists | immigration enforcement | R |
| 2026 | B | ICE J&A-26-0191 (EO 14390) | "targeting lists of U.S. victims" | scam victims | D |
| Sept 23, 2026 | C | DHS statement | "We know who we are targeting ahead of time" | enforcement | R/D |
| Aug 2025 | B | Clearview J&A-25-0183 | investigative targeting of unidentified suspects (text redacted) | criminal suspects | D |
- **Rule:** do not link rows with different senses. The method note (Oct 21) already expects "fraud" and similar terms to be reused in several senses.

### PT-08 · "eligibility … verification" / "voter verification"  [G2, S2]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Oct 31, 2025 | B | SAVE SORN DHS/USCIS-004 reissued (FR 2025-19735) | "voter verification" purpose | D |
| Jun 10, 2026 | A | H.R. 8312 §2 (engrossed) | "identity, eligibility, account, and vital event verification and validation tools and analytical services" | D |
| Oct 23, 2026 | B | STATE-26 SORN (FR 2026-21695) | "voter eligibility" added to PURPOSE(S); routine use (w) "federal government verification platforms" | D |
- **What it shows (I):** a Treasury bill, a DHS SORN and a State SORN each build "eligibility" and "verification" into a data-sharing authority. H.R. 8312 does not mention voters; the other two do.
- **H check:** H1 (benefits-program vocabulary) is the most likely alternative.

### PT-09 · Written-in limits (the breadcrumbs)  [G2–G3, tracked as a category]
Phrases that state a limit. They show what the paper says is not happening.
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Jun 10, 2026 | A | H.R. 8312 §2 | program is "voluntary"; "does not include any investigative or law enforcement function"; "for no other purpose including any policy analysis and enforcement action purpose" | D |
| Sept 24, 2026 | A | CISA 2026 election plan | fusion centers "owned and operated by the states," which "keeps the function under state control"; services remain "voluntary" | D |
| Jul 22, 2026 | C | Peters 100-Day plan (proposal to CISA) | "The objective is not to replace the statewide voter-registration database" | D |
| May 14, 2026 | B | Palantir LSJ | "All data … wholly owned and controlled by DHS … can be accessed, managed, and shared as needed" (a control statement that also permits sharing) | D |
- **What it shows (I):** each of the three plans pairs a broad collection or coordination role with a written limit. Per the method rule, the limit wording is evidence of what was planned for, not proof it holds.
- **Next:** for each limit phrase, log the first later document that uses the system in a way the limit would address (e.g., a TRX user list that includes law enforcement; a DUA that adds Treasury data).

### PT-10 · "whole of government" / "every authorized asset"  [G2, S1]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Sept 22, 2026 | A | Hegseth memo | "this whole of government effort"; "mobilize every authorized asset, capability, and partnership under your command" | D |
- **Next:** search the DHS Aug 24 Mullin letter, the CISA plan, EO 14395 and NSPM-7 for the same pairing.

### PT-11 · Access to "all" records and "all State programs"  [G2–G3, S3]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Mar 20, 2025 | A | EO 14243 §3(a) | "full and prompt access to all unclassified agency records, data, software systems, and information technology systems"; §3(a)(2) "unfettered access to comprehensive data from all State programs that receive Federal funding" | D (fetch summary; verify) |
| Jun 10, 2026 | A | H.R. 8312 §2(B) | program "capable of receiving (including in bulk data formats and through systems that facilitate real-time data access) any data asset, information, or record related to the administration of Federal programs (including federally funded State-administered programs)" | D |
| Oct 2026 | A | EO 14399 §4(c), as quoted by the Oct 27 watch (not re-read by me) | SSA to "provide all necessary citizenship and identity data" | R (wording U) |
| Sept 4, 2025 | B | DHS Palantir LSJ | "unified search capabilities across multiple internal and external systems"; migration of "existing investigative data from legacy systems" | D |
- **What it shows (I):** the bill's "any data asset, information, or record" plus "federally funded State-administered programs" tracks the EO's "all unclassified agency records" and "all State programs that receive Federal funding." That is the same scope, in new words (S3), and the bill adds bulk and real-time ingestion. Neither the EO nor the bill mentions voters in the quoted text.
- **H check:** H4 (the bill borrowing the EO's frame) and H1 (program-integrity vocabulary).

---

### PT-12 · "continuous" identity verification / monitoring  [G2, S2, partial]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| Jul 15, 2026 | C | House Oversight subcommittee hearing, Socure witness (Burris) | "make continuous identity verification the standard across the lifecycle of an account"; "identity should be considered critical infrastructure" | D |
| Jun 10, 2026 | A | H.R. 8312 §2 | screening "relevant cyber activity … to review recipient or payee changes to virtual identity" (continuous in effect, word not used in the quote) | D |
| (to confirm) | B | ICE DASS "continuous monitoring" (registry ICE-10) | wording to be pulled from the DASS solicitation | U |
- **Next:** pull the DASS solicitation text and the PCIS and SAVE materials for "continuous" and "ongoing" wording. Note the second hit needs a verbatim "continuous" before it counts.

### PT-13 · "policy direction" / "evolving policy direction"  [G1-leaning, S1]
| Date | Tier | Document | Exact words | Mark |
|---|---|---|---|---|
| FY2027 (Mar 2026) | B | CISA FY2027 Congressional Justification, Election Security cut | "CISA will continue to focus on its core mission areas and adapt to evolving policy direction." | D |
| FY2027 (Mar 2026) | B | Same document, CFATS elimination | "realigned in accordance with current legislative and policy direction" | D |
- The phrase is reused for an unrelated program cut, so it is budget boilerplate (H2), not a signal about elections. Kept as a marker only.

## Search queue (not yet run)
1. (EO 14248 done Oct 26) "votes of citizens" + "dilut" in EO 14399, the SAVE America Act text and findings, and the DOJ California complaint.
2. "any data asset, information, or record" (H.R. 8312 §2) against the PRAC statute and OMB memos (EO 14243 comparison done, PT-11).
3. "single source of truth" / "golden record" / "master data" in USCIS and ICE solicitations and PIAs; in tier A texts.
4. "voter fraud organization" (HSI code) and "VFR/VRO" against EO 14395 §1 and the Fraud Task Force materials.
5. "platform" in the CISA 2026 plan and Peters plan against "Unified Data Platform."
6. "continuous monitoring" in DASS, SAVE and PCIS texts.
7. Run each new document's 2–3 most unusual phrases through this file first.

## Excluded as boilerplate (G1)
GSAR 509.406-3(a)(2) (GSA class deviation RGO-2026-01, Jan 15, 2026): "Refer possible criminal or fraudulent activities to the Office of the Inspector General" and the OIG-to-debarment-official step. Standard debarment procedure, not election-specific. Kept here only as a marker that routine OIG referral language is everywhere; the watch item is any new acquisition rule that adds data-sharing with OIG or PRAC systems.
"logical follow-on," "only one source capable," "interest of economy and efficiency," "unique or highly specialized," "fair and reasonable," "posted on SAM.gov within 14 days."

## Change log
- 2026-10-26 (late night): added HUD EICAM row to PT-02, new PT-12, RGO-2026-01 note in exclusions.
- 2026-10-26 (evening): EO 14243 read via fetch (PT-03, PT-02 tier A, new PT-11).
- 2026-10-26: Created. Ten seed entries from texts read in this project; no new searches run beyond those already in the notes.
