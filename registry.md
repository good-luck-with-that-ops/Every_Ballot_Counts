---
title: System Registry
permalink: /registry/
description: One entry per federal system, contract vehicle or data feed touching the 2026 election-data picture, with evidence marks.
---

One entry per federal system, contract vehicle or data feed that touches the election-data picture, with what is known, how we know it, and what is still unresolved. It is a living reference, updated as records are found. Started Oct 26, 2026.

**Marks (every claim):** D primary document · R reporting · I inference · U unresolved · K general knowledge, verify.
**Flow numbers:** f1–f57 are the numbered flows on the [architecture map](../map/architecture.html).
**Entry fields:** Owner · What it holds · Vendor/vehicle · PIA/SORN · Inbound feeds · Outbound feeds · Court mentions · Status since Jan 20, 2025 · Open questions/records (U).
**Sources:** entries cite the kind of source inline (a justification, a Federal Register notice, a court filing, a news report). Links to the underlying documents are being added over time; the supporting working notes are not published yet. Vendors are shown as infrastructure: a company appears only where a document ties it to a system, and no entry implies wrongdoing by any vendor.
**Caution:** this is research by an independent individual, not an investigation with inside sources. Inferences (I) and unresolved items (U) are labeled so you can weigh them. Corrections are welcome (see the [about page](../about.html)).

## Index

| ID | System |
|---|---|
| USC-01 | SAVE (Systematic Alien Verification for Entitlements) |
| USC-02 | PCIS (Person Centric Identity Services: Identity Index, PCER, Identity Resolution Queue) |
| USC-03 | PCQS (Person Centric Query Service) |
| USC-04 | DBIS / eCISCOR enterprise data lake and warehouse (PLANXS) |
| USC-05 | Senzing / Databricks graph (Graph Data Services) |
| USC-06 | FDNS and FDNS-DS (Fraud Detection and National Security) |
| USC-07 | USCIS source systems (CIS2, ELIS, CLAIMS 3/4, CPMS, CAMINO, Global, AR-11) |
| USC-08 | USCIS Vetting Center (UVC) and Operation PARRIS |
| USC-09 | EO 14399 State Citizenship Lists infrastructure |
| ICE-01 | ICM (Investigative Case Management) on Palantir |
| ICE-02 | ICE Enterprise Lakehouse |
| ICE-03 | ImmigrationOS and ERO Enforcement Case Management (Palantir) |
| ICE-04 | ELITE (Palantir targeting platform) |
| ICE-05 | RAVEn, RAVEn GO, Lead Tracking Tool, HORUS (HSI) |
| ICE-06 | FALCON |
| ICE-07 | HSI Innovation Lab ("iLab") profiles |
| ICE-08 | CBFCC (HSI Cross-Border Financial Crimes Center) election pipeline |
| ICE-09 | ATrac ("Alien Tracker") |
| ICE-10 | DASS (continuous-monitoring analytics, Thomson Reuters Special Services) |
| ICE-11 | VSPTS (Visa Security Program Tracking System) |
| ICE-12 | Mobile Fortify (NEC) and "Mobile Identify" |
| ICE-13 | Field capture peripherals: body cameras (Axon Evidence.com) and BITMAP devices (Parsons) |
| COM-01 | Clearview AI (face search) |
| COM-02 | LexisNexis (RELX) and Thomson Reuters CLEAR (commercial people-search) |
| COM-03 | OSINT and location tools (Penlink Tangles/Webloc, ShadowDragon, Fivecast, Babel Street, Zignal) |
| CBP-01 | TECS (subject records and lookouts) |
| CBP-02 | ATS (Automated Targeting System) |
| CBP-03 | TVS (Traveler Verification Service) |
| CBP-04 | Vehicle Biometric Capability Evaluation |
| CBP-05 | DSAI (Digital Solutions and Application Innovation) BPA forecast |
| DHS-01 | HART / IDENT (OBIM) and the NEC enterprise facial matcher |
| DHS-02 | DHS-wide Palantir BPA 70RTAC26A00000001 (LSJ FY25-00257) |
| DHS-03 | DHS-wide Databricks BPA 70RTAC26A00000010 ("enterprise data lakehouse") |
| DHS-04 | DHS-wide Carahsoft BPA 70RTAC26A00000011 (SSJ FY26-0119) |
| DHS-05 | HSIN (Homeland Security Information Network) |
| DHS-06 | DHS HQ election team "target-list compilation" |
| CIS-01 | CISA Palantir SaaS (70RCSJ26FC0000028) |
| CIS-02 | CISA Databricks PaaS (70RCSJ26FC0000030) |
| CIS-03 | CISA Unified Data Platform and Integration Support (SiloSmashers, 70RCSJ26FC0000039) |
| CIS-04 | CISA Socure / Lucid / AvePoint licenses (70RCSJ26FC0000042) |
| CIS-05 | FusionAware TRX "Elections Threats Reporting Exchange" (70RCSJ26FR0000062) |
| CIS-06 | CISA Esri GIS licenses (70RCSJ26FC0000012) |
| CIS-07 | NRMC AI orders (SOFITC3, 70RCSJ26FC0000036 and …0038) and National Risk Register support |
| CIS-08 | CI3 (classified critical-infrastructure briefing channel) |
| CIS-09 | HSIN-CI / CI-ISE support (70RCSJ26FR0000058) |
| CIS-10 | Stakeholder Engagement Division advisory support (AttainX, 70RCSJ26FR0000055) |
| HUD-01 | HUD Enterprise Identity, Credential, and Access Management (EICAM, HUD/OCIO-07) |
| DOJ-01 | DOJ state voter-roll holdings |
| DOJ-02 | National Fraud Enforcement Division / NFDC hub |
| DOJ-03 | DOJ Reconciliation Working Group |
| TRE-01 | Treasury Do Not Pay |
| TRE-02 | Fiscal Service analytics under H.R. 8312 §2 |
| TRE-03 | Treasury ".032" fraud-tip intake |
| TRE-04 | America.gov / Login.gov identity proofing |
| PRA-01 | PRAC analytics platform |
| PRA-02 | SSA "yes/no" agreement |
| SSA-01 | Numident |
| SSA-02 | Master Earnings File feed |
| STA-01 | STATE-26 (State Department records, passports) |
| STA-02 | Consular Consolidated Database (CCD) |
| CEN-01 | Census voter-file purchase (DataClear / Bridgetree) |
| CEN-02 | Census legal-status classification (residence rule) |
| FUS-01 | Fusion-center channel and 28 CFR Part 23 |


---

# PART A · USCIS

### USC-01 · SAVE (Systematic Alien Verification for Entitlements)
Map flows: f1, f2, f3, f10, f23, f40
- **Owner:** USCIS (D).
- **What it holds:** A point-in-time verification service that queries federal records for authorized users, not a standalone database (D, Bartell decl.). 2025 overhaul added SSN case creation and bulk upload (USCIS announcement May 22, 2025, D via AILA; the announcement does not mention SSA, and the SSA Numident link rests on PIA-006(d), D). 58M+ voter queries and 27 state agreements as of Feb 10, 2026 (D, Edlow testimony). A DHS memo reported Jul 24, 2026 says 10 states ran full rolls through it (R, Daily Signal; the memo's date and text not seen directly; report source #34). SSN lookups of U.S.-born citizens opened to election officials in May 2025, with a last-four-digits option added Aug 15, 2025 (R, NPR, Sept 10, 2025).
- **Vendor / vehicle:** FY26 "voter verification service" $70.7M (D per CMP note; PIID not recorded here, U). Vendor U. VIS (the system behind SAVE and E-Verify) draws from eCISCOR (D, eCISCOR PIA 2015).
- **PIA / SORN:** SAVE SORN DHS/USCIS-004 reissued Oct 31, 2025, FR 2025-19735 (D): adds citizens by birth, SSA data, driver's-license sources, "voter verification" purpose. The SORN says SAVE "is not to be used for administrative (noncriminal) immigration enforcement purposes" (D, SORN FR 2025-19735); the Bartell declaration ¶16 says DHS does not use SAVE that way (D). SAVE PIA 2020 describes the PCER microservice (D, baseline); DHS/USCIS/PIA-006(d), dated Oct 31, 2025 (D, read Oct 27), documents five changes: voter registration and voter-maintenance-list verification; collection of SSNs "which may include those of U.S. born citizens"; sharing among USCIS, SSA and State; a bulk "list processor"; and no fee for non-federal agencies. SSN queries send name, date of birth and a full or partial SSN to SSA, which returns match flags, a citizenship indicator (A to F), a foreign-born indicator, state or country code, Alien number where applicable, and a death indicator. Retention is ten years from completion of the verification (NARA N1-566-08-07), longer if part of an ongoing law-enforcement investigation. The PIA states that agencies carry the notice and consent duties and that individuals get no opportunity to consent at the USCIS level (D).
- **Inbound feeds:** [f1] state voter rolls in bulk by SSN/license no. (D). [f2] Numident (D). [f57] eleven further systems SAVE queries to answer agency requests: Central Index, GLOBAL, RAILS, Salesforce CRM, SEVP, EID, ADIS, OneNet, TSA OIA TIM, MEPCOM IRIS, Education FSA CPS (D, PIA-006(d) pp. 7–9; the PIA also lists CPMS, ELIS, CLAIMS 3, eCISCOR, Numident, CMS and the DOJ immigration-court exchange, already on the map). [f3] DMV/Nlets, "not live at the time of publication" (D). [f23] eCISCOR warehouse → VIS (D). PIA-006(d) lists the federal systems SAVE queries: USCIS CIS, ELIS, CLAIMS 3, eCISCOR, GLOBAL, RAILS, CPMS and a Salesforce CRM; DHS OneNet, ICE SEVP and EID, CBP ADIS, TSA I&A TIM; plus MEPCOM, Education FSA CPS, CMS, SSA Numident, DOJ EOIR's EIRS, and State's CCD and ACRQ (D).
- **Outbound feeds:** [f10] SAVE → FDNS referrals stopped after the LWV order, but pre-order referrals kept under the FDNS SORN (D, Bartell ¶¶12–14). PIA-006(d) says that when potential fraud or misuse is indicated, SAVE information may be shared case by case with DHS internal law-enforcement organizations, named as ICE and CBP (D, PIA p. 15). The PIA text does not mention HSI, FDNS or the CBFCC; the SAVE-to-HSI lead flow [f40] rests on reporting (R). [f40] By Jan 2026, about 25,000 of the leads HSI was working came from SAVE flags; a further ~15,000 leads went to HSI's cross-border financial crimes unit (R, ProPublica Aug 14, 2026). Whether the 15,000 are SAVE-derived is not stated.
- **Court mentions:** LWV v. DHS (D.D.C., filed Sept 30, 2025): modified SAVE vacated Jun 22, 2026 (D; the Westlaw cite previously listed could not be verified). DHS v. LWV, No. 26A308, SCOTUS stay Sept 25, 2026 (D). LWV/EPIC/LULAC v. DHS, 1:26-cv-03602, filed Oct 15, 2026, seeks deletion of voter information collected under the Voter Data Collection Policy (D). "2026 WL 1784297" is not independently verified (U). CNA v. Mullin ECF 46-1 ¶¶12–16 (D). US v. California complaint fn. 1: the USCIS process "was done independent of SAVE" (D, complaint p. 9 n.1). Arizona AG and Secretary of State v. Maricopa County Recorder, filed Oct 21, 2026: 25 citizens flagged by SAVE as "not eligible"; the Recorder agreed Oct 23 to reinstate them (R, Votebeat, KJZZ).
- **Status since Jan 20, 2025:** Apr 22, 2025 DHS/USCIS/DOGE "comprehensive optimization" announced (D, AILA posting). May 22, 2025 SSN case creation and bulk upload announced (D, AILA posting; SSA link per PIA-006(d)). Oct 31, 2025 SORN (D). Jun 22, 2026 vacatur (D). Sept 25, 2026 stay, SAVE revived (D). Apr 30, 2026 bulk CSV gained an optional "Custom Agency Reference" field (R, secondary source; USCIS notice not yet read). The June 2026 SAVE User Reference Guide (reviewed Jun 23, 2026) describes a "Custom Agency Reference" for internal tracking in single-case creation and in case responses, and lists the minimum bulk-upload CSV fields as name, date of birth, a numeric identifier and the benefit sought; it does not list the field for bulk upload (D). The guide prints the SORN as "DHS/USCIS-044" with the cite 90 FR 48948 (Oct 31, 2025), an apparent typo for -004. USCIS publishes an open dataset of "all SAVE cases" Jan 2016–Jul 2026 (posted Sept 14, 2026) that excludes voter-verification and oversight cases (D, USCIS data page).
- **Open questions / records (U):** Does the "SAVE → HSI flags shared (2025 deal)" channel really run through SAVE or through the data layer (USC-04/06)? Request: SAVE SOW and PIID for the $70.7M; list processor volumes and error handling; USCIS–SSA interconnection agreement; what the 10 states' full-roll runs returned; the "Custom Agency Reference" field's use.

### USC-02 · PCIS (Person Centric Identity Services: Identity Index, PCER, Identity Resolution Queue)
Map flows: f13, f14, f15, f16, f17, f18, f19, f53
- **Owner:** USCIS (D).
- **What it holds:** One profile per person in an "Identity Index" combining biographic and biometric data, status and history; "a single, trusted source of biographical and biometric information" (D, PIA-087). In production since Nov 2021 (D). Matching uses "a weighted absolute scoring model and a machine-learning model"; inputs include A-number, name, DOB, country of birth, fingerprint ID, SSN (D). Close matches go to the Identity Resolution Queue, worked by human "Identity Specialists" (D). The "~500M records from 8 systems" figure is Excella's public description of Jun 18, 2025, not the PIA's (R).
- **Vendor / vehicle:** Genesis Consulting Partners 70SBUR21F00000076, $4.1M ($4,113,565 across actions dated Mar 31, Jul 19 and Nov 30, 2021; a BPA call), Apr 2021–Nov 2022, technical oversight (D, USAspending). Steampunk 70SBUR21F00000109, $7.9M, May 2021–Dec 2024, strategy and implementation (D). Excella described PCIS publicly (contract U). Senzing licensed over the same period (USC-05).
- **PIA / SORN:** DHS/USCIS/PIA-087, Dec 2022 (D). No update found after Dec 2022 (U). Covering SORNs: DHS/USCIS-001 (A-File) and -007 (Benefits Information System) (D per PCIS-B). Both gained a Treasury Do Not Pay routine use (FR 2025-24030, effective Jan 30, 2026) (D).
- **Inbound feeds:** [f16] about eight USCIS systems, "the list will change" (D, PIA p. 8). [f13] CBP TECS. [f14] CBP ATS. [f15] IDENT biometrics. [f17] DOJ EOIR court data. [f18] State Consular Consolidated Database (all D, PIA pp. 11–14). Also ADIS, ICE SEVIS and ENFORCE (D). SSN is a stored field; no SSA source named (D).
- **Outbound feeds:** [f19] Identity Resolution Queue. "PCIS does not share data outside of DHS as part of its normal operations" (D, p. 31). Users: USCIS, ICE, CBP; I&A will access; State requested access (D, p. 7); FDNS officers are named users (D, p. 16). [f53] PCIS-covered SORNs now permit disclosure to Treasury Do Not Pay (D, permitted not shown used). Query front end: USC-03.
- **Court mentions:** No complaint or order names PCIS (D, absence per PCIS-A §6). The LWV complaint names the Data Lake (USC-04).
- **Status since Jan 20, 2025:** Mar 28, 2025 DOGE access to the data lake that PCIS sits on (R, FedScoop). Oct 6, 2025 FDNS, a named user group, became a law-enforcement entity (D). Dec 31, 2025 Do Not Pay routine use added to covering SORNs (D). Dropped from the Oct 21 report despite being found Oct 13–14 (project process note).
- **Open questions / records (U):** Any PCIS PIA update after 2022. PIA appendices listing sources added since. Do voter files or state rolls enter PCIS? Identity Resolution Queue volumes and who works it. Request: USCIS privacy threshold analyses for the voter matching.

### USC-03 · PCQS (Person Centric Query Service)
Map flows: none on the map
- **Owner:** USCIS (D).
- **What it holds:** A query service that "provides a way to quickly identify citizenship status using only a name and date of birth" (D, wording from the 16 AGs' Oct 14, 2024 letter). State Department staff use PCQS, and eCISCOR is a data provider to it (D, eCISCOR PIA). PCQS predates PCIS, and the PCIS PIA says PCQS "will be subsumed into or replaced by PCIS" and that PCIS draws on PCQS data (D, PCIS PIA, Dec 2022). Whether PCQS now fronts PCIS is the project's reading (I). PCQS PIAs exist (2018 update).
- **Vendor / vehicle:** U.
- **PIA / SORN:** U (PCQS PIA not located).
- **Inbound feeds:** eCISCOR (D). PCIS (I; the PCIS PIA describes the flow in the other direction, PCQS into PCIS).
- **Outbound feeds:** State Department users (D). Other agencies U.
- **Court mentions:** None found (U).
- **Status since Jan 20, 2025:** The AGs' Oct 14, 2024 letter objected to DHS's "refusal to grant access" to PCQS and to SAVE requiring a DHS identifier (D, letter text). The 2025 SAVE overhaul (SSN searches, SSA data) delivered most of what the letter asked (I).
- **Open questions / records (U):** Current user agencies. Any state or election-office access since 2025. PCQS PIA and SORN. Relationship to SAVE's SSN and bulk queries.

### USC-04 · DBIS / eCISCOR enterprise data lake and warehouse (PLANXS)
Map flows: f20, f22, f23, f24, f25
- **Owner:** USCIS; the Office of the Chief Data Officer appears to steward it (I).
- **What it holds:** DBIS has seven components (D, PLANXS II RFI, Oct 29, 2024): eCISCOR relational and dimensional data; SMART (Oracle BI); SAS Predictive Modeling Environment; eCISCOR Bigdata on Databricks, "also referred to as the USCIS enterprise data lake"; Tableau analytics; Graph Data Services (USC-05); SPAR social-listening (Sprinklr). It stores "an exact copy" of connected source systems (D, 2018 PIA per CMP). The eCISCOR PIA lists reporting, analytics, statistical analysis and adjudication purposes (D, PIA §3.1); the phrases "AI and ML" and "analytic or adjudicative use" come from the PLANXS II notice, not the PIA (U, not independently read).
- **Vendor / vehicle:** PLANXS task order 70SBUR21F00000194 under NIH CIO-SP3 75N98119D00087, Octo Metric LLC, $95.3M obligated, Sept 24, 2021–Dec 11, 2026, potential end Feb 11, 2027 (D). Mods: P00017 $20.8M (Feb 5, 2025); P00018 +2 Tableau FTEs (Sept 11, 2025); P00021 option year 5 $9.0M (Feb 11, 2026); P00022 change order $5.8M (Aug 10, 2026) (D). Extension justification ("JEFO Exceeding the MP_PLANXS Extension," posted Aug 17, 2026) read Oct 26: P00022 extends the order up to 6 months, Aug 12, 2026–Feb 11, 2027, sole source to Octo Metric under RFO 16.507-6(b)(2) "unique or highly specialized" (D). It states PLANXS II "was competitively solicited and awarded," the award was protested, the agency issued a stop-work order on it, and "any other vendor would have less than 30 days to understand the data environment and transition services currently performed by 70 FTEs"; a new entrant needs at least 90 days (D). The winner of PLANXS II and the protest forum are not stated (U). This replaces the earlier "no PLANXS II award found, incumbent likely extended" reading (see J4). The J&A calls Databricks "the primary component for extracting value," names SMART, the SAS Predictive Modeling Environment and eCISCOR BigData and BigData Analytics "unique to USCIS," and lists task areas including AI/ML and predictive and prescriptive analytics (D). It mentions no voter or election work (D). Databricks licenses: 70SBUR25F00000064 $6.27M (Mar 31, 2025–Mar 30, 2026; tag "SECTION 2(D) SECTION 4(A)" unexplained, U); 70SBUR25F00000211 $1.48M (Sept 24, 2025–Mar 30, 2026); no USCIS renewal found, possibly folded into DHS-03 (I). Address verification: 70SBUR26F00000061 (New Tech/Melissa), $191K, Mar 16, 2026–Mar 15, 2027, "critical for maintaining data integrity within enterprise data lake" (D). Stack: AWS, Databricks E2/Delta Lake/MLflow, Informatica incl. Address Doctor, SAS Visual Investigator, Senzing Runtime API v3.10.2, Tableau, Sprinklr (D, RFI).
- **PIA / SORN:** eCISCOR PIA Jan 23, 2015 (Appendix A lists 16 sources, only one external: Treasury Pay.gov/TRS) (D). Data lake PIA Jul 26, 2018; no SORN of its own, relies on source-system SORNs (D per CMP). Updates since U.
- **Inbound feeds:** [f20] 130+ internal USCIS source connections (D, RFI). External inbound ~12 in 2024, up from 1 in 2015; which ones U. [f24] Sprinklr social listening fed back into the lake (D, RFI). [f25] DOGE access via Databricks, Mar 28, 2025 USCIS CIO memo requested by DHS CIO and Chief Data Officer (R, FedScoop).
- **Outbound feeds:** [f21] to the Senzing/Databricks graph. [f22] to the warehouse. [f23] eCISCOR → VIS/SAVE (D, PIA App. C). eCISCOR also supplies PCQS (USC-03). ~12 outbound internal and 3 external outbound connections (D, RFI; which U). USCIS sends ad hoc "Computer Readable Extracts" to federal agencies "for law enforcement purposes" (D, PIA §6.1).
- **Court mentions:** LWV v. DHS complaint ¶¶17–18, 160–172 allege the lake pools SSA, IRS, National Directory of New Hires, CMS Medicaid, DOL, HHS UC-portal data and, "on information and belief," state voter rolls, with DOGE staff named (D as allegation, not finding). LWV/EPIC/LULAC 1:26-cv-03602 seeks deletion of voter information collected under the Voter Data Collection Policy; the complaint does not mention the data lake, eCISCOR, Databricks, PCIS, Senzing or FDNS, so it is listed here only as related litigation (D).
- **Status since Jan 20, 2025:** Mar 28, 2025 DOGE access (R). Mar 31, 2025 Databricks order (D). Aug 2026 P00022 supports "a data hub which integrates and shares seamlessly" (D). External feeds grew from 1 (2015) to ~12 (2024) (D).
- **Open questions / records (U):** Which ~12 external inbound and 3 outbound connections, with dates added since Jan 2025. Data lake PIA after 2018. PLANXS SOW and modifications. GAO decision B-424623 (Oct 8, 2026) denied Octo Metric's protest of a USCIS task order to AEX Digital under RFQ 70SBUR26Q00000052: GSA MAS 54151S, total small business set-aside, issued Jun 22, 2026, AEX evaluated $88,090,259 against Octo's $100,598,462; Octo is described as the incumbent (D, GAO). That this is PLANXS II is our inference from the incumbent, the IT-support and analytics scope and the timing (I). If so, AEX Digital would inherit the data lake work; whether it inherits DOGE-era access arrangements is U. Ingestion logs and interconnection agreements for state voter files. What "Section 2(d) Section 4(a)" cites. DHS's answer to the LWV complaint's lake paragraphs.

### USC-05 · Senzing / Databricks graph (Graph Data Services)
Map flows: f21
- **Owner:** USCIS (D).
- **What it holds:** An entity-resolution graph over the lake: "relationships between people, locations, accounts, assets, events and case details"; "knowledge graphs give investigators a 360-degree analytical view" (D, RFI). Senzing's order text: "supports persistent indexes of persons" (D).
- **Vendor / vehicle:** Senzing via GovSmart. 70SBUR24F00000273, $1.06M (two $529,562 actions, Sept 19, 2024 and Aug 28, 2025), Sept 30, 2024–Sept 29, 2026 (D, USAspending). Renewal 70SBUR26F00000235, $610,342, action date Sept 25, 2026, Sept 30, 2026–Sept 29, 2027 (D, USAspending); the "3 offers" figure is from the earlier source (U). That USCIS has bought Senzing every year since 2022 is not established: only the 2024 and 2026 orders were checked (U). Justification for either order not retrieved (U).
- **PIA / SORN:** None specific found (U).
- **Inbound feeds:** [f21] from the lake (D).
- **Outbound feeds:** Investigators and FDNS analysts (I). Downstream destinations U.
- **Court mentions:** None names Senzing (D, absence). US v. California ¶¶33–43 says USCIS used unnamed "third-party software" with high/medium/low tiers; DHS disputed that USCIS used third-party software and said commercial third-party data and other government data were used to supplement public records (R, Newsweek). Senzing is one possible candidate (I); nothing ties it (U).
- **Status since Jan 20, 2025:** Renewal order dated Sept 25, 2026 (D, USAspending). Comparable CBP tool: Tamr entity resolution, 70B06C22C00000067, $1.6M, Sept 2022 (D).
- **Open questions / records (U):** SOWs for both Senzing orders. Data-source configurations. Do FDNS or OCDO run voter files through it? Name and contract of the "third-party software." Vendors are infrastructure; nothing implies a company knows of any use.

### USC-06 · FDNS and FDNS-DS (Fraud Detection and National Security)
Map flows: f7, f8, f9, f10, f11, f12
- **Owner:** USCIS FDNS (D). Designated a law-enforcement entity as of Oct 6, 2025 (D, Bartell n.1, which does not cite the rule). A separate rule, 90 FR 42797 (FR 2025-16978; published Sept 5, effective Oct 6, 2025), codifies the USCIS Director's law-enforcement authorities and does not itself designate FDNS (D). FDNS's Criminal Investigative Division "was not directly involved" in the investigations into unlawful voting (D, Bartell n.1).
- **What it holds:** Fraud and national-security case records (FDNS-DS is the case system; specifics K, U here). Receives target lists treated as "presumptively valid"; agents were ordered to complete a minimum of 40 suspected-subject reviews, with no more than twelve minutes to clear a person from the list (D, CNA order ECF 87; the quota is also in the New Yorker, R). The order does not say who the "agents" are, and it attributes the clearing and TECS creation to "USCIS personnel" without naming FDNS (FDNS appears only in a sealing passage and a methodology reference). Clears names against commercial databases; the order notes such databases are "typically used for targeted advertising" and include addresses, demographics and vehicle ownership (D, CNA order). USCIS has created TECS records for U.S. citizens, per the order relaying the whistleblower disclosure (an allegation the court recounts, not a finding; D).
- **Vendor / vehicle:** TRSS social-media vetting pilot 70SBUR26P00000021, $2,756,396, Sept 15–Oct 14, 2026, one offer, "only one source" under FAR 6.302-1, described as "FDNS Tactical Operations Division requires social media vetting services to enhance investigations" (D, USAspending, read Oct 27). SAM combined synopsis/solicitation "Integrated Commercial Vetting and Data-Analysis Pilot Services" (solicitation 70SBUR26R00000015; the SAM page prints the notice ID as 70SBUR25R00000015), posted Aug 27, 2026, Amendment 0001 Sept 2 extending offers to Sept 9, 2026 (D, SAM notice and attachment read Oct 27). The notice states USCIS intends a noncompetitive award to Thomson Reuters Special Services because no other source showed it could provide the whole integrated requirement within a 30-day pilot (anticipated Sept 15–Oct 14, 2026); TRSS's CLEAR Risk Inform/CLEAR Batch with RTIA, Fivecast MATRIX and analyst/data-scientist support met the minimums. The PWS is titled "for FDNS" and names FDNS's Tactical Operations Division. It calls for batch processing of Government-provided "records of interest," a base quantity of up to 100,000 input records for the pilot (not per batch), identity resolution using commercial and public data including incarceration/arrest information, discovery and correlation of online accounts and social-media activity, Government-defined risk-indicator categories, up to ten reports of individuals with potential risk indicators, and an advisory-only limit (no adjudicative, eligibility, enforcement or adverse-action determinations). The contractor may not use the data for model training or resale. The solicitation text does not mention voters or elections (D). LexisNexis (RELX) 70SBUR25F00000065, $5.4M, Mar 2025–Mar 2027 (D). Axon body cameras 70SBUR26F00000181, $159,675, USAspending action date Aug 26, 2026 (D).
- **PIA / SORN:** FDNS SORN holds pre-order SAVE referrals (D, Bartell). SORN number not confirmed (K lead: DHS/USCIS-006, verify). FDNS-DS PIA U.
- **Inbound feeds:** [f7] target lists compiled by DHS (D, CNA order: "DHS builds the target list"; the order names no office, and the "HQ election team" attribution is the map's label, I). [f10] SAVE referrals, stopped (D). [f9] commercial data brokers (D). [f8] queries to state voter-lookup portals (R, allegation in a whistleblower disclosure to Sen. Padilla, publicized Sept 14, 2026).
- **Outbound feeds:** [f11] TECS records (D). [f12] flagged people reach HSI under the Jul 23, 2025 USCIS–ICE MOA (D title; text not public).
- **Court mentions:** CNA v. Mullin ECF 46-1 (Bartell, Sept 28), ECF 67, ECF 87 (Oct 21 PI order). "FDNS is not a SAVE user agency" (Bartell ¶15). LWV v. DHS (D).
- **Status since Jan 20, 2025:** May 2, 2025 Delegation 15006 (D). Jul 23, 2025 fourth USCIS–ICE MOA (D title). Sept 5, 2025 rule, effective Oct 6 (D). Dec 5, 2025 Vetting Center (USC-08). Apr 2026 funding request for 200 special agents (R). Aug 31, 2026 DHS "Surge Initiative Guidance" directing HSI agents to prioritize election-related field investigations (D, CNA order; FDNS not named).
- **Open questions / records (U):** FDNS CID charter. All four MOAs and annexes; any post-Oct 6, 2025 addendum. IBFU referral criteria and USCIS→CBFCC referral counts. TECS disposition codes for cleared people. FDNS-DS PIA and SORN currency.

### USC-07 · USCIS source systems (CIS2, ELIS, CLAIMS 3/4, CPMS, CAMINO, Global, AR-11)
Map flows: f16, f20
- **Owner:** USCIS (D).
- **What it holds:** A-files, benefit applications, biometrics, change-of-address records (D, PCIS PIA). CIS2 retention is permanent; CPMS keeps biometric records 100 years from birth (D).
- **Vendor / vehicle:** Various, U.
- **PIA / SORN:** A-File DHS/USCIS-001 and Benefits Information System DHS/USCIS-007, each with a Do Not Pay routine use effective Jan 30, 2026 (D).
- **Inbound feeds:** Applicants, other DHS components (D, general).
- **Outbound feeds:** [f16] to PCIS Identity Index; [f20] to the data lake (D).
- **Court mentions:** None specific (U).
- **Status since Jan 20, 2025:** Dec 31, 2025 routine-use change (D). Source list "will change" (D, PIA); current list U.
- **Open questions / records (U):** Current inbound list for PCIS and the lake, with dates added.

### USC-08 · USCIS Vetting Center (UVC) and Operation PARRIS
Map flows: none on the map
- **Owner:** USCIS FDNS (D).
- **What it holds:** Centralized enhanced screening in Atlanta of pending and already-approved applications, using classified and unclassified DHS, law-enforcement and IC resources and AI; prioritizes countries of concern; the announcement says it "aligns with" EO 14161 (D, Dec 5, 2025 announcement via AILA). Operation PARRIS re-checks admitted refugees, with interviews and referrals to ICE (D).
- **Vendor / vehicle:** Forecast F2026075843 "USCIS Vetting Center (UVC) Project Consulting Support," published Sept 23, 2026, owner FDNS, $2–5M, OASIS+ small-business competition, new requirement, solicitation est. Nov 2, 2026, award Q1 FY27, completion Dec 31, 2028 (R, via CGA; forecast not re-read here).
- **PIA / SORN:** U.
- **Inbound feeds:** U. **Outbound feeds:** Referrals to ICE (D, PARRIS description).
- **Court mentions:** None found (U).
- **Status since Jan 20, 2025:** Dec 5, 2025 announcement (D). Oct 14, 2026 interim final rule 2026-20956 (USCIS-2026-0397) cuts the refugee NOIT response time from 30 to 10 days, justified by PARRIS/UVC reviews (R, CGA).
- **Open questions / records (U):** UVC data sources. Does it touch voter or citizenship matching? Forecast text and SOW when posted.

### USC-09 · EO 14399 State Citizenship Lists infrastructure
Map flows: none on the map
- **Owner:** DHS/USCIS with SSA (D, EO text).
- **What it holds:** EO 14399 §2(a) (Mar 31, 2026) directs DHS/USCIS to "compile and transmit … a list" from federal citizenship and naturalization records, SSA records, SAVE data and other federal databases. §4(c): SSA "shall provide all necessary citizenship and identity data"; DHS builds the "infrastructure necessary to compile, maintain, and transmit" it within 90 days (D). A "State Citizenship Lists" portal is mentioned in earlier research notes (U).
- **Vendor / vehicle:** U.
- **PIA / SORN:** U. Watch for a new SORN or PIA.
- **Inbound feeds:** Federal citizenship and naturalization records, SSA, SAVE (D, EO text); actual feeds U.
- **Outbound feeds:** Lists to election officials (D, EO text). DOJ said in Sept that a list before the midterms "We might. It's possible. I cannot say" (R, DOJ attorney at the Sept 25 hearing before Judge Xinis, answering about the portal and state citizenship lists; Democracy Docket).
- **Court mentions:** The government's CNA opposition (ECF 46) relies on EO 14399 and dates it Mar 21, 2026; the brief itself cites 91 FR 17,125 (Mar. 31, 2026), and the project uses Mar 31 (D).
- **Status since Jan 20, 2025:** EO signed Mar 31, 2026; 90-day infrastructure deadline passed ~Jun 29, 2026 (D by arithmetic).
- **Open questions / records (U):** Has any list been transmitted? Which system compiles it (SAVE, the lake, PCIS)? SSA feed under §4(c). EO date discrepancy.


---

# PART B · ICE / HSI

### ICE-01 · ICM (Investigative Case Management) on Palantir
Map flows: f37
- **Owner:** ICE/HSI (D).
- **What it holds:** HSI case records, subjects, vehicles, reports and media (D). The current ICM was deployed in 2016 as a modified COTS system "built on the Palantir Gotham platform," hosted in Palantir's cloud, with O&M under task order 70CTD022FR0000170 "until 2027" (D, ICE LSJ J&A-25-0266). Palantir ties go back earlier (R/K: EPIC FOIA; Intercept 2017). The ICM Interface Hub publishes ICE subject records to CBP's TECS, where they "serve as 'lookout records'" (2016 PIA, R via Biometric Update, Oct 4, 2026). The RAVEn PIA lists ICM as a daily source into RAVEn and says RAVEn products are entered manually into "a case management system"; an automatic feed back to ICM is not described (D, RAVEn PIA).
- **Vendor / vehicle:** Palantir. Order 70CTD026FC0000018, $45,848,617, Jun 26, 2026, HSI modernization for Investigative Case Management and analytics (D). ICM named in the DHS Palantir LSJ as "built on Palantir's platforms" (D). The replacement is justified in ICE LSJ J&A-25-0266 (sole source to Palantir under FAR 8.405-6(a)(1)(i)(B); firm-fixed-price, one 12-month base plus four 12-month options; 42 vendors assessed; FedRAMP High required on day one), posted to SAM Jan 16, 2026 as notice ICE_JA-25-0266 (D, read Oct 27). Whether this order sits under BPA 70RTAC26A00000001 is U.
- **PIA / SORN:** ICM PIA (2016) (D per the PIA as cited by Biometric Update; PIA text not re-read). ICE-008 Search, Arrest and Seizure SORN modified Jul 2025, FR 2025-13609, now covers witnesses, bystanders and people "incidentally recorded," with biometric, geolocation and commercial data (D). ICM's own SORN U.
- **Inbound feeds:** [f37] leads from RAVEn (D). Field entries by HSI agents, including the observer records in Hilton (R).
- **Outbound feeds:** TECS lookouts via the Interface Hub (R). The LSJ requires an "Enterprise Lakehouse repository" that can be an authoritative ICE data source, hold seizure data from CBP and arrest data from EID/EAGLE, and "share subject information with CBP for lookout and seizure tracking purposes" (D, LSJ J&A-25-0266). It must interoperate with CJIS, DOJ, NLETS, OBIM and CBP (D). "Derived analytical data" must be "owned wholly/entirely by ICE" (D).
- **Court mentions:** Hilton v. Noem (D. Me.; some secondary sources give the caption as "Hilton v. Mullin," No. 69985): an HSI agent photographed observers in Maine (Jan 2026, "Operation Catch of the Day") and entered eight people into ICM; the government's filing (ECF 117, Sept 18) acknowledges one plaintiff's ICM entry "led to" a Mar 2026 border stop and continued enhanced screening (R via Biometric Update). Newly unsealed filings include agent deposition excerpts; other depositions remain sealed (R, Press Herald Oct 5, 2026). ECF 132 was filed Oct 2, 2026; its attachment 132-40 is Elinor Hilton's supplemental declaration (D, read Oct 27). She states that on Jan 21, 2026 agents photographed her and her car and said they would put observers on a "watchlist," and that on Jun 16, 2026 an unmarked vehicle stopped outside her driver's-license address (declarant's account; allegations, not findings). Whether ECF 132 itself contains agent deposition excerpts is not confirmed (U). The case is No. 2:26-cv-00092-JAW. Plaintiffs made their own names public.
- **Status since Jan 20, 2025:** Jul 2025 SORN modification (D). Jan 2026 observer entries (R). Jun 2026 modernization (D). ICE requires ICM data to be migrated to a new Enterprise Lakehouse; progress not reported (R).
- **Open questions / records (U):** What happens to analytic products when source records are corrected or deleted? Pull Hilton docket exhibits (government declarations describing systems). ICM–TECS interface logs for election-related cases. Which BPA the modernization order sits under.

### ICE-02 · ICE Enterprise Lakehouse
Map flows: none on the map
- **Owner:** ICE (R).
- **What it holds:** Per the ICE LSJ: case management records (people, businesses, vehicles), workflows, reports and attached media, plus data from other law-enforcement agencies such as CBP seizures and EID/EAGLE arrests, in a single repository supporting investigative analytics (D, J&A-25-0266).
- **Vendor / vehicle:** Part of the Palantir ICM modernization (J&A-25-0266; order 70CTD026FC0000018, ICE-01) (D); LSJ requires one "unified/single integrated platform" for case management and analytics. Relationship to the DHS-wide Databricks lakehouse (DHS-03) is U (I: the department's common layer).
- **PIA / SORN:** U.
- **Inbound feeds:** migrated ICM data (R); outside law-enforcement data (U, source not located). **Outbound feeds:** CBP, for lookout and seizure tracking (R, expected). The lakehouse "must interoperate" with DOJ, FBI CJIS, NLETS and OBIM (R); interoperability is not the same as sharing.
- **Court mentions:** None found.
- **Status since Jan 20, 2025:** ICE is requiring ICM data to be migrated into it (R); progress is a watch item (U).
- **Open questions / records (U):** Vendor, ATO, requirements document and any J&A. Whether CISA's Databricks order (CIS-02) shares the platform. Retention and correction rules for derived data.

### ICE-03 · ImmigrationOS and ERO Enforcement Case Management (Palantir)
Map flows: none on the map
- **Owner:** ICE ERO (D).
- **What it holds:** A "lifecycle" targeting and case platform; $30M prototype in 2025 (R/baseline). The DHS Palantir LSJ names ImmigrationOS and ICM as built on Palantir platforms (D).
- **Vendor / vehicle:** Palantir. ERO modernization for Enforcement Case Management 70CTD026FC0000012, $86,271,599, May 5, 2026 (D). BPA parentage U.
- **PIA / SORN:** U.
- **Inbound / outbound feeds:** U. No voter link shown (U).
- **Court mentions:** None found.
- **Status since Jan 20, 2025:** 2025 prototype; May 5, 2026 order (D).
- **Open questions / records (U):** ImmigrationOS PIA, requirements, interfaces with ELITE and ICM.

### ICE-04 · ELITE (Palantir targeting platform)
Map flows: f36
- **Owner:** ICE (D).
- **What it holds:** A targeting platform. A senior ICE official said agents have a "list of 20 million people" on their iPhones through Palantir tools (R, 404 Media, May 12, 2026); that this is ELITE is our inference (I). FOIA records (Bates 057, Jul 6–7): voter data "pending Palantir entry into ELITE" (D); six states listed: Missouri, Michigan, New Mexico, Connecticut, Georgia, Kentucky (R via CGA); reported counts are records, and no source gives unique persons (I).
- **Vendor / vehicle:** Palantir (DHS LSJ covers all BPA orders). ELITE-specific order U.
- **PIA / SORN:** U.
- **Inbound feeds:** [f36] iLab output; "use U" (D/U). **Outbound feeds:** HSI leads and targeting (I).
- **Court mentions:** The Oct 24 PCIS note lists ELITE among systems "named in litigation"; which filing U. FOIA production (Democracy Forward, Oct 1, 2026) is in the shared evidence base (D).
- **Status since Jan 20, 2025:** Jul 2026 FOIA emails (D). An unnamed Palantir spokesman told WIRED, per Biometric Update (Oct 9, 2026), that "voter roll data has never been integrated into ELITE" (R; WIRED original not located). A source familiar with the matter told Democracy Docket the data "was not and is not integrated into ELITE" (R). The two statements are unreconciled (U).
- **Open questions / records (U):** Was the "pending entry" completed? ELITE PIA/SORN. Palantir's July emails vs its denial.

### ICE-05 · RAVEn, RAVEn GO, Lead Tracking Tool, HORUS (HSI)
Map flows: f12, f30, f31, f32, f33, f34, f37, f38, f42, f51, f52
- **Owner:** ICE/HSI (D).
- **What it holds:** Core analytics, the Lead Tracking Tool, RAVEn GO (mobile field interviews) and HORUS (face-image isolation and matching) (D, PIA). RAVEn GO record fields: agent; "criteria for interview and organizational affiliation indications"; date and location; citizenship; family citizenship; contacts; vehicle; photo ID number; photos; scars and tattoos; SSN; A-number; TECS case number (D, PIA pp. 52–53).
- **Vendor / vehicle:** Booz Allen order 70CTD022FR0000002. Modification P00019 / J&A JA-26-0191 "Advanced Target Development" (posted ~Sept 2, 2026) adds five new tasks under PWS 4.1.10 "Data Science/Machine Learning Engineering" (D, J&A read Oct 26: J&A-26-0191, file 5.1.1-P00019_JA-26-0191_70CTD022FR0000002). Reporting (R, GovTribe via CGA) described the tasks as ML engineering, cross-dataset analytics, network identification, lead generation and threat prioritization and tied them to the HSI Innovation Lab; the redacted J&A does not show the task names or the Innovation Lab (U). Per the J&A (D): the support is for the Homeland Security Task Force National Coordination Cell under EO 14390 "Combating Cybercrime, Fraud, and Predatory Schemes Against American Citizens," to extract information on scam call-center networks (financial information, leadership, links to corrupt officials, "targeting lists of U.S. victims," recruitment); the order's original goal was "streamlining the ingestion of public, private sector, and authoritative U.S. Government data" for "cross-dataset exploration" to identify networks, generate leads and prioritize threats; basis RFO FAR 8.401(b) / GSAR 538.7104-3(b)(1)(iii), logical follow-on to a competed FSS order; Booz Allen offers proprietary technology at its own investment "unlike the current Government Furnished Equipment-based model," deployable within two weeks; a fragment names the White House National Security Council (context redacted). No voter or election language appears in the readable text (D). 2021 PWS public (D, dhs.gov).
- **PIA / SORN:** DHS/ICE/PIA-055, appendix update Jun 2025 (D); earlier PIA Aug 2024 (D per TIP note). RAVEn SORN U; the PIA lists source-system SORNs (FinCEN .003, FBI-001, DHS/ALL-041, SSA 60-0059) (D).
- **Inbound feeds:** [f12] TECS-flagged people (D). [f30] IRS addresses; IRS-to-ICE address sharing is documented, but no source ties it to RAVEn (R; receiving system unknown). [f31] Medicaid data; reporting ties it to a Palantir tool, possibly ELITE, not RAVEn (R; receiving system unknown). [f32] SSA Master Earnings File, annually (D). [f33] PRAC loan-level data including nationality (D). [f34] FinCEN Bank Secrecy Act reports, daily (D). [f38] possible alerts from TRSS CLEAR-based monitoring; not documented (I). On-demand queries to NCIC and IDENT/HART (D). USDA NFC payroll (ICE employee data) (D).
- **Outbound feeds:** [f37] leads to ICM. [f42] HSI is a founding NFDC partner; flow U. [f51] lead lists drive field interviews (D, ECF 87); whether each contact is logged is U (the Aug 28 memo requires documenting findings in a "Criminal Voter Fraud Initiative Portal"). [f52] voter-fraud reports "for submission to VP Task Force" (HSI report Jun 16, 2026, D, FOIA).
- **Court mentions:** The Oct 24 PCIS note lists RAVEn among systems "named in litigation"; which filing U. CNA v. Mullin ECF 87 describes DHS target lists and iLab enrichment but does not name RAVEn (D).
- **Status since Jan 20, 2025:** Jun 2025 PIA appendix update (D). Sept 2026 P00019 (R). Voter-data PIA gap noted Oct 21 (D).
- **Open questions / records (U):** RAVEn GO usage rules; whether HSI policy now requires logging every contact. Lead Tracking Tool outcomes for cleared people. "Criteria" entries for voter-related contacts. Whether P00019 touches election work (the 2021 PWS already had reusable analytics and private-sector data integration; methodological not operational overlap, per CGA).

### ICE-06 · FALCON
Map flows: none on the map
- **Owner:** ICE (K). **What it holds:** A Palantir-based ICE system (2014 PIA, per Oct 24 procurement note; K, verify). VSPTS data already fed FALCON (same source).
- **Vendor / vehicle:** Palantir (K). **PIA / SORN:** 2014 PIA (K). **Feeds, court, status:** U.
- **Open questions / records (U):** Current status of FALCON; relation to ICM, ELITE, ImmigrationOS; whether it was folded into the Palantir BPA's "legacy migration."

### ICE-07 · HSI Innovation Lab ("iLab") profiles
Map flows: f35, f36, f49
- **Owner:** HSI Innovation Lab (D).
- **What it holds:** "unknown artificial intelligence tools" used to "create a compiled list of individual profiles" from the 48.2M "independent sources" and DOJ's 50.6M voter-roll records (D, CNA order ECF 87 at 2–3). "Secondary enrichment and identification of high-value targets" (R, Biometric Update, which places this in late May 2026; Bates cite not rechecked). HSI broadcast Aug 31, 2026 "50 State Voter Roll Processing" (cited to ECF 50-2; the exhibit text could not be read, so unverified, U).
- **Vendor / vehicle:** U. Booz Allen P00019 adds five Innovation Lab tasks (R; see ICE-05). Sandia "Athena" used on NJ and PA rolls (R, ProPublica).
- **PIA / SORN:** U.
- **Inbound feeds:** [f35] voter rolls from the DHS HQ target-list compilation. **Outbound feeds:** [f36] to ELITE (use U). [f49] California list of more than 20,000 individuals: the complaint says USCIS sent HSI the list and the federal government provided it to California on Oct 13, 2026; DOJ is not named as a recipient, so the "to DOJ" routing is our label (D, US v. California complaint, Oct 15, 2026).
- **Court mentions:** CNA v. Mullin ECF 87; ECF 50-2. US v. California ¶¶33–43. Provenance conflict: the complaint says USCIS used unnamed "third-party software"; the map credits iLab. At the Oct 25 Ninth Circuit argument, DOJ counsel struggled to explain what role an unidentified third party played in analyzing the data (R, Democracy Docket); the court rejected DOJ's request Oct 26 (R, CNN). Treat the origin of the California list as U.
- **Status since Jan 20, 2025:** Aug 31, 2026: DHS "Surge Initiative Guidance" (D, ECF 87 p. 2). The "50 State Voter Roll Processing" broadcast cited to a separate exhibit was not found in ECF 87 or ECF 50-2 (U). Oct 15, 2026 complaint (D).
- **Open questions / records (U):** iLab tool inventory; names and contracts of the AI tools; the provenance of the 48.2M.

### ICE-08 · CBFCC (HSI Cross-Border Financial Crimes Center) election pipeline
Map flows: f40, f41
- **Owner:** HSI (D).
- **What it holds:** The "Election Integrity Investigations" pipeline of Jun 15, 2026: roll acquisition → enrichment → leads → field validation → organizations (D, FOIA). CBFCC "facilitates the referral, coordination, and dissemination" of voter leads; the Identity and Benefit Fraud Unit (IBFU) took over from a "Tiger Team" ~Jul 2025 (D, ECF 46-2 ¶¶9–10).
- **Vendor / vehicle:** U.
- **PIA / SORN:** U.
- **Inbound feeds:** [f40] ~25,000 SAVE-flag leads; a further ~15,000 leads went to HSI's cross-border financial crimes unit (R, ProPublica). **Outbound feeds:** [f41] field validation (D); ECF 87 reports only a plaintiffs' allegation of "at least 148" organizations reviewed (Dkt. 79-2), not a finding.
- **Court mentions:** CNA v. Mullin ECF 46-2 (acting Deputy Assistant Director declaration; name blank); ECF 87.
- **Status since Jan 20, 2025:** Jul 2025 IBFU takeover (D). Mar 2026 ICE–DOJ data-sharing letter lets HSI use rolls for any "appropriate investigation of potential violations of federal election law" (R). Aug 31, 2026 surge (D).
- **Open questions / records (U):** USCIS→CBFCC referral counts and criteria; IBFU referral criteria; the CBFCC's data holdings.

### ICE-09 · ATrac ("Alien Tracker")
Map flows: none on the map
- **Owner:** ICE (R).
- **What it holds:** Geospatial targeting using FBI, ATF, USMS and SSA data (R, NYT via The Independent, Jun 2025); DOL, HHS, HUD and IRS data planned (R, 404 Media, Apr 2025).
- **Vendor / vehicle, PIA / SORN, feeds, court:** U. No voter link shown (U).
- **Status since Jan 20, 2025:** Reported Apr 2025 (R).
- **Open questions / records (U):** PIA, vendor, current data sources.

### ICE-10 · DASS (continuous-monitoring analytics, Thomson Reuters Special Services)
Map flows: f38
- **Owner:** ICE/HSI (D).
- **What it holds:** Continuous monitoring of up to 1M entities, with alerts, risk scoring and graph anomaly detection (R, Biometric Update, Aug 15, 2026, and GovConWire; J&A text not independently retrieved). The procurement text cites voter fraud, immigration fraud and national security (R, 404 Media, Jul 17, 2026).
- **Vendor / vehicle:** BPA 70CMSD26A00000008, $125M, five years through Sept 29, 2031 (R). Sole-source J&A-26-0099 dated Jul 14, 2026 (number and date from the SAM notice, not from press), withdrawn Aug 12 (R), then competed with reportedly one bid (R, GovConWire citing OrangeSlices). SAM notice 68e3b2668da549dea1b90593cb5a390b (D). Sept 29, 2026 TRSS orders: 70CMSD26FC0000057 $1.54M; …0060 $2.69M (SEVP); …0061 $2.47M; …0069 $503K, about $7.21M (aggregator values, not reconciled). Control: TRSS LEIDS ICE 2021, ~$25.2M. Likely the same $125M "CLEAR 'voter fraud'" contract in the report timeline (Jul 17; ICE said it would compete the requirement, reported Aug 15–18, with a solicitation forecast of Aug 24) (I).
- **PIA / SORN:** U.
- **Inbound feeds:** Commercial and public data via TRSS CLEAR (I). **Outbound feeds:** [f38] possible alerts and risk scores into HSI lead systems; not documented, and Biometric Update says the TRSS data flow into ICE's Palantir systems is not established (I).
- **Court mentions:** None found.
- **Status since Jan 20, 2025:** Jul 14, 2026 J&A; Aug 12 withdrawn; Sept 2026 BPA and orders (R).
- **Open questions / records (U):** Signed BPA, parent identifier, PWS, ordering guide; reconcile with the September calls. Do not equate ceiling or capacity with spending or enrollment.

### ICE-11 · VSPTS (Visa Security Program Tracking System)
Map flows: none on the map
- **Owner:** ICE/HSI (D).
- **What it holds:** Visa-security vetting data shared among State, ICE and CBP (R).
- **Vendor / vehicle:** Incumbent Steampunk. Sole-source bridge 70CTD026FR0000055, Sept 23, 2026, up to two years, ~$1.65M, to keep it running "during the transition" to Palantir Foundry; J&A dated Oct 7; the competed July 2026 recompete was cancelled because leadership wanted a "more advanced, modernized solution" (R, Biometric Update, Oct 9).
- **PIA / SORN:** U. Data already fed FALCON (K, 2014 PIA).
- **J&A read Oct 26 (D, J&A-26-0230, ICE OAQ for the HSI Visa Security Program):** Interim sole-source order to Steampunk under CIO-SP3 SB IDIQ 75N98120D00251, FFP, FY2026 HSI base funds, logical-follow-on exception (FAR 16.507-6). Scope: O&M, enhancements, AWS GovCloud hosting, Tier 2/3 help desk. VSPTS "store[s], track[s], and manage[s] visa vetting and screening operations" and supports "automated pre-adjudicated screening and vetting of individuals applying for U.S. visas." Key text: the competitive recompete planned for July 2026 "was canceled in favor of a more advanced, modernized solution. ICE leadership intends to transition VSPTS operations to Palantir's Foundry platform," and during the interim "the new VSPTS applications are expected to be developed and deployed on the Foundry platform." Market research is testing whether SWIFT IDIQ PaaS contractors can "migrate the VSPTS application to the Foundry Platform." The text does not say how Palantir or Foundry was chosen (U).
- **Feeds, court:** U.
- **Status since Jan 20, 2025:** Sept 23 bridge; Oct 7 J&A (R); J&A text now D.
- **Open questions / records (U):** How Foundry was chosen; the migration contract (SWIFT) and its date; the Foundry order or BPA call that hosts VSPTS (DHS-02); whether State and CBP visa data feeds change.

### ICE-12 · Mobile Fortify (NEC) and "Mobile Identify"
Map flows: f39, f48
- **Owner:** ICE and CBP (R).
- **What it holds:** A field face-scan app that queries IDENT (270M+ records), CBP's Traveler Verification Service, State's visa and passport photo database, NCIC, Nlets, TECS and SEACATS (R: 404 Media, WaPo, NPR, Wired, 2025–26). Photos are kept 15 years "regardless of immigration or citizenship status"; a person cannot refuse (R, DHS document, 404 Media Oct 31, 2025). A Privacy Threshold Analysis (PTA) exists, approved May 12, 2025 and expiring May 12, 2028 (D, the PTA as published by Biometric Update, Dec 2025). No Mobile Fortify-specific PIA or SORN; the PTA relies on existing PIAs for ICE's EID and CBP's ATS (D).
- **Vendor / vehicle:** NEC, named in the DHS 2025 AI Use Case Inventory (R). No separate award identified; likely rides on the NEC enterprise license, $23.85M, Sept 30, 2024 (I; see DHS-01). CBP's Mobile Identify for local police: reported Nov 4, 2025 as publicly released and Dec 5, 2025 as removed from Google Play (R; these are report dates).
- **PIA / SORN:** PTA only; no Mobile Fortify-specific PIA or SORN (D). "Mobile Query" appears in earlier working notes but in no primary record found; it may be another name (U).
- **Inbound feeds:** [f48] The PTA lists ATS/TVS, a biometric gallery and IDENT (D); queries to State photos, TECS, NCIC and Nlets are reported but not confirmed in a primary source (R). **Outbound feeds:** [f39] captures retained; receiving system U (ATS per CBP-02, source U).
- **Court mentions:** None found. ICE told lawmakers that Mobile Fortify results are "definitive" and should be trusted over a birth certificate (R, 404 Media, Jan 19, 2026).
- **Status since Jan 20, 2025:** First reported Jun 2025 (R); Oct 31, 2025 DHS document (R).
- **Open questions / records (U):** The Mobile Fortify PTA/PIA; the list of galleries queried; the task order or modification adding mobile capability; whether passport photos of U.S. citizens are in the queried gallery.

### ICE-13 · Field capture peripherals: body cameras (Axon Evidence.com) and BITMAP devices (Parsons)
Map flows: f39
- **Owner:** ICE and USCIS (D).
- **What it holds:** Body-worn camera footage in Axon's cloud (Evidence.com) (R/baseline). ICE expected every field officer equipped by end Aug 2026; policy calls for expedited release of footage after a serious injury or death in custody when judged in the "best interests of the agency" (R, AP, Aug 8, 2026). BITMAP mobile biometric collection devices for ICE-HSI (D).
- **Vendor / vehicle:** Axon: 70CMSW26FR0000046 $13.1M and …0045 $17.8M (Jul 17 and 20, 2026); PCI Guidehouse JV 70CMSW26C00000014 $1.8M body-camera PMO (Sept 16); 70CMSW25FR0000020 $67,500 Evidence.com engineering (Mar 11, 2025); USCIS 70SBUR26F00000181 $159,675 (action date Aug 26, 2026). Parsons: 70CMSD26P00000133 $40K and 70CMSD26P00000097 $99K, not competed (Sept 25 and 30, 2026) (D).
- **PIA / SORN:** U (ICE-008 SAS SORN covers incidental recordings, see ICE-01).
- **Feeds:** [f39] receiving system for captures U (IDENT/HART?). Link from Axon to any DHS analytics platform U.
- **Court mentions:** None found.
- **Status since Jan 20, 2025:** Mar 2025 Evidence.com work; Jul–Sept 2026 purchases (D).
- **Open questions / records (U):** Retention; any face-search or AI transcription on footage; BITMAP device specs and where captures go.

---

# PART C · Commercial identity, OSINT and location tools (vendor products, neutral infrastructure)

### COM-01 · Clearview AI (face search)
Map flows: none on the map
- **Owner/user:** ICE/HSI; CBP; FBI; USMS; IRS; DOJ Criminal Division (D, USAspending).
- **What it holds:** A database of "50+ billion" (HSI) or "60+ billion" (CBP SOW) scraped facial images (R/D vendor-described).
- **Vendor / vehicle:** ICE/HSI 70CMSD25P00000111: $3.75M awarded Sept 5, 2025 plus option 1 exercised Sept 1, 2026 $3.94M = $7.69M; one offer, "only one source"; runs to Sept 4, 2027 (D). Reporting says $9.2M signed Sept 9, 2025 (R; unreconciled). Stated purpose "child sexual exploitation cases and assaults against law enforcement officers" (D). Earlier ICE buys $224K (2020), $2.29M (2021), $1.10M (2024). CBP: NTC $225K (Feb 10, 2026), Border Patrol licenses Jun 2025 (D); a Jul 2026 purchase is not sourced (U). FBI: the Clearview PO found is 15F06723P0001356, signed Jan 26, 2023, running to Jan 2026; no Jan 2026 award of $150K was found (U); USMS (Mar 2026); IRS (Mar 2026); DOJ Criminal Division "AI Federal Investigator Tool" $31.5K (signed Sept 24, 2026; performance starts Sept 30) (D). CBP NTC $225K (Feb 10, 2026): FedScoop confirms the 15-license deal but not the amount or day (U).
- **PIA / SORN:** ICE FRS PIA is referenced by RAVEn HORUS (D). Others U.
- **Inbound / outbound feeds:** Probe photos in; candidate matches out (I). Whether run on protest footage is U.
- **Court mentions:** None found. The NTC Counter Network Division was reported to have run searches on journalists, congressional members and staff, and U.S. citizens' groups (R, Yahoo News, Dec 2021–Jan 2022). CBP's Feb 2026 Clearview contract (15 NTC licenses) cites "counter-network analysis" (R, FedScoop, Feb 11, 2026); this is CBP's contract, not ICE's.
- **Status since Jan 20, 2025:** Sept 2025 award, largest yet (about 3.4× the 2021 buy); Feb 2026 CBP NTC; Sept 2026 option (U: the $3.94M option amount and Sept 1 date were not shown in the record reached).
- **Justification read Oct 26 (D, J&A-25-0183, FAR 6.302-1 only one responsible source, new FFP purchase order for the HSI Innovation Lab):** Notice of intent posted Aug 6, 2025. HSI has used Clearview "since June 2019." The vendor is described as "sole provider" of facial search of public online imagery with source attribution, compliance and audit tools, gallery enrollment and a "unified platform," over "50+ billion facial images." An authorized reseller exists and a NASA SEWP V RFI drew a market-research quote, but the J&A still concludes sole source; HSI later reduced its license count; the CO will request invoices for Clearview sales to other agencies to check price. Stated mission text is largely redacted. The file does not show the contract number; matching it to 70CMSD25P00000111 rests on timing, Sept 5, 2025 award (I). It ties Clearview to the Innovation Lab (ICE-07) (D). No voter or election language in the readable text (D).
- **Open questions / records (U):** CBP SOW and CBP justification; NTC Counter Network Division election tasking; the redacted purpose and license counts; the reseller quote.

### COM-02 · LexisNexis (RELX) and Thomson Reuters CLEAR (commercial people-search)
Map flows: f9
- **User:** USCIS, ICE/HSI, FDNS (D).
- **What it holds:** Address history, relatives, utilities and other commercial identity data (K). The LexisNexis requirement describes Palantir/PenLink interfaces and batch identity queries (R).
- **Vendor / vehicle:** RELX 70SBUR25F00000065, $5.4M (seven obligating actions totaling $5,434,485, Mar 2025–Sept 2026; USAspending), Mar 2025–Mar 2027 "law enforcement research subscriptions" (D). ICE LEIDS 70CMSD26C00000009, ~Aug 31/Sept 1, 2026 (D lead; award not read). TRSS CLEAR via DASS and the FDNS vetting solicitation (see ICE-10, USC-06). Bridge notice 192126FLMURQ0071.
- **PIA / SORN:** U.
- **Feeds:** [f9] commercial databases used to clear names (D, CNA order).
- **Court mentions:** CNA order notes commercial databases are "typically used for targeted advertising" and include addresses, geolocation, demographics, family structure and vehicle ownership (D).
- **Status since Jan 20, 2025:** Mar 2025 USCIS buy; Aug–Sept 2026 ICE award (D lead).
- **Open questions / records (U):** Executed award and actual interface records. General API requirements do not establish voter ingestion or ELITE use.

### COM-03 · OSINT and location tools (Penlink Tangles/Webloc, ShadowDragon, Fivecast, Babel Street, Zignal)
Map flows: none on the map
- **User:** ICE Intelligence, ICE Homeland Security Task Force, USCIS FDNS (D).
- **What it holds:** Social-media and location analytics. Webloc is location data (K).
- **Vendor / vehicle:** Pen-Link 70CMSD26FR0000187 $1.87M; …0185 $1.63M; …0181 $1.63M (Sept 25, 2026). ShadowDragon (via ETS) 70CMSD26FR0000166 $132,931 (Sept 21). Fivecast (via ETS) 70CMSD26FR0000093 $777,777 (Sept 15). Babel Street (via Flywheel Data) 70CTD026FR0000025 $10,300,000, 25 Insights licenses, "location and identity" APIs (May 20, 2026). Zignal (Sept 2025). A USCIS FDNS social-media vetting pilot is reported as a $2.8M noncompetitive purchase order to Thomson Reuters Special Services, with CLEAR Risk Inform, CLEAR Batch and Fivecast MATRIX meeting the minimum requirements (R, ExecutiveBiz, Oct 8, 2026, citing G2Xchange); the SAM notice and Amendment 0001 attachment, read Oct 27, confirm the intent to award noncompetitively to TRSS and the required capabilities (D; see USC-06).
- **PIA / SORN:** ICE IIRS (ICE-006) SORN modified Jul 2025, FR 2025-13613 (D). Others U.
- **Feeds, court:** U.
- **Status since Jan 20, 2025:** Sept 2026 cluster is mostly fiscal-year-end (competing explanation).
- **Open questions / records (U):** Justifications and SOWs; data sources; whether any is tasked to election-related networks.


---

# PART D · CBP

### CBP-01 · TECS (subject records and lookouts)
Map flows: f11, f12, f13
- **Owner:** CBP, used DHS-wide (D).
- **What it holds:** Subject records that act as lookouts and "follow a person." TECS records "can be used against [an individual] in any interaction they may have with the federal government, such as crossing the border during travel or seeking a benefit"; USCIS created TECS records for citizens (D, ECF 87 reciting the record). RAVEn GO field records carry a TECS case number (D).
- **Vendor / vehicle:** U.
- **PIA / SORN:** Not located (U). K lead: DHS/CBP-011 TECS SORN; verify.
- **Inbound feeds:** [f11] FDNS-created records (D). ICM lookouts via the Interface Hub (R). The CNA order says USCIS "generates TECS records for individuals identified through the Voter Eligibility Matching Policy" and that USCIS "concedes that errors will result" (D, ECF 87, citing the government declaration ECF 46-1 ¶8). The earlier quoted "directive" wording is unverified (U).
- **Outbound feeds:** [f12] flagged people reach HSI (D). [f13] PCIS input (D). Border stops and enhanced screening: alleged in a Hilton motion (R, Neoteo; allegations, disputed by DHS, not findings).
- **Court mentions:** CNA v. Mullin ECF 46 (nonfinal "starting point" argument), ECF 87 (order prongs (a) and (b)); Hilton ECF 117 (D/R); Noem v. Vasquez Perdomo, 25A169 (Sept 8, 2025; Kavanaugh concurrence on stops) (D).
- **Status since Jan 20, 2025:** TECS record creation for voter matching, by USCIS per the CNA order (D); Oct 21, 2026 PI order ¶1(b) bars field operations based wholly on TECS records generated from the Voter Eligibility Matching Policy, against persons the enjoined parties believe are U.S. citizens, in nine states (CA, CT, GA, MO, NV, NY, PA, WA, WI) (D). The order says "USCIS generates" those records; it does not name FDNS.
- **Open questions / records (U):** Do flags close or annotate after a person is cleared? TECS disposition codes; whether a "voter fraud organization" checkbox or similar tag exists in TECS or RAVEn GO.

### CBP-02 · ATS (Automated Targeting System)
Map flows: f14
- **Owner:** CBP (D).
- **What it holds:** Risk targeting (D, map). Mobile Fortify photos kept 15 years: reported as held by ATS (CBP DSAI forecast); the underlying source for ATS as the repository is not recorded (U).
- **Vendor / vehicle:** U. CBP's entity-resolution tool is Tamr, 70B06C22C00000067, $1.6M, Sept 2022 (D; relation to ATS U).
- **PIA / SORN:** Not located (U).
- **Inbound feeds:** U. **Outbound feeds:** [f14] PCIS input (D, PCIS PIA).
- **Court mentions:** None found.
- **Status since Jan 20, 2025:** U.
- **Open questions / records (U):** Source for ATS storing Mobile Fortify photos; ATS PIA/SORN currency; DSAI SOW (CBP-05).

### CBP-03 · TVS (Traveler Verification Service)
Map flows: f48 (via Mobile Fortify)
- **Owner:** CBP (D).
- **What it holds:** Face galleries built from DHS holdings, including photos from passport and visa records shared by State (K, DHS/CBP/PIA-056, 2018; verify). Mobile Fortify queries it (R).
- **Vendor / vehicle, PIA / SORN beyond PIA-056, feeds, court:** U.
- **Status since Jan 20, 2025:** U.
- **Open questions / records (U):** Current PIA; what U.S.-citizen live captures are retained, and whether Mobile Fortify queries them.

### CBP-04 · Vehicle Biometric Capability Evaluation
Map flows: none on the map
- **Owner:** CBP (R). **What it holds:** A vehicle-based biometrics evaluation planned for FY2026 (R, GovCIO, Sept 16, 2025); CBP also said it would use AI to flag unusual travel activity ahead of the World Cup (R, MeriTalk, May 28, 2026).
- **Vendor, PIA/SORN, feeds, court, status:** U.
- **Open questions / records (U):** Primary source; vendor; retention; whether it leads to CBP-05.

### CBP-05 · DSAI (Digital Solutions and Application Innovation) BPA forecast
Map flows: none on the map
- **Owner:** CBP (R).
- **What it holds:** Application development for all CBP operational and support offices, explicitly including "integration of biometrics technology into new and existing applications," AI/ML, mobile and web apps, analytics, chatbots, IoT, gateways, blockchain (R, Biometric Update, Oct 26, 2026).
- **Vendor / vehicle:** Forecast: $20–50M competitive firm-fixed-price BPA, small-business set-aside; solicitation expected Nov 16, award Dec 30, performance to Mar 14, 2029. Incumbent Ellumen (DTSS order Sept 2020 ~$21.8M; PAMS order Sept 2023 ~$7.3M; July 2024 bridge ~$14.4M) (R). A recompete, first forecast Dec 2024 (R).
- **PIA / SORN:** N/A. **Feeds:** Which systems receive biometrics is not stated (U).
- **Court mentions:** None.
- **Status since Jan 20, 2025:** Slipped solicitation date (R). Ordinary explanation strong (I).
- **Open questions / records (U):** Pull the SOW when the solicitation posts (~Nov 16). Check whether ATS, TECS, TVS, HART or Mobile Fortify are named, and whether ICE/HSI sharing or Enterprise Lakehouse integration is in scope.

---

# PART E · DHS-wide platforms and vehicles

### DHS-01 · HART / IDENT (OBIM) and the NEC enterprise facial matcher
Map flows: f15, f39
- **Owner:** DHS Office of Biometric Identity Management (OBIM) (D). Reports to the DHS CIO since Aug 2025 after a White House Homeland Security Council review began May 2025; DOGE "extended its operations to OBIM," though two sources said it got no direct system access (R, FedScoop May 20 and Aug 14, 2025).
- **What it holds:** "More than 300 million profiles" of faces, fingerprints and irises; IDENT handles nearly half a million queries a day (R, FedScoop, 2025). HART is the delayed replacement; a White House spokesperson described the goal as to "accelerate the delivery of HART" and a "unified biometric experience for DHS" (R, FedScoop, Aug 14, 2025).
- **Vendor / vehicle:** NEC National Security Systems: sole-source maintenance and support for DHS's perpetual NEC AIM facial-matching licenses, $23.85M (Sept 30, 2024; three years to Sept 29, 2027), following $7.95M (Sept 30, 2023) (D). The DHS Palantir LSJ requires "integration with biometric and identity management systems, such as the [redacted]" (D; likely HART/IDENT, I).
- **PIA / SORN:** DHS/OBIM/PIA-001 (IDENT); HART has a 2020 PIA and an Aug 2024 update, which says a further PIA will issue before HART becomes operational (D, DHS/OBIM/PIA-004(a)); the Jun 2025 RAVEn PIA appendix was not re-read (U). SORN DHS/ALL-041 External Biometric Records, 83 FR 17829 (Apr 24, 2018) (D).
- **Inbound feeds:** [f39] Mobile Fortify and body-cam captures; receiving system unknown (U). **Outbound feeds:** [f15] to PCIS (D). RAVEn on-demand queries (D). Mobile Fortify queries IDENT (R).
- **Court mentions:** None found.
- **Status since Jan 20, 2025:** May 2025 HSC review; Aug 2025 reporting change (R).
- **Open questions / records (U):** HSC review output (May–Aug 2025); DOGE access logs or agreements for OBIM; HART PIA.

### DHS-02 · DHS-wide Palantir BPA 70RTAC26A00000001 (LSJ FY25-00257)
Map flows: f36, f37 (platform for ICM/ELITE); CIS-01
- **Owner:** DHS OCIO (D).
- **What it holds:** BPA for "department-wide data integration and data analysis solution" (D, LSJ). Capabilities include "deconfliction of data to ensure each subject has one consolidated record" (D; "golden record" is master-data-management vocabulary for the same idea). Requirements: "Unified Platform for Case Management and Analytics … will eliminate data silos" (echoes EO 14243); "seamless data sharing and integration across all DHS components, including ICE, CBP, TSA, FEMA and [redacted]"; "unified search capabilities across multiple internal and external systems"; migration of "existing investigative data from legacy systems"; interfaces "within external agencies" already built (D). Whether voter data enters any DHS Palantir instance is U.
- **Vendor / vehicle:** Palantir. BPA awarded Feb 12, 2026, $1B ceiling to Feb 2031, one offer (D, USAspending). LSJ FY25-00257: COR certification Sept 4, 2025, posted May 14, 2026; "covers all BPA orders" (D). ICE required "complete delivery by September 2026" (D). Consolidates existing DHS Palantir licenses as maintenance agreements expire (D). Orders: CISA 70RCSJ26FC0000028 $32,106,350 (CIS-01); ICM 70CTD026FC0000018; ERO 70CTD026FC0000012; Secret Service "data modeling" $18.7M (Mar 18, 2026); USCIS VOWS 70SBUR26F00000003/-26/-55 ~$100K each (D). FY-end wave at IRS (four), State, HHS, HUD, Commerce (D); competing explanation for timing.
- **PIA / SORN:** Not a system. Underlying instances carry their own.
- **Inbound / outbound feeds:** "daily data export to the analytical system" with a redacted partner (D, LSJ). Everything else U.
- **Court mentions:** None names the BPA. Palantir statement (Courtney Bowman, mid-2025): "We are not building, we have not been asked to build, and we're not in contract to build any kind of federal master list or master database across different agencies" (R, as quoted in The Epoch Times; the Palantir blog text was not re-read).
- **Status since Jan 20, 2025:** Feb 12, 2026 award; May 14, 2026 LSJ posted; Sept 2026 orders. Palantir Q3 earnings reported by calendar sites for Mon Nov 2, 2026, the day before the election (R; no company announcement found; time unconfirmed). Palantir's CTO was reported in June 2026 as a CISA director contender; the White House said "not accurate" (R).
- **Posting lag (I):** the LSJ cites FAR 8.405-6(a)(2)(i)(B) for posting; the companion Carahsoft SSJ states a 14-day-after-award posting rule, and GSAR 538.7104-3(b)(3) (GSA class deviation RGO-2026-01, Jan 15, 2026) uses 14 days (30 for urgent awards) (D, fetch summary of RGO text). BPA awarded Feb 12, 2026 (USAspending) but LSJ posted May 14, 2026, about 91 days later. FAR 8.405-6(a)(2)(i) itself sets a 14-day posting clock after establishing a BPA over the simplified acquisition threshold, and GSAR RGO-2026-01 applies to GSA contracting activities only, so a separate BPA clock is a weak explanation. Remaining explanations: BPA award date differs from the date the justification attached; administrative lag; delayed posting by choice. Unresolved.
- **Open questions / records (U):** Unredacted LSJ (names redacted components, CISA?); order-level files; ATO boundaries; whether CISA's instance connects to others.

### DHS-03 · DHS-wide Databricks BPA 70RTAC26A00000010 ("enterprise data lakehouse")
Map flows: f20 (platform for USC-04); CIS-02
- **Owner:** DHS OCIO (D).
- **What it holds:** Single-award DHS-wide BPA for Databricks products and services (D); keeps DHS's "enterprise data lakehouse environment and intelligence platform built on Databricks" running, naming USCIS, CBP, FEMA, ICE and the Coast Guard, not CISA (R, Washington Technology, Mar 20, 2026).
- **Vendor / vehicle:** Databricks Federal LLC. BPA Jul 17, 2026–Jul 16, 2031, 2 offers, $1B ceiling (D). Orders: 70RTAC26FC0000024 $57.0M (Jul 31, 2026–Jul 30, 2027); 70RTAC26FC0000046 $1.49M (Sept 29, 2026); CISA 70RCSJ26FC0000030 $4.95M (Sept 30, 2026; "other statutory authority") (D).
- **PIA / SORN:** Not a system; U.
- **Feeds, court:** None names the BPA (U).
- **Status since Jan 20, 2025:** Jul 17, 2026 award per OrangeSlices; HigherGov shows a Jul 16 start date, so the award date is U (D). The Mar 20 article predates the award, so a precursor vehicle may exist (U).
- **Open questions / records (U):** The precursor arrangement; justification for single award; ICE's Enterprise Lakehouse relationship (ICE-02).

### DHS-04 · DHS-wide Carahsoft BPA 70RTAC26A00000011 (SSJ FY26-0119)
Map flows: none; CIS-04
- **Owner:** DHS (ITAC) (D).
- **What it holds:** A ~$2.66B reseller BPA, $2,657,393,210, signed Jul 15, 2026, period Jul 20, 2026 to Jul 19, 2031 (D, USAspending), decentralized ordering; stated purposes include data analytics, cybersecurity, collaboration, and identity and access management (R, GovConWire; exact SSJ wording not re-read) (SSJ file dated Oct 2026; posting date not shown in the SSJ, D). OEM list (about 70+) reportedly includes Socure, Lucid, AvePoint, Cellebrite, Recorded Future, Hypori, Okta, SailPoint, Radiant Logic, Cloudera, Confluent, VAST Data, Elasticsearch, Splunk, ServiceNow, ThreatConnect, Qlik, Box, Mattermost (names not re-verified against the SSJ pages; U).
- **Vendor / vehicle:** Carahsoft. "All Brand Name requirements will be justified at the order level" (reported from the SSJ; exact text not independently re-read, U); order-level brand-name justification for CISA's Socure order not found (U).
- **PIA / SORN, feeds, court:** N/A or U.
- **Status since Jan 20, 2025:** SSJ posted Oct 20, 2026 (D); GovConWire reported it in Oct 2026 and gives a ceiling of about $2.7B (R). FedScoop says the period runs to "July 2031"; the SSJ itself gives no period dates or value, which come from other documents.
- **What the OEM list is (D):** Not a roster of everything Carahsoft sells. The SSJ says DHS "tailored the original requirement to only include OEMs that are solely distributed by Carahsoft" (§8) and that OEMs "rely exclusively on Carahsoft" (§6). The SSJ says the full scope "will include but not be limited to" the listed vendors; DHS may add vendors later "if Carahsoft is the exclusive GSA MAS holder" for them, and on/off-boarding is allowed. No separate roster of exclusives exists in the project. Palantir and Databricks do not appear in the OEM names that could be extracted from the SSJ text, which is incomplete (U); each has its own DHS-wide BPA (DHS-02, DHS-03) and Databricks is bought direct, so they likely fail the exclusivity test (I); absence is not evidence about anything else. Data/identity-relevant names on the list: Socure, Radiant Logic, Cloudera, Confluent, VAST Data, Elasticsearch, Cribl, Splunk, Qlik, Cellebrite, Recorded Future, Hypori (D; OCR column order is scrambled, so check pairings against the PDF).
- **Posting lag (I):** SSJ §9 says DHS will post "within 14 days after award"; the BPA was signed Jul 15, 2026 (period began Jul 20, D, USAspending) and the SSJ was posted Oct 20, 2026 (about 97 days after signing). The award date itself is not stated in the SSJ (U). Same open question as DHS-02.
- **Open questions / records (U):** Order-level justification for 70RCSJ26FC0000042 (it exceeds the simplified acquisition threshold); the Carahsoft-held OEM roster by order.

### DHS-05 · HSIN (Homeland Security Information Network)
Map flows: none on the map
- **Owner:** DHS (D).
- **What it holds:** Reported to support World Cup and America250 security coordination (R, Nextgov, Jul 2026, citing Sen. Warner; House testimony Feb 24, 2026, Miami fusion center on sharing via HSIN). Hackers breached "HSIN servers and a SharePoint system used for collaboration" reportedly in late May to early June 2026; DHS called it "a specific, unclassified legacy information sharing environment" (R, Nextgov, Jun 30, 2026).
- **Vendor / vehicle, PIA/SORN, court:** U. See CIS-09 for HSIN-CI.
- **Status since Jan 20, 2025:** 2026 breach (R). (I) A plausible operational reason for a new Teams-based exchange in Sept; no source makes the link.
- **Open questions / records (U):** Breach scope; whether the CISA exchange (CIS-05) replaces HSIN functions for election offices.

### DHS-06 · DHS HQ election team "target-list compilation"
Map flows: f5, f6, f7, f27, f35, f55
- **Owner:** DHS compiles the target list (D, CNA order ECF 87); the "headquarters election team" attribution is the map's label (I; "Team America" appointees label is from the map, source U).
- **What it holds:** Compiles target lists from DOJ's voter rolls (50.6M records) and 48.2M "independent sources" of questionable provenance, and gives the list to USCIS, which the order glosses as FDNS personnel (D, CNA order ECF 87). Not a standalone system; a function and a data-assembly step.
- **Vendor / vehicle, PIA/SORN:** U.
- **Inbound feeds:** [f5] DOJ rolls (D; OLC opinion May 12, 2026: "no impediment" to sharing with HSI). [f6] 48.2M records (D). [f27] SSA DOGE file of ~1,000 people (D, Jan 16, 2026 DOJ correction filing, per Nextgov/The Register; sent to DOGE with copies to DHS and a Labor DOGE associate; nothing ties it to target-list compilation, I). [f55] State passport data under new routine use (w) from Nov 23, 2026; DHS is not named in it (D, future).
- **Outbound feeds:** [f7] to FDNS; [f35] voter rolls to iLab (the CNA order confirms DHS "enriches" data through a system called iLab, D; the name "50 State Voter Roll Processing" is cited to a separate exhibit, U).
- **Court mentions:** CNA v. Mullin ECF 87, 50-2.
- **Status since Jan 20, 2025:** EO 14248 (Mar 25, 2025) predicate; Aug 31, 2026 surge (D).
- **Open questions / records (U):** The source and provenance of the 48.2M; the team's charter; where the compiled lists are stored.

---

# PART F · CISA

Funding note (corrected Oct 25): every CISA award checked lists funding office "Off of the Dir CISA," its default code; it is not a sign of front-office control (D). Year-end spending (Sept 25–30) is the leading competing explanation for the September cluster. These are CISA's first Palantir and first Databricks awards in USAspending 2016–2026 (D). Map card: "CISA · no documented data flow in (U)."

### CIS-01 · CISA Palantir SaaS (70RCSJ26FC0000028)
Map flows: none documented
- **Owner:** CISA Office of the Director funds (D).
- **What it holds:** "Procure Palantir license for software as a service" (D, award text). Use case unstated (U). SiliconANGLE (Feb 19, 2026, citing Wired) says CISA, CBP, ICE and FEMA "will be able to access Palantir services" under the DHS-wide deal, for "investigative case management, threat identification, logistics coordination and operational planning" (R); these are DHS-wide uses, not CISA-specific ones. Possibly CADS-related (K/U); no award is labeled CADS. CADS itself (FY2027 Congressional Justification, read Oct 26, D): "Cyber Analytics and Data System," a Level 1 IT investment, $145.5M in the FY2026 annualized CR and $65.8M in the FY2027 request; a "system-of-systems" for cyber data ingestion, analytics and "information sharing" with partners; FY2025 work integrated datasets into the Cloud Log Aggregation Warehouse (CLAW) and "operationalized unified workflows"; FY2026 plans "modernizing the environment with Data Lakehouse technologies" and integrating "Federal and Critical Infrastructure network visibility" data. It describes network and cloud telemetry, not voter or citizen records (D). Whether the Palantir and Databricks orders sit inside CADS is U.
- **Vendor / vehicle:** Palantir, $32,106,350, Sept 29, 2026–Sept 29, 2027, under BPA 70RTAC26A00000001; fair opportunity "ONLY ONE SOURCE – OTHER"; Clinger-Cohen planning Yes; P00001 only corrects the period of performance (D). Covered by the BPA LSJ; no order-level justification posted (I).
- **PIA / SORN:** None found (watch for any new CISA SORN or PIA, or a national-security-system designation).
- **Feeds:** None documented either way (U).
- **Court mentions:** None.
- **Status since Jan 20, 2025:** Sept 29, 2026 award. Program activity (File C) not yet posted; recheck in December (reminder set for Dec 15, 2026) (D).
- **Open questions / records (U):** SOW; File C program activity; whether TRX, Palantir and Databricks share one ATO/authorization boundary; Palantir's Nov 2 earnings and 10-Q language.

### CIS-02 · CISA Databricks PaaS (70RCSJ26FC0000030)
Map flows: none documented
- **Owner:** CISA (D).
- **What it holds:** "Databricks platform as a service subscription" (D). CISA is buying into the department's existing lakehouse platform (I).
- **Vendor / vehicle:** Databricks Federal LLC, ~$4.95M, Sept 30, 2026–Sept 29, 2027, under DHS-03; "other statutory authority" (D).
- **PIA / SORN, feeds, court:** U.
- **Status since Jan 20, 2025:** First CISA Databricks award (D).
- **Open questions / records (U):** SOW; data sources; shared tenant with USCIS's lake?

### CIS-03 · CISA Unified Data Platform and Integration Support (SiloSmashers, 70RCSJ26FC0000039)
Map flows: none documented
- **Owner:** CISA (D).
- **What it holds:** "CISA Unified Data Platform and Integration Support Services" (D). Possibly the integration layer for the Palantir and Databricks licenses; this rests only on the title and award timing (I).
- **Vendor / vehicle:** SiloSmashers, $3,581,901, signed Sept 29–30, 2026 (the FY26 order number settles the year; the 2025 date was the parent BPA) (D). Parent: Digital Transformation Support Services (DTSS), a multiple-award vehicle with four separate BPAs, one per holder: 70RCSJ25A00000024 AttainX, …25 Electrosoft, …26 SiloSmashers, …27 SOFITC3 (R, OrangeSlices); $500M is the base-and-all-options value (ExecutiveBiz gave $200M as an estimate), awarded around Sept 30, 2025, including "enterprise data management" (R). This order sits under the SiloSmashers BPA (…26).
- **PIA / SORN, feeds, court:** U.
- **Status since Jan 20, 2025:** Sept 2026 order (D).
- **Open questions / records (U):** SOW; ATO/system boundary documents for the "Unified Data Platform."

### CIS-04 · CISA Socure / Lucid / AvePoint licenses (70RCSJ26FC0000042)
Map flows: none documented
- **Owner:** CISA (D).
- **What it holds:** Licenses for an identity-verification vendor (Socure), diagramming (Lucid) and cloud-collaboration (AvePoint) tools (D). CISA's use is unexplained (U). Burris (Socure, VP and Head of Public Sector Strategy) testified to the House Oversight Government Operations Subcommittee Jul 15, 2026 (hearing "Emerging Fraud Threats and the Evolving Fraud Landscape," Serial 119-70; full print read Oct 26): his written statement says identity "should be treated as national infrastructure," urges evaluating identity "across the full lifecycle of an account, continuously and in real time," and asks Congress to "make permanent and expand the data-sharing authorities" (Do Not Pay is discussed at pp. 8–9); cites Socure's FAFSA screening for the Department of Education (more than $1B in a single cycle; legitimate applicants pass automatically at "a rate above 92 percent," Education's estimates); he was Chief of Staff in the White House Office of the Federal CIO across two administrations (D, written statement; earlier quotes in this entry were not in it and have been removed). No voter or citizenship mention in the testimony (D).
- **Vendor / vehicle:** $385,670, Sept 29, 2026, under Carahsoft BPA 70RTAC26A00000011 (DHS-04). Order-level brand-name justification not found (U).
- **PIA / SORN, feeds, court:** U.
- **Status since Jan 20, 2025:** Sept 2026 award. Socure also won Login.gov identity proofing (TRE-04).
- **Open questions / records (U):** Order-level justification; SOW; what Socure is used for at CISA.

### CIS-05 · FusionAware TRX "Elections Threats Reporting Exchange" (70RCSJ26FR0000062)
Map flows: none documented
- **Owner:** CISA (D). Nextgov describes the CISA plan as giving all fusion centers and state and local election officials access at no cost (R, paraphrase, not a quote); Nextgov says CISA states the model was used during the 2026 World Cup and does not name the platform. Federal partners, Fusion Centers, Federal Agencies and CISA Central will be actively engaged on the platform for day-to-day communication … The wording "successfully deployed and utilized during FIFA World Cup 2026" is attributed to the Sept 24, 2026 plan in earlier notes but was not found in Nextgov and the plan page was not re-read (U).
- **What it holds:** Incident reporting and intelligence sharing for election offices, built on Teams and Esri. "TRX" is DVG's own product name, not a CISA configuration; the only CISA-specific word is "Elections" (D, DVG pages; correction of the Oct 24 note). The vendor page also lists "statewide warrant operations and enforcement" among uses (D). Who reports, which fields, who can see them: U.
- **Vendor / vehicle:** DVG Interactive (Data Vision Group, LLC), via Carahsoft, NASA SEWP NNG15SC03B; $1,277,200 perpetual license; Sept 30, 2026–Jan 15, 2027; one offer; coded "follow-on action following competitive initial action" with no earlier CISA action found; "posted to SAM: Yes" but no notice found (D). DVG has no other federal prime award found (D).
- **PIA / SORN:** None found (U).
- **Inbound / outbound feeds:** Undocumented. Predecessor: the combined SLTT security-operations-center/ISAC cooperative agreement (MS-ISAC and EI-ISAC) 23CISMSI00003, about $70M federal share, Sept 30, 2023–Sept 29, 2025 (D, HigherGov grant record); no successor found (U).
- **Court mentions:** None.
- **Status since Jan 20, 2025:** Sept 30, 2026 award; term ends Jan 15, 2027 (D, HigherGov). Feb 24, 2026 House testimony describes a Super Bowl-adjacent trafficking-data effort (Santa Clara County: a public-safety mapping tool plus a common chat/file-sharing tool), naming no vendors (D); DVG's listing of Super Bowl and Club World Cup deployments was not confirmed (U); FIFA lineage plausible, undocumented (I).
- **Open questions / records (U):** SOW; users and fields; retention; whether DOJ, HSI or NFDC are users; the partner list; the "competitive initial action"; Teams tenant (GCC-High?).

### CIS-06 · CISA Esri GIS licenses (70RCSJ26FC0000012)
Map flows: none documented
- **Owner:** CISA (D). **What it holds:** GIS licenses; CISA's Gateway (formerly IP Gateway) ran on Esri ArcGIS as of 2016 (R, Route Fifty); the current platform is not confirmed, so the order may be routine (I).
- **Vendor / vehicle:** Esri, $1.01M, Jul 30, 2026; CISA's first real Esri buy (prior: $50K training, 2019) (D). FusionAware runs on Esri (D).
- **PIA/SORN, feeds, court:** U. Nothing public found as of Oct 27, 2026 (U).
- **Open questions / records (U):** SOW.

### CIS-07 · NRMC AI orders (SOFITC3, 70RCSJ26FC0000036 and …0038) and National Risk Register support
Map flows: none documented
- **Owner:** CISA National Risk Management Center (D).
- **What it holds:** "AI Digital Solution Development, Automation, and Infrastructure Support Services," …0036, $5,483,119; "NRMC AI Modernization for Risk Analytics," …0038, $4,585,415 (labor services, PSC DD01) (D). IDA "National Risk Register support," $4.6M (Sept 30) (D). A 2024 NRMC risk-analysis PWS covered the 16 sectors "and one subsector, Elections Systems" (R, OrangeSlices quoting the Feb 2024 sources-sought notice). CISA's strategy has it helping build a White House "National Risk Register" (R, Nextgov Oct 26). "Modernization" suggests upgrading an existing capability, which is thin evidence from a title word (I). Whether AI work runs on the Palantir/Databricks environment: U.
- **Vendor / vehicle:** SOFITC3, LLC (Piscataway, NJ), first calls under DTSS BPA 70RCSJ25A00000027 (Sept 30, 2025–Sept 24, 2030; competed; 37 offers); solicitation 70RCSJ26Q00000057; Sept 30, 2026–Sept 29, 2027 (D).
- **PIA / SORN, feeds, court:** U.
- **Status since Jan 20, 2025:** Sept 2026 orders. NRMC history: 2021–24 "mis/dis/mal-information and communication analytics" requirement, about $14.4M obligated of a $15.56M ceiling (CyberMedia Technologies) (D, HigherGov).
- **Open questions / records (U):** SOWs; the 2021 mis/dis/mal deliverables (relevant to any 2026 "influence" product).

### CIS-08 · CI3 (classified critical-infrastructure briefing channel)
Map flows: none on the map
- **Owner:** CISA (D). **What it holds:** A monthly classified briefing run with ODNI that reaches "more than 70 secure locations nationwide" (R, Nextgov paraphrasing the CISA plan; the plan's fuller wording was not re-read). Full name of CI3 not recorded (U).
- **Vendor, PIA/SORN, feeds, court:** U.
- **Open questions / records (U):** What CI3 stands for; who gets read in; any voter-related content.

### CIS-09 · HSIN-CI / CI-ISE support (70RCSJ26FR0000058)
Map flows: none on the map
- **Owner:** CISA (D). **What it holds:** HSIN-Critical Infrastructure and the CI information-sharing environment; support renewed $1.80M, Sept 30, 2026 (D).
- **Vendor, PIA/SORN, feeds, court:** U. Parent HSIN breached May–Jun 2026 (DHS-05) (R).
- **Open questions / records (U):** Whether the HSIN breach touched HSIN-CI.


### CIS-10 · CISA Stakeholder Engagement Division advisory support (AttainX, 70RCSJ26FR0000055)
Map flows: none on the map
- **Owner:** CISA Stakeholder Engagement Division (SED); awarding office DHS OCPO / 70RCSJ; funding office "Off of the Dir CISA" (D, USAspending page read in browser Oct 26; HigherGov's 70PCS1 was a different field).
- **What it holds:** Not a data system. "Task order for critical infrastructure engagement and advisory support services" for SED: planning, execution, analysis and documentation of engagement, advisory and coordination functions; council advisory and strategic engagement program support; "national-level coordination construct" support; sector risk management engagement support; contract management; "explicitly excluding budget, procurement, or human capital support" (R, HigherGov description; not found in DHS's acquisition forecast text, verification pending). No election, voter or data-platform wording appears in the descriptions checked: HigherGov and DHS APFS forecast 73860 (D/R). Whether it supports the Election Infrastructure Subsector or its coordinating council is U.
- **Vendor / vehicle:** AttainX (small business; also a holder of DTSS BPA 70RCSJ25A00000026, CIS-03). Delivery order under OASIS+ WOSB IDV 47QRCA24DW109, solicitation 70RCSJ26R00000008. No set-aside coded on the order (D, USAspending, read Oct 27). AttainX's recipient profile lists 8(a) participant, economically disadvantaged women-owned, women-owned small, minority-owned and small business (D); that may be what HigherGov's "women-owned" label reflects (I); "Full and Open Competition After Exclusion of Sources," multiple-award fair opportunity, 18 offers, performance-based, no subcontracts. $7.5M obligated, up to $15,058,542; Sept 30, 2026–Sept 29, 2027, potential end Sept 29, 2028; about 43 FTE; Herndon, VA. P00001 on Oct 23, 2026 is an administrative modification adding DD254, updating the PWS and changing the CO/CS; $0 (D, USAspending). Funding office "Off of the Dir CISA", extent competed "D: Full and Open Competition After Exclusion of Sources," 18 offers, contract type "Delivery Order," PSC R408, NAICS 336611 (D, read Oct 27). DHS's own acquisition forecast for the requirement (APFS 73860) says Full Small Business, NAICS 541611, $20–50M, which conflicts with the coding above and fits the work better than 336611 (D). HigherGov lists NAICS 336611 (shipbuilding), which does not fit the work. Resolved Oct 26 from the parent solicitation (D, 47QRCA23R0005 RFP text and Amendment 0009 of Jul 7, 2026): 336611 Ship Building and Repairing is the first NAICS code listed for orders in the Technical and Engineering Domain (CLIN 50201) and the Logistics Domain (CLIN 50801), size standard 1,300 employees, the broadest in those lists. A second OASIS+ WOSB IDV (47QRCA24DW048) also lists it alone (R, HigherGov). So the code comes from the vehicle's NAICS list, not from CISA (I). Accident, not trail; the one thing it does is give a 1,300-employee size standard.
- **PIA / SORN, feeds, court:** None (not a system).
- **Status since Jan 20, 2025:** Sept 30, 2026 award; part of the year-end CISA cluster. The competition record points to an ordinary buy (I). Same family of work as CIS-09 (HSIN-CI) and the EI-ISAC gap (FUS-01).
- **Open questions / records (U):** SOW and PWS for 70RCSJ26R00000008; whether SED's council support covers election-sector councils; what the Oct 23 DD254 adds (see below). Budget context (D, FY2027 CISA Congressional Justification, Program Change 26): the request eliminates 120 positions (101 FTE) and about $50.1M of Stakeholder Engagement (council management 35, stakeholder engagement 65, international affairs 20) and cuts the Stakeholder Engagement and Requirements line from about $90.2M to $31.2M. A $15M two-year contractor task order for SED signed Sep 30 against a proposed in-house cut: outsourcing, gap-filler, or expectation that Congress will not enact the cut (U, I).
- **USAspending read Oct 26 (D):** Award type label "Delivery Order" and contract type DELIVERY ORDER, while the description says "TASK ORDER" and the PSC is R408 (Support, Professional: Program Management/Support), a services code; so the label is an FPDS coding convention, not a supplies buy (I). Not R499 as earlier noted. Parent IDV 47QRCA24DW109 (IDC, multiple award, GSA FAS). 18 offers; extent competed D; commercial procedures not used; Clinger-Cohen "NO"; no federal account linked. Mod P00001 (Oct 23, $0): "ADMIN MOD TO ADD DD254, UPDATE PWS AND CHANGE CO/CS." (full text, read Oct 26; CO/CS = contracting officer / contract specialist). A DD254 is the security classification specification, meaning the work involves classified information or a facility clearance (K, verify); the PWS was updated at the same time. Funding office matches the default code, which resolves the earlier worry (D).

---

# PART F2 · HUD

### HUD-01 · HUD Enterprise Identity, Credential, and Access Management (EICAM, HUD/OCIO-07)
Map flows: none on the map
- **Owner:** HUD OCIO; notice issued by the Office of the Chief Information Security Officer, system HUD/OCIO-07 (D, FR 2026-15428, 91 FR 48175, Jul 30, 2026).
- **What it holds:** Identity and access records for "individuals who have been issued credentials for access to HUD data, systems, or facilities," which the notice says may include employees, former employees, contractors and grantees, state and local government partners, public housing authorities, private-sector partners, participating lenders, and tenants and program beneficiaries (D, read in the Federal Register text Oct 26). Fields include citizenship and place of birth, ID images and selfies, and risk scores and transaction details from third-party identity-proofing and fraud-prevention services (D). Okta Universal Directory is described as "the centralized, cloud-based source of truth for all user and device identities" (D). Identity proofing is "supported by Socure"; the system eliminates storing SSNs (D). SSA-provided PII is "not shared with EICAM" (D).
- **Vendor / vehicle:** Okta GovCloud on AWS GovCloud; Socure as identity-proofing service and listed record source (D). Contract vehicle not stated (U).
- **PIA / SORN:** HUD/OCIO-07, new system of records, Jul 30, 2026. Routine use (9): disclosure "to another Federal, State or local agency for the purpose of comparing to the agency's system of records or to non-Federal records, in coordination with an Office of Inspector General" for an audit, investigation or review under the Inspector General Act (D). This is standard model text (K), so it shows the channel exists, not that it has been used.
- **Inbound / outbound feeds:** Inbound from the HUD web access system, Active Directory, HR system, Okta, FHAC and Socure (D). Outbound presumably only through the 12 routine uses, which include law-enforcement and DOJ disclosures (I from the SORN).
- **Status since Jan 20, 2025:** New SORN Jul 30, 2026 (D). Correction: an earlier PHRASE_TRAIL note called this a workforce-only system; the notice's covered-individuals list is broader.
- **Open questions / records (U):** Whether any tenant or beneficiary verification uses citizenship status checks; any HUD use of SAVE; Socure contract vehicle.

---

# PART G · DOJ

### DOJ-01 · DOJ state voter-roll holdings
Map flows: f4, f5
- **Washington, Oct 26 (R, per Oct 27 watch):** Charles Neil Floyd and Pete Serrano of the U.S. Attorney's offices asked Secretary of State Hobbs to set aside ballots of 405 alleged noncitizen registrants (R, Washington State Standard, KOMO). Assistant AG Harmeet Dillon had requested the full unredacted roll earlier, and DOJ's suit for the roll was dismissed. No charges yet; Hobbs disputes the data. KOMO reports the names came from agent interviews of detainees and border crossers compared with immigration databases and public registration data; SAVE is not mentioned (our reading that it was not SAVE is an inference from silence, I). Not tied to a registry system beyond this entry (U).
- **Owner:** DOJ Civil Rights Division (D).
- **What it holds:** State voter rolls collected through demands and suits; about 50.6M records are reported (R; count not re-verified). Other holdings are U.
- **Vendor / vehicle:** U.
- **PIA / SORN:** None found for the roll collection (U).
- **Inbound feeds:** [f4] state voter rolls (D, suits and agreements). **Outbound feeds:** [f5] rolls to the DHS HQ team (DHS-06). OLC opinion, May 12, 2026: "no impediment" to sharing with HSI (D).
- **Court mentions:** CNA v. Mullin ECF 46, 87; Common Cause vacatur, Oct 9, 2026 (D; scope and effect on the holdings not re-checked, U).
- **Status since Jan 20, 2025:** EO 14248 (Mar 25, 2025) predicate; May 12, 2026 OLC; Oct 9, 2026 vacatur (D).
- **Open questions / records (U):** Whether the vacatur forces deletion or only bars use; where the files sit; who has access; whether DOJ copies exist outside the DHS-bound set.

### DOJ-02 · National Fraud Enforcement Division / NFDC hub
Map flows: f42, f43, f44, f45, f46, f47
- **Owner:** DOJ (D). Division announced Jan 2026, leader sworn in Apr 1, 2026, formally established by a Federal Register final rule Aug 18, 2026; the National Fraud Detection Center hub launched Aug 24, 2026 (D/R; DOJ release and law-firm summary). Related bills: H.R. 9576 (National Fraud Enforcement Division Act, would make the division permanent) and H.R. 10326 (federal-state fraud-data sharing) (R).
- **What it holds:** A hub that takes in referrals and data from PRAC, HSI, Treasury and tips, and passes leads to ballot suits (map f47) (D/R split per map).
- **Vendor / vehicle:** U. **PIA / SORN:** None found (U).
- **Inbound feeds:** [f42] RAVEn/HSI; [f43–f46] other agency feeds as drawn on the map (flow-level marks live in the map).
- **Outbound feeds:** [f47] leads to the ballot-suit track (R/I).
- **Court mentions:** None names the hub.
- **Status since Jan 20, 2025:** Aug 24, 2026 launch (D).
- **Open questions / records (U):** Charter; the data-sharing agreements for each inbound flow; whether it holds records or only routes them.

### DOJ-03 · DOJ Reconciliation Working Group
Map flows: none on the map
- **Owner:** DOJ (R/D).
- **What it holds:** A solicitation (SAM opportunity f9c99a484c6e43eca1e3b1a705575850) whose attachment is missing; no award found (U).
- **Vendor, PIA/SORN, feeds, court:** U.
- **Notice record (D, viewed on SAM.gov Oct 26):** Special notice published Nov 17, 2025; responses due Nov 20; inactive Nov 26. No attachment and no change history visible now, though the description says the terms "are provided as an attachment" (D), so an attachment existed at posting or was meant to. Responses due 3 days after posting is very short (D). Why the attachment is gone, and whether the notice was ever live, is U. Competing readings: H1 ordinary short special notice, attachment dropped on archiving; H2 attachment removed or withheld deliberately; H3 posted in error or pulled early; H4 posted late as a formality after the vendor was already chosen; H5 a standard no-cost trial arrangement with no deeper meaning. None is settled.
- **Open questions / records (U):** The attachment (terms); respondents; awardee; the Dec 31, 2025 report; relation to DOJ-01. Checks: SAM API record and /resources listing for the notice; web-archive captures from Nov 17–26, 2025; FOIA to DOJ Justice Management Division for the notice file, terms, capability statements and any report.

---

# PART H · Treasury, PRAC, SSA, State, Census, fusion centers

### TRE-01 · Treasury Do Not Pay
Map flows: f53
- **Owner:** Treasury Bureau of the Fiscal Service (D).
- **What it holds:** A payment-integrity matching service across federal and state data sets. Map flow 53 carries PCIS outflow to it (D/R per map).
- **Vendor / vehicle, PIA / SORN, court:** U.
- **Inbound feeds:** [f53] from PCIS. **Outbound feeds:** U.
- **Open questions / records (U):** Whether any voter-related field enters Do Not Pay; matching agreements; IG Act §6(j) reliance.

### TRE-02 · Fiscal Service analytics under H.R. 8312 §2
Map flows: none on the map
- **Owner:** Treasury (D for the bill text).
- **What it holds:** The bill would direct Treasury analytics; it passed the House Jun 10, 2026; no Senate action found (D/U).
- **Open questions / records (U):** Senate path; Peters plan overlap.

### TRE-03 · Treasury ".032" fraud-tip intake
Map flows: f54
- **Owner:** Treasury (D). Docket SORN-TREAS-DO-2026-0463; the companion Federal Register notice lists the information collection as "1505-NEW"; the number 1505-0284 is unverified (U).
- **What it holds:** Tips from the public. Whether voter-related tips are accepted: U.
- **Vendor / vehicle:** U. **Outbound feeds:** [f54] to the ballot-suit track (per map).
- **Open questions / records (U):** The SORN's routine uses; retention.

### TRE-04 · America.gov / Login.gov identity proofing
Map flows: none on the map
- **Owner:** GSA (Login.gov) and the America.gov effort (R/U).
- **What it holds:** Identity-proofing data. Socure is a subcontractor to Xcelerate Solutions on a five-year, $163M Login.gov identity-proofing call order (R, Biometric Update, Jul 2026). Any tie to a wider America.gov effort is unsourced (U).
- **Open questions / records (U):** Relation, if any, to CISA's Socure order (CIS-04). Treat as parallel unless a source links them.

### PRA-01 · PRAC analytics platform
Map flows: f43, f44 (as drawn)
- **Owner:** Pandemic Response Accountability Committee (D).
- **What it holds:** About 622M graph nodes and 1.65B relationships, over 1B records from more than 60 sources, as of Feb 2026 (D, PRAC testimony). Operates under the IG Empowerment Act §6(j) matching exemption (D, mechanism).
- **Vendor / vehicle:** U. **PIA / SORN:** U.
- **Open questions / records (U):** DUAs (the Oct 26 fusion-center note lists some); the §6(j) basis for any voter-related match.

### PRA-02 · SSA "yes/no" agreement
Map flows: f26, f27 (as drawn)
- **Owner:** SSA (D).
- **What it holds:** A verification agreement returning yes/no answers; the DOGE file of ~1,000 people (D, Jan 2026 filing) is separate (DHS-06 f27).
- **Open questions / records (U):** The agreement text and its date.

### SSA-01 · Numident
- **Owner:** SSA (K). **What it holds:** Identity and citizenship-at-enrollment data (K, verify). Citizenship accuracy limits are a known issue (K).
- **Write-back from SAVE (D, SSA press release Oct 20, 2026, opened and read Oct 27):** "Through data received from the Department of Homeland Security's Systematic Alien Verification for Entitlements (SAVE), SSA has updated approximately 25 million records that previously had missing citizenship information," and is correcting 8.5 million more with "inaccurate citizenship status." Same release: SSA has "corrected nearly 15 percent of all active SSNs," calls the database "our country's books and records," and says it strengthens "the foundation of identity data relied upon throughout government"; it also added 17 million death dates using SSA and State Department data; it does not mention voters or elections (D). So SAVE reads SSA data (f2) and SSA now writes SAVE output into its own records. Which SSA system holds the updates, the SORN or matching-agreement basis, and how many changes move a person from citizen to noncitizen are U. A SAVE error written into SSA's file could in principle later return as "SSA confirms" (I).
- **Open questions / records (U):** What DHS/USCIS can query.

### SSA-02 · Master Earnings File feed
- **Owner:** SSA (R/U). **What it holds:** Earnings records. Feed to DHS reported in the notes; direction and legal basis U.

### STA-01 · STATE-26 (State Department records, passports)
Map flows: f55
- **Owner:** State (D). FR 2026-21695 (91 FR 66906, Oct 23, 2026), State-26 Passport Services Records; effective on publication except routine uses (u), (v), (w), which take effect Nov 23, 2026 (D).
- **What it holds:** Passport application data; new routine use (w) allows sharing with entities "utilizing federal government verification platforms," including to verify identity or citizenship and voter eligibility; DHS is not named in any new routine use (D, SORN text).
- **Open questions / records (U):** Comments filed; routine-use text vs. voter use.

### STA-02 · Consular Consolidated Database (CCD)
- **Owner:** State (K). **What it holds:** Visa and passport records feeding TVS galleries (K).
- **Open questions / records (U):** Any new sharing since Jan 20, 2025.

### CEN-01 · Census voter-file purchase (DataClear / Bridgetree)
Map flows: f57
- **Owner:** Census Bureau (D).
- **What it holds:** Purchased commercial voter files. Award 13ADDC26C0002, $796K (D); Votebeat separately reports an $885,000 Data-Clear contract in 2024, which may be a different award (U).
- **Vendor / vehicle:** DataClear and Bridgetree, per notes (D/R).
- **Open questions / records (U):** Title 13 §9 firewall; whether files leave Census.

### CEN-02 · Census legal-status classification (residence rule)
Map flows: none on the map
- **Owner:** Census (D). 91 FR 57524, Sept 10, 2026; comments close Nov 2, 2026 (D).
- **What it holds:** A proposed rule on residence and legal-status classification for the census count.
- **Open questions / records (U):** Whether Census outputs reach DHS.

### FUS-01 · Fusion-center channel and 28 CFR Part 23
Budget note (D, CISA FY2027 Congressional Justification, Program Change 9, read Oct 26): the request cuts 14 positions and $39.6M for Election Security, eliminating the Election Security Advisors in each of the ten regions and not renewing the EI-ISAC cooperative agreement; justification: "conclude dedicated election security activities … adapt to evolving policy direction." A request, not enacted (funding runs on the continuing resolution to Dec 11).
Map flows: none on the map
- **Owner:** State and local fusion centers (D); DHS I&A links.
- **What it holds:** Intelligence sharing under 28 CFR Part 23 criminal-intelligence rules (D, mechanism). CISA's exchange (CIS-05) gives fusion centers access (D, plan).
- **Open questions / records (U):** The EI-ISAC gap after Sept 29, 2025; what a fusion center may retain from election-office reports.

---

# PART I · Map nodes without their own row

| Node | Flows | Where it appears |
|---|---|---|
| State voter databases and portals | f1, f2, f4 | DOJ-01, USC-01 |
| DMV / Nlets | f2 | USC-01 |
| EOIR | as drawn | ICE entries |
| IRS addresses | as drawn | DHS-06, USC |
| CMS Medicaid | as drawn | USC entries |
| FinCEN BSA | as drawn | ICE entries |
| "Independent sources" (48.2M) | f6 | DHS-06 |
| Data brokers | as drawn | ICE entries |
| DOGE teams → Cloudflare (SSA data shared through unapproved Cloudflare; DOJ correction filing, Jan 2026) (D) | f28 | DHS-06, PRA-02 |
| DOGE teams → political advocacy group ("voter data agreement" signed; filing says no evidence SSA data was shared; Hatch Act referrals) (D, use U) | f29 | DHS-06, PRA-02 |
| DOGE access to the USCIS lake / target-list compilation | f25, f27 | USC-04, DHS-06 |
| Ballot suits and county hold demands (f50: lists plus 48-hour hold demands and prosecution warnings, AP/Democracy Docket Oct 23–24, 2026, R) | f47, f49, f50, f54 | DOJ-02 |
| Field interviews | as drawn | ICE entries |
| VP Task Force reports | as drawn | DHS-06 |

---

# PART J · Appendices

## J1 · Contract-vehicle index
| Vehicle | Holder | Ceiling / value | Dates | Entries |
|---|---|---|---|---|
| 70RTAC26A00000001 (LSJ FY25-00257) | Palantir | $1B | Feb 12, 2026 to Feb 2031 | DHS-02, CIS-01 |
| 70RTAC26A00000010 | Databricks | $1B | Jul 17, 2026 to Jul 16, 2031 | DHS-03, CIS-02 |
| 70RTAC26A00000011 (SSJ FY26-0119) | Carahsoft | $2,657,393,210 | Jul 20, 2026 to Jul 19, 2031 | DHS-04, CIS-04 |
| 70RCSJ25A00000026 (DTSS) | AttainX, Electrosoft, SiloSmashers, SOFITC3 | $500M | Sept 30, 2025 | CIS-03 |
| 70RCSJ25A00000027 (DTSS) | SOFITC3 | per notes | Sept 30, 2025 to Sept 24, 2030 | CIS-07 |
| NASA SEWP NNG15SC03B | Carahsoft (for DVG) | $1,277,200 order | Sept 30, 2026 to Jan 15, 2027 | CIS-05 |

## J2 · Justification-sweep tracker
| Vendor / item | Status |
|---|---|
| Palantir LSJ FY25-00257 | Done |
| Carahsoft SSJ FY26-0119 | Done |
| PLANXS P00022 JEFO | Done Oct 26 (USC-04) |
| Socure order-level (70RCSJ26FC0000042) | Not retrieved |
| Clearview J&A-25-0183 (contract number match is I) | Done Oct 26 (COM-01) |
| VSPTS J&A-26-0230 | Done Oct 26 (ICE-11) |
| Booz Allen J&A-26-0191 (P00019) | Done Oct 26 (ICE-05) |
| DASS J&A-26-0099 | Withdrawn |
| Databricks, Senzing, LexisNexis, Thomson Reuters, Babel Street, Fivecast, ShadowDragon, Penlink, Cellebrite, SAS, NEC, IDEMIA, Axon | Not started |

Method: attachments are downloaded from SAM.gov and read in full (text extraction, or OCR for scans).

## J3 · Priority records to request
1. Unredacted Palantir LSJ and order-level files for CISA …0028.
2. SOW and system-boundary documents for CISA …0028, …0030, …0039, …0042, FR…0062.
3. DSAI SOW (when posted, ~Nov 16).
4. Order-level brand-name justification for the Socure order.
5. DOGE access logs or agreements for OBIM and SSA.
6. DOJ-01 storage, access and deletion status after the Oct 9 vacatur.

## J4 · Corrections found while building
- LWV order date: map flow 10 and an earlier working note say Jun 22, 2025; the suit was filed Sept 30, 2025. The registry uses Jun 22, 2026 (WL cite).
- TRX: the product name is DVG's own; only "Elections" is CISA-specific (correction of the Oct 24 note).
- CISA funding-office code is a default, not a signal (corrected Oct 25).
- SiloSmashers order year is 2026; the 2025 date belongs to the parent BPA.
- PLANXS II: earlier note said no award was found and the incumbent was extended; the P00022 justification says PLANXS II was competitively awarded, protested, and stop-worked (read Oct 26).
- P00019: reporting tied the five tasks to the HSI Innovation Lab; the redacted J&A shows neither the task names nor the Innovation Lab, and ties the work to EO 14390 scam call centers.
- EICAM (HUD): earlier PHRASE_TRAIL note called it a workforce-only identity system; the SORN's covered-individuals list includes tenants and program beneficiaries (found by the Oct 27 watch, confirmed in the FR text Oct 26).
- Other conflicts recorded in the individual USC and ICE entries.

## J6 · Check-against-registry protocol
For every new document, article or watch item: (1) find the system by ID; (2) compare each stated fact to the entry; (3) if it adds or conflicts, update the entry with a dated line and a mark; (4) if no system fits, add a row; (5) log the change below. Inherited marks are not re-verified unless stated.

## J7 · Change log
- 2026-10-27 (SAVE PIA read): DHS/USCIS/PIA-006(d) (Oct 31, 2025) read in full from the vault copy; USC-01 updated with its stated changes, SSA response fields, retention, queried systems and the ICE/CBP fraud-or-misuse sharing line.
- 2026-10-27 (primary documents opened from the vault and browser): (1) ICE LSJ J&A-25-0266 (SAM notice ICE_JA-25-0266, Jan 16, 2026) read in full: ICE-01 and ICE-02 upgraded from reporting to primary-document marks (Gotham-based ICM deployed 2016, O&M order 70CTD022FR0000170 to 2027, Enterprise Lakehouse requirements, derived-data ownership, 42 vendors assessed). (2) DHS-wide Palantir LSJ FY25-00257 text re-read: the quotes on department-wide data integration, interfaces within external agencies, coverage of all BPA orders, September 2026 delivery and the daily data export all match. (3) AttainX order 70RCSJ26FR0000055 read on USAspending: funding office, extent competed, 18 offers, PSC R408, NAICS 336611, P00001 confirmed; no set-aside on the order, and the recipient profile lists 8(a), women-owned and minority-owned small business. (4) GAO B-424623 (Oct 8, 2026) read: Octo Metric protest of a USCIS task order to AEX Digital denied; possible PLANXS II link recorded as an inference. (5) SAVE PIA-006(d) (Oct 2025) located; text not yet read.
- 2026-10-27 (USAspending check): amounts and dates confirmed or corrected for TRSS pilot PO, RELX/LexisNexis, Genesis, Senzing orders and the Axon order (Aug 26, 2026 action date).
- 2026-10-27 (evening): SAM solicitation 70SBUR26R00000015 (TRSS/FDNS pilot) read from the notice and attachment; Hilton ECF 132-40 read; SAVE User Reference Guide (June 2026) read; "100,000 records per batch" corrected to 100,000 base input records.
- 2026-10-27 (map update): map now shows flow f57 (eleven further systems SAVE queries, from SAVE PIA-006(d) pp. 7–9) and numbered bubbles sit near the source end of each line. YouTube link updated to the new channel.
- 2026-10-27 (third verification pass): audited 256 more document-supported claims. Corrected: FDNS vs USCIS attribution in the CNA order (the order says USCIS personnel; no "HQ election team"); LWV/EPIC/LULAC complaint no longer tied to the data lake; May 22, 2025 announcement does not mention SSA; FR 2025-16978 does not designate FDNS (Bartell n.1 does); State-26 routine use (w) does not name DHS; Burris quotes replaced with his written statement; Nextgov plan wording marked paraphrase and unverified; SSJ "including but not limited to" wording and Palantir/Databricks absence downgraded; Super Bowl testimony, NRMC contract title and amounts, HUD owner, OMB number, FBI/DOJ Clearview details, Axon/Guidehouse dates, earnings date. Unverified items (SAM, USAspending-only, PCIS PIA-087, LSJ details) stay marked U.
- 2026-10-27 (second verification pass): re-checked 85 document-supported claims and 10 open items. Corrected: Carahsoft BPA signed Jul 15, 2026, period Jul 20, 2026 to Jul 19, 2031 (number and $2,657,393,210 confirmed on USAspending); DTSS is four separate BPAs, one per holder; SAVE restriction cited to the SORN; CNA order wording on review quotas, commercial databases and TECS records; California complaint wording and list routing; FDNS law-enforcement designation cite; eCISCOR PIA quotes re-sourced; Palantir master-database quote; Palantir ELITE denial (unnamed spokesman via WIRED); HART PIA status; EI-ISAC predecessor agreement is the combined MS-ISAC/EI-ISAC award; CI3 and CISA-plan quotes softened to what was read; Census award figure conflict noted; Fivecast/FDNS pilot restored with ExecutiveBiz. CISA FY2027 budget lines (Program Changes 9 and 26) re-checked against the justification text and hold. Still unverifiable from public pages: many order numbers and justification quotes (USAspending, SAM.gov and the Palantir LSJ PDF could not be read).
- 2026-10-27 (claim re-verification): 131 R/I/U lines re-checked against sources. Corrected: SAVE SSN-lookup dates; ProPublica 25,000/15,000 leads (separate groups); PCQS/PCIS PIA direction; DHS dispute of third-party software; Palantir ELITE quote attribution (WIRED per Biometric Update, not CNN); DASS-to-RAVEn flow (f38) downgraded to inference; DASS purposes source (404 Media); Ninth Circuit Oct 25 wording; ATrac source list; Mobile Fortify PTA/PIA wording and Thompson attribution; Mobile Identify dates are report dates; Clearview license is CBP's; body-cam 'best interests' scope; HSIN World Cup attribution; Palantir/CISA quote; DOJ fraud-division dates and bill numbers (H.R. 9576, H.R. 10326); Washington Oct 26 letter details; Socure is a subcontractor on the Login.gov order; PRAC figures marked D. Unverified items remain labeled.
- 2026-10-26 (night): CIS-10 checked against USAspending page: PSC R408, Delivery Order label explained, P00001 adds DD254 and updates PWS, funding office confirmed.
- 2026-10-27 (morning): monitor output checked: SSA write-back added to SSA-01; Washington ballot-hold demand noted at DOJ-01. EICAM and Burris hearing already in.
- 2026-10-26 (night, 3): Added HUD-01 (EICAM) after the monitor run found tenants and beneficiaries in scope; corrected the workforce-only reading.
- 2026-10-26 (night, 2): FY2027 CISA Congressional Justification read: CADS added to CIS-01, SED consolidation to CIS-10, election-security cut to FUS-01.
- 2026-10-26 (late-night): CIS-10 NAICS resolved from the OASIS+ WOSB solicitation; posting-lag observation added to DHS-02 and DHS-04; Burris hearing text read (CIS-04).
- 2026-10-26 (late): Added CIS-10 (AttainX SED order, from HigherGov).
- 2026-10-26 (night): Read four justifications (PLANXS P00022, Clearview, VSPTS, Booz Allen P00019); updated USC-04, ICE-05, ICE-11, COM-01, J2, J4.
- 2026-10-26 (evening): DOJ-03 notice record and DHS-04 OEM-list reading added from a SAM.gov review.
- 2026-10-26: Registry created; flow numbers checked against the map; other marks inherited from earlier research notes.

