# EPICS & STORIES - Command Center Dashboard Backlog

**Product Owner:** Jayshree  
**Timeline:** July 9 - September 30, 2026  
**Definition of Done:** Task completed + Data accuracy 100% verified OR connection verified with data source

---

## EPIC M1: Strengthen Data Pipeline Reliability & Complete Regional Harmonization

**Owner:** Jayshree (Requirements), Karol (Data), Abi (Visuals)  
**Target:** Sprint 1-4 (Jul 9 - Sep 3)  
**Status:** In Progress (Media & SRE connections underway)

---

### STORY M1.1: Connect Media KPIs (WOA, AWT, MMR) to Command Center

**Owner:** Jayshree (Req), Karol (Data), Abi (Visuals)  
**Sprint:** 1-2  
**Visual Component:** Dashboard table display for Media KPIs

#### Task M1.1.1: Define WOA, AWT, MMR data requirements & mapping
- **Owner:** Jayshree
- **Input:** CDL data structure, current Media definitions
- **Output:** Requirement document with field mapping
- **DoD:** Mapping doc signed off by Santi (Media team)
- **Blocker:** None
- **Parallel Work:** Abi designs visual layout

#### Task M1.1.2: AWT Requirements & Data Quality Check
- **Owner:** Jayshree / Karol
- **Input:** Raw AWT data from Media source
- **Output:** AWT connection to CDL with 100% accuracy validation
- **DoD:** Data matches Media source (audit trail required)
- **Blocker:** None
- **Timeframe:** 5 days

#### Task M1.1.3: WOA Requirements & Data Quality Check
- **Owner:** Jayshree / Karol
- **Input:** Raw WOA data from Media source
- **Output:** WOA connection to CDL with 100% accuracy validation
- **DoD:** Data matches Media source (audit trail required)
- **Blocker:** None
- **Timeframe:** 5 days

#### Task M1.1.4: MMR (Mexico/Chile TV) Connection to CDL
- **Owner:** Jayshree
- **Input:** Mexico & Chile TV Media data
- **Output:** MMR data available in CDL
- **DoD:** 100% accuracy verified against source
- **Blocker:** Clarification on Mexico/Chile data source availability
- **Timeframe:** 5 days

#### Task M1.1.5: Sign-off from Media Team
- **Owner:** Santi (Media)
- **Input:** WOA, AWT, MMR validation results
- **Output:** Formal approval email
- **DoD:** Signed approval document
- **Blocker:** Tasks M1.1.2-M1.1.4 must be complete
- **Timeframe:** 2 days

#### Task M1.1.6: Create Media KPIs Visual Requirement
- **Owner:** Jayshree
- **Input:** Media KPI data structure, user feedback
- **Output:** Visual requirement doc (table layout, fields, filters)
- **DoD:** Approved by Abi for implementation
- **Parallel:** Task M1.1.2-5
- **Timeframe:** 3 days

#### Task M1.1.7: Build & Connect Media KPI Dashboard Table
- **Owner:** Abi
- **Input:** Visual requirement (Task M1.1.6), CDL data connection (Tasks M1.1.2-5)
- **Output:** Dashboard table displaying WOA, AWT, MMR with real-time refresh
- **DoD:** Table displays data, filters work, auto-refresh verified
- **Blocker:** Tasks M1.1.5, M1.1.6 must be complete
- **Timeframe:** 5 days

---

### STORY M1.2: Move Media BHT to Production Quality Data

**Owner:** Jayshree (Req), Karol (Data), Abi (Visuals)  
**Sprint:** 2  
**Visual Component:** BHT dashboard connection

#### Task M1.2.1: Data Quality Revision of Media BHT KPIs
- **Owner:** Jayshree / Karol
- **Input:** Current BHT staging data
- **Output:** Production-ready BHT data with quality metrics
- **DoD:** 100% data accuracy validated, no duplicates/nulls, matches source
- **Blocker:** None
- **Timeframe:** 5 days

#### Task M1.2.2: Switch Connection from Staging to Production
- **Owner:** Abi
- **Input:** Production-ready BHT data (Task M1.2.1)
- **Output:** Dashboard now queries production BHT data
- **DoD:** Connection verified, no data loss, query performance acceptable
- **Blocker:** Task M1.2.1 complete
- **Timeframe:** 2 days

#### Task M1.2.3: Validate BHT Data in Dashboard
- **Owner:** Jayshree
- **Input:** Production BHT dashboard connection
- **Output:** Verification report with sample records
- **DoD:** 100% accuracy confirmed
- **Blocker:** Task M1.2.2 complete
- **Timeframe:** 2 days

---

### STORY M1.3: Migrate SRE Nielsen KPIs to Strategic Metric View

**Owner:** Karol (Data), Abi (Visuals), Jayshree (Req)  
**Sprint:** 2-3  
**Visual Component:** SRE metric dashboard with channel detail

#### Task M1.3.1: Confirm Strategic KPIs from SRE (Nielsen source)
- **Owner:** Jayshree
- **Input:** Current SRE KPI list
- **Output:** Approved list of strategic KPIs to migrate to DGTM/CDL
- **DoD:** SRE team sign-off
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M1.3.2: Brazil Displays Connection from DGTM
- **Owner:** Karol
- **Input:** DGTM source connection details
- **Output:** Brazil display data flowing into CDL
- **DoD:** 100% connection accuracy verified
- **Blocker:** Task M1.3.1 complete
- **Timeframe:** 5 days

#### Task M1.3.3: Confirm Dashboard Connection to Strategic KPIs
- **Owner:** Abi
- **Input:** CDL data (Task M1.3.2)
- **Output:** Dashboard displays strategic KPIs in metric view
- **DoD:** Filters, drill-downs, and refresh working
- **Blocker:** Task M1.3.2 complete
- **Timeframe:** 3 days

---

### STORY M1.4: Deliver OSA Visibility at SRE-Equivalent Granularity

**Owner:** Jayshree (Req), Karol (Data), Abi (Visuals)  
**Sprint:** 3-4  
**Visual Component:** OSA table with granular detail  
**Blocker:** POS Launcher Approval (see Dependencies)

#### Task M1.4.1: Obtain Launcher Approval for POS Access
- **Owner:** Karol
- **Input:** POS data access request
- **Output:** Launcher approval ticket/email
- **DoD:** Formal approval from Launcher team
- **Blocker:** CRITICAL - Blocks all downstream OSA tasks
- **Timeframe:** 5-7 days (external dependency)

#### Task M1.4.2: Obtain POS Regional Approval for All LA Markets
- **Owner:** Jayshree
- **Input:** Regional stakeholder list
- **Output:** Approval from each LA market to access POS
- **DoD:** Signed approvals from all market leaders
- **Blocker:** CRITICAL - Blocks data pull
- **Timeframe:** 5-7 days (external dependency)
- **Dependency:** Task M1.4.1 must be complete

#### Task M1.4.3: Define OSA Granularity Equivalent to SRE Level
- **Owner:** Jayshree
- **Input:** SRE granularity specification, OSA current state
- **Output:** Requirement doc for OSA table structure (SKUs, channels, stores, time periods)
- **DoD:** Approved by data governance & SRE team
- **Blocker:** Tasks M1.4.1, M1.4.2 must be complete
- **Timeframe:** 3 days

#### Task M1.4.4: Create OSA Table from CDL to Dashboard
- **Owner:** Karol
- **Input:** OSA granularity requirement (Task M1.4.3), POS data (approved)
- **Output:** OSA data flowing from CDL to dashboard
- **DoD:** 100% accuracy verified against POS source
- **Blocker:** Task M1.4.3 complete, approvals granted
- **Timeframe:** 5 days

#### Task M1.4.5: Validate OSA Data Quality
- **Owner:** Jayshree
- **Input:** OSA table from CDL
- **Output:** Validation report with sample records
- **DoD:** 100% accuracy confirmed
- **Blocker:** Task M1.4.4 complete
- **Timeframe:** 2 days

#### Task M1.4.6: Create OSA Visual Requirement for Abi
- **Owner:** Jayshree
- **Input:** OSA data structure, user feedback
- **Output:** Visual requirement doc (table layout, filters, drill-downs)
- **DoD:** Approved by Abi for implementation
- **Parallel:** Tasks M1.4.1-5
- **Timeframe:** 3 days

#### Task M1.4.7: Build & Connect OSA Dashboard Table
- **Owner:** Abi
- **Input:** Visual requirement (Task M1.4.6), CDL data (Task M1.4.4)
- **Output:** Dashboard table displaying OSA with granular detail
- **DoD:** Table displays data, filters/drill-downs work, auto-refresh verified
- **Blocker:** Tasks M1.4.5, M1.4.6 complete
- **Timeframe:** 5 days

---

### STORY M1.5: Harmonize Sell Out and DOH Data Across All LA Markets

**Owner:** Jayshree (Req), Karol (Data), Vitoria (Sharepoint)  
**Sprint:** 2-3  
**Visual Component:** Harmonized Sell Out/DOH dashboard tables

#### Task M1.5.1: Document Current Sell Out & DOH Definitions by Market
- **Owner:** Jayshree
- **Input:** Current definitions from each LA market
- **Output:** Mapping doc showing differences in definitions/formats
- **DoD:** All LA markets documented
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M1.5.2: Define Harmonized Sell Out & DOH Standard
- **Owner:** Jayshree
- **Input:** Market definitions (Task M1.5.1), business requirements
- **Output:** Single standardized definition for all LA markets
- **DoD:** Approved by leadership & market leaders
- **Blocker:** Task M1.5.1 complete
- **Timeframe:** 5 days

#### Task M1.5.3: Map & Transform Sell Out/DOH Data to CDL
- **Owner:** Karol
- **Input:** Harmonized standard (Task M1.5.2), source data from all markets
- **Output:** Sell Out & DOH data in CDL with market filters
- **DoD:** 100% accuracy verified for each market
- **Blocker:** Task M1.5.2 complete
- **Timeframe:** 7 days

#### Task M1.5.4: Validate Harmonized Data Across Markets
- **Owner:** Jayshree
- **Input:** CDL data (Task M1.5.3)
- **Output:** Validation report confirming consistency across markets
- **DoD:** 100% accuracy, no gaps or duplicates
- **Blocker:** Task M1.5.3 complete
- **Timeframe:** 3 days

#### Task M1.5.5: Create Sell Out & DOH Visual Requirements
- **Owner:** Jayshree
- **Input:** Harmonized data structure
- **Output:** Visual requirement doc for Abi (filters by market, channel, time)
- **DoD:** Approved by Abi
- **Parallel:** Tasks M1.5.1-4
- **Timeframe:** 3 days

#### Task M1.5.6: Build Harmonized Sell Out & DOH Dashboard Tables
- **Owner:** Abi
- **Input:** Visual requirement (Task M1.5.5), CDL data (Task M1.5.3)
- **Output:** Dashboard tables displaying Sell Out & DOH by market
- **DoD:** Tables display data, filters work, market comparison enabled
- **Blocker:** Tasks M1.5.4, M1.5.5 complete
- **Timeframe:** 5 days

---

### STORY M1.6: Add Data Security Controls

**Owner:** Jayshree (Req), Karol (Data)  
**Sprint:** 3-4  
**Visual Component:** Access control logging & audit trails

#### Task M1.6.1: Define Data Security Requirements
- **Owner:** Jayshree
- **Input:** POS/Sell Out access restrictions, compliance requirements
- **Output:** Security requirement doc (field-level access, audit logging)
- **DoD:** Approved by data governance & security team
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M1.6.2: Implement Field-Level Access Controls in CDL
- **Owner:** Karol
- **Input:** Security requirements (Task M1.6.1)
- **Output:** CDL with role-based access controls
- **DoD:** Access controls tested & working, no unauthorized access
- **Blocker:** Task M1.6.1 complete
- **Timeframe:** 5 days

#### Task M1.6.3: Set Up Audit Logging for POS/Sell Out Data
- **Owner:** Karol
- **Input:** CDL access controls
- **Output:** Audit trail logging all POS/Sell Out queries
- **DoD:** Logs capturing user, timestamp, query, data accessed
- **Blocker:** Task M1.6.2 complete
- **Timeframe:** 3 days

#### Task M1.6.4: Validate Security Controls & Audit Trails
- **Owner:** Jayshree
- **Input:** Access controls & audit logs
- **Output:** Validation report
- **DoD:** Security controls working, audit logs accurate
- **Blocker:** Task M1.6.3 complete
- **Timeframe:** 2 days

---

## EPIC M2: Drive Business Adoption of Command Center

**Owner:** Jayshree (Req), Vitoria (Sharepoint/Training), Will (Deployment)  
**Target:** Sprint 1-2 (Jul 9 - Aug 6)  
**Status:** In Progress

---

### STORY M2.1: Sharepoint Launch + Training Sessions (CBA with CC included)

**Owner:** Vitoria (Lead), Will (Deployment), Jayshree (Req)  
**Sprint:** 1-2  
**Visual Component:** Sharepoint documentation, training videos

#### Task M2.1.1: Set Up Sharepoint Site Structure
- **Owner:** Vitoria
- **Input:** Site requirements, page hierarchy
- **Output:** Sharepoint site ready for content
- **DoD:** Site accessible, navigation working, permissions set
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M2.1.2: Develop Training Manual - Command Center How to Use
- **Owner:** Vitoria / Jayshree
- **Input:** Command Center features, user workflows
- **Output:** Comprehensive training manual (text + screenshots + videos)
- **DoD:** Manual covers all major features, tested by user group
- **Blocker:** None
- **Timeframe:** 7 days

#### Task M2.1.3: Create Official Metrics & Update Calendar
- **Owner:** Jayshree
- **Input:** All KPI definitions, refresh schedules
- **Output:** Source manual with metric definitions & official update dates
- **DoD:** All metrics documented, calendar published
- **Blocker:** M1 stories must be largely complete
- **Timeframe:** 5 days

#### Task M2.1.4: Prepare CBA Training (CC included)
- **Owner:** Will / Vitoria
- **Input:** Training manual (Task M2.1.2), Command Center workflows
- **Output:** CBA training session slides + exercises
- **DoD:** Training ready for delivery
- **Blocker:** Task M2.1.2 complete
- **Timeframe:** 5 days

#### Task M2.1.5: Launch Sharepoint Site & Publish Training Materials
- **Owner:** Vitoria / Will
- **Input:** Sharepoint site (Task M2.1.1), manual (M2.1.2), metrics (M2.1.3), CBA training (M2.1.4)
- **Output:** Sharepoint live with all training materials published
- **DoD:** Site accessible to all users, materials searchable, links working
- **Blocker:** Tasks M2.1.1-4 complete
- **Timeframe:** 2 days

#### Task M2.1.6: Conduct Training Sessions with Leadership & Market Leaders
- **Owner:** Will / Vitoria
- **Input:** Training materials (Task M2.1.5)
- **Output:** Training sessions completed, feedback collected
- **DoD:** All key users trained, competency verified
- **Blocker:** Task M2.1.5 complete
- **Timeframe:** 5 days (ongoing throughout Sprint 2)

---

### STORY M2.2: Improve Methodology Analysis Document v2.0

**Owner:** Jayshree (Req), Abi (Visuals)  
**Sprint:** 1-2  
**Visual Component:** Updated methodology documentation

#### Task M2.2.1: Review Current Methodology Document v1.0
- **Owner:** Jayshree
- **Input:** Current methodology doc
- **Output:** Gap analysis identifying what needs updating
- **DoD:** All gaps documented
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M2.2.2: Update Methodology with All New KPIs & Data Harmonization
- **Owner:** Jayshree / Abi
- **Input:** Gap analysis (Task M2.2.1), M1 work (Media KPIs, SRE Nielsen, OSA, Sell Out/DOH)
- **Output:** Methodology v2.0 including all new KPIs, definitions, formulas, harmonization rules
- **DoD:** All KPIs documented with clear definitions & lineage
- **Blocker:** M1 stories must be defined
- **Timeframe:** 7 days

#### Task M2.2.3: Add Visual Aids to Methodology v2.0
- **Owner:** Abi
- **Input:** Methodology v2.0 (Task M2.2.2)
- **Output:** Updated doc with diagrams, flowcharts, visual explanations
- **DoD:** Visuals clear and accurate
- **Blocker:** Task M2.2.2 complete
- **Timeframe:** 3 days

#### Task M2.2.4: Review & Approve Methodology v2.0 with Stakeholders
- **Owner:** Jayshree
- **Input:** Methodology v2.0 (Task M2.2.3)
- **Output:** Signed approval from leadership & data governance
- **DoD:** Approved, ready for publication
- **Blocker:** Task M2.2.3 complete
- **Timeframe:** 3 days

#### Task M2.2.5: Publish Methodology v2.0 to Sharepoint
- **Owner:** Vitoria
- **Input:** Approved methodology (Task M2.2.4)
- **Output:** v2.0 published on Sharepoint
- **DoD:** Document accessible, searchable, linked from main page
- **Blocker:** Task M2.2.4 complete
- **Timeframe:** 1 day

---

## EPIC M3: Integrate Pacifico and Ladmar Fully into Command Center's Regional View

**Owner:** Marcela (Data), Jayshree (Req), Abi (Visuals)  
**Target:** Sprint 3-4 (Aug 7 - Sep 3)  
**Status:** Discovery required

---

### STORY M3.1: Deliver Pacifico and Ladmar Sell Out and DOH Visibility

**Owner:** Marcela (Data/Sideload), Jayshree (Req), Abi (Visuals)  
**Sprint:** 3  
**Visual Component:** Pacifico & Ladmar Sell Out/DOH tables

#### Task M3.1.1: Identify Pacifico & Ladmar Data Sources & Owners
- **Owner:** Marcela
- **Input:** Internal data catalog, stakeholder interviews
- **Output:** Documented data sources (system name, contact, refresh frequency, format)
- **DoD:** All sources identified & contacts confirmed
- **Blocker:** CRITICAL - Blocks all downstream Pacifico/Ladmar tasks
- **Timeframe:** 5 days (external discovery)

#### Task M3.1.2: Define Pacifico & Ladmar Data Mapping
- **Owner:** Jayshree / Marcela
- **Input:** Data sources (Task M3.1.1), harmonized Sell Out/DOH definitions (M1.5.2)
- **Output:** Mapping doc for Pacifico & Ladmar data to standard schema
- **DoD:** Mapping document approved
- **Blocker:** Task M3.1.1 complete
- **Timeframe:** 3 days

#### Task M3.1.3: Sideload Pacifico Sell Out Data to CDL
- **Owner:** Marcela
- **Input:** Data source (Task M3.1.1), mapping (Task M3.1.2)
- **Output:** Pacifico Sell Out data in CDL with 100% accuracy
- **DoD:** Data matches source, no gaps/duplicates
- **Blocker:** Tasks M3.1.1, M3.1.2 complete
- **Timeframe:** 3 days

#### Task M3.1.4: Sideload Pacifico DOH Data to CDL
- **Owner:** Marcela
- **Input:** Data source (Task M3.1.1), mapping (Task M3.1.2)
- **Output:** Pacifico DOH data in CDL with 100% accuracy
- **DoD:** Data matches source, no gaps/duplicates
- **Blocker:** Tasks M3.1.1, M3.1.2 complete
- **Timeframe:** 3 days

#### Task M3.1.5: Sideload Ladmar Sell Out Data to CDL
- **Owner:** Marcela
- **Input:** Data source (Task M3.1.1), mapping (Task M3.1.2)
- **Output:** Ladmar Sell Out data in CDL with 100% accuracy
- **DoD:** Data matches source, no gaps/duplicates
- **Blocker:** Tasks M3.1.1, M3.1.2 complete
- **Timeframe:** 3 days

#### Task M3.1.6: Sideload Ladmar DOH Data to CDL
- **Owner:** Marcela
- **Input:** Data source (Task M3.1.1), mapping (Task M3.1.2)
- **Output:** Ladmar DOH data in CDL with 100% accuracy
- **DoD:** Data matches source, no gaps/duplicates
- **Blocker:** Tasks M3.1.1, M3.1.2 complete
- **Timeframe:** 3 days

#### Task M3.1.7: Validate Pacifico & Ladmar Data Quality
- **Owner:** Jayshree
- **Input:** CDL data (Tasks M3.1.3-6)
- **Output:** Validation report confirming 100% accuracy
- **DoD:** All data validated
- **Blocker:** Tasks M3.1.3-6 complete
- **Timeframe:** 3 days

#### Task M3.1.8: Create Pacifico & Ladmar Visual Requirements
- **Owner:** Jayshree
- **Input:** Sell Out & DOH data structure
- **Output:** Visual requirement doc for Abi (tables, filters, drill-downs)
- **DoD:** Approved by Abi
- **Parallel:** Tasks M3.1.1-7
- **Timeframe:** 3 days

#### Task M3.1.9: Build Pacifico & Ladmar Sell Out & DOH Dashboard Tables
- **Owner:** Abi
- **Input:** Visual requirement (Task M3.1.8), CDL data (Tasks M3.1.3-6)
- **Output:** Dashboard tables displaying Pacifico & Ladmar data
- **DoD:** Tables display data, filters work, drill-downs enabled
- **Blocker:** Tasks M3.1.7, M3.1.8 complete
- **Timeframe:** 5 days

---

### STORY M3.2: Launch Pacifico Market View

**Owner:** Jayshree (Req), Abi (Visuals)  
**Sprint:** 3  
**Visual Component:** Pacifico market view dashboard

#### Task M3.2.1: Define Pacifico Market View Requirements
- **Owner:** Jayshree
- **Input:** Pacifico data (M3.1), leadership requirements
- **Output:** Requirement doc specifying market view structure (KPIs, filters, drill-downs, exclusions like HHP)
- **DoD:** Approved by Pacifico market leader
- **Blocker:** Story M3.1 must provide data
- **Timeframe:** 3 days

#### Task M3.2.2: Create Pacifico Market View Table & Visual Design
- **Owner:** Jayshree / Abi
- **Input:** Market view requirements (Task M3.2.1)
- **Output:** Visual requirement doc for dashboard implementation
- **DoD:** Design approved
- **Blocker:** Task M3.2.1 complete
- **Timeframe:** 3 days

#### Task M3.2.3: Build Pacifico Market View Dashboard
- **Owner:** Abi
- **Input:** Visual requirement (Task M3.2.2), CDL data
- **Output:** Dashboard with Pacifico-specific metrics & drill-downs
- **DoD:** Market view functional, all filters working, performance acceptable
- **Blocker:** Task M3.2.2 complete
- **Timeframe:** 5 days

#### Task M3.2.4: Validate Pacifico Market View with Users
- **Owner:** Jayshree
- **Input:** Market view dashboard (Task M3.2.3)
- **Output:** User feedback & validation report
- **DoD:** Meets requirements, users confirmed accurate
- **Blocker:** Task M3.2.3 complete
- **Timeframe:** 2 days

---

### STORY M3.3: Connect Ladmar to Market View

**Owner:** Jayshree (Req), Abi (Visuals)  
**Sprint:** 3-4  
**Visual Component:** Ladmar market view dashboard

#### Task M3.3.1: Define Ladmar Market View Requirements
- **Owner:** Jayshree
- **Input:** Ladmar data (M3.1), leadership requirements
- **Output:** Requirement doc specifying market view structure
- **DoD:** Approved by Ladmar market leader
- **Blocker:** Story M3.1 must provide data
- **Timeframe:** 3 days

#### Task M3.3.2: Create Ladmar Market View Table & Visual Design
- **Owner:** Jayshree / Abi
- **Input:** Market view requirements (Task M3.3.1)
- **Output:** Visual requirement doc for dashboard implementation
- **DoD:** Design approved
- **Blocker:** Task M3.3.1 complete
- **Timeframe:** 3 days

#### Task M3.3.3: Build Ladmar Market View Dashboard
- **Owner:** Abi
- **Input:** Visual requirement (Task M3.3.2), CDL data
- **Output:** Dashboard with Ladmar-specific metrics & drill-downs
- **DoD:** Market view functional, all filters working
- **Blocker:** Task M3.3.2 complete
- **Timeframe:** 5 days

#### Task M3.3.4: Validate Ladmar Market View with Users
- **Owner:** Jayshree
- **Input:** Market view dashboard (Task M3.3.3)
- **Output:** User feedback & validation report
- **DoD:** Meets requirements, users confirmed accurate
- **Blocker:** Task M3.3.3 complete
- **Timeframe:** 2 days

---

## EPIC M4: Expand Command Center with Analytical Depth

**Owner:** Karol (Data), Jayshree (Req), Abi (Visuals)  
**Target:** Sprint 3-4 (Aug 7 - Sep 3)  
**Status:** In Progress

---

### STORY M4.1: Add Channel Granularity to Trade Panel

**Owner:** Karol (Data), Jayshree (Req), Abi (Visuals)  
**Sprint:** 3  
**Visual Component:** Trade panel with channel detail

#### Task M4.1.1: Define Channel Granularity Requirements for Trade Panel
- **Owner:** Jayshree
- **Input:** Current Trade Panel, user requirements
- **Output:** Requirement doc specifying channel-level breakdowns
- **DoD:** Approved by leadership
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M4.1.2: Add Channel Dimension to Trade Panel Data Pipeline
- **Owner:** Karol
- **Input:** Trade Panel source data, channel mapping
- **Output:** Trade Panel data with channel granularity in CDL
- **DoD:** 100% accuracy verified, no data loss
- **Blocker:** Task M4.1.1 complete
- **Timeframe:** 5 days

#### Task M4.1.3: Validate Channel-Granular Trade Panel Data
- **Owner:** Jayshree
- **Input:** Trade Panel data (Task M4.1.2)
- **Output:** Validation report confirming accuracy
- **DoD:** 100% accuracy confirmed
- **Blocker:** Task M4.1.2 complete
- **Timeframe:** 2 days

#### Task M4.1.4: Create Trade Panel Channel Visual Requirement
- **Owner:** Jayshree
- **Input:** Channel granular data
- **Output:** Visual requirement doc (table with channel drill-down)
- **DoD:** Approved by Abi
- **Parallel:** Tasks M4.1.1-3
- **Timeframe:** 3 days

#### Task M4.1.5: Build Trade Panel with Channel Detail
- **Owner:** Abi
- **Input:** Visual requirement (Task M4.1.4), CDL data (Task M4.1.2)
- **Output:** Dashboard table displaying Trade Panel by channel
- **DoD:** Channel drill-down working, filters functional
- **Blocker:** Tasks M4.1.3, M4.1.4 complete
- **Timeframe:** 5 days

---

### STORY M4.2: Add Channel Granularity to SRE

**Owner:** Karol (Data), Jayshree (Req), Abi (Visuals)  
**Sprint:** 4  
**Visual Component:** SRE table with channel detail

#### Task M4.2.1: Define Channel Granularity Requirements for SRE
- **Owner:** Jayshree
- **Input:** Current SRE metrics, user requirements
- **Output:** Requirement doc specifying channel-level breakdowns
- **DoD:** Approved by SRE team & leadership
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M4.2.2: Add Channel Dimension to SRE Data Pipeline
- **Owner:** Karol
- **Input:** SRE source data, channel mapping
- **Output:** SRE data with channel granularity in CDL
- **DoD:** 100% accuracy verified
- **Blocker:** Task M4.2.1 complete
- **Timeframe:** 5 days

#### Task M4.2.3: Validate Channel-Granular SRE Data
- **Owner:** Jayshree
- **Input:** SRE data (Task M4.2.2)
- **Output:** Validation report confirming accuracy
- **DoD:** 100% accuracy confirmed
- **Blocker:** Task M4.2.2 complete
- **Timeframe:** 2 days

#### Task M4.2.4: Create SRE Channel Visual Requirement
- **Owner:** Jayshree
- **Input:** Channel granular data
- **Output:** Visual requirement doc (table with channel drill-down)
- **DoD:** Approved by Abi
- **Parallel:** Tasks M4.2.1-3
- **Timeframe:** 3 days

#### Task M4.2.5: Build SRE Table with Channel Detail
- **Owner:** Abi
- **Input:** Visual requirement (Task M4.2.4), CDL data (Task M4.2.2)
- **Output:** Dashboard table displaying SRE by channel
- **DoD:** Channel drill-down working, filters functional
- **Blocker:** Tasks M4.2.3, M4.2.4 complete
- **Timeframe:** 5 days

---

### STORY M4.3: Add TOF KPI

**Owner:** Jayshree (Req), Karol (Data), Abi (Visuals)  
**Sprint:** 4  
**Visual Component:** TOF KPI dashboard table

#### Task M4.3.1: Define TOF KPI Requirements & Calculation
- **Owner:** Jayshree
- **Input:** TOF definition, source data requirements
- **Output:** Requirement doc specifying formula, data sources, granularity
- **DoD:** Approved by leadership
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M4.3.2: Build TOF KPI Data Pipeline
- **Owner:** Karol
- **Input:** TOF requirements (Task M4.3.1)
- **Output:** TOF KPI calculated and available in CDL
- **DoD:** 100% accuracy verified against source
- **Blocker:** Task M4.3.1 complete
- **Timeframe:** 5 days

#### Task M4.3.3: Validate TOF KPI Data Quality
- **Owner:** Jayshree
- **Input:** TOF data (Task M4.3.2)
- **Output:** Validation report
- **DoD:** 100% accuracy confirmed
- **Blocker:** Task M4.3.2 complete
- **Timeframe:** 2 days

#### Task M4.3.4: Create TOF Visual Requirement
- **Owner:** Jayshree
- **Input:** TOF data
- **Output:** Visual requirement doc (metric display, trends, filters)
- **DoD:** Approved by Abi
- **Parallel:** Tasks M4.3.1-3
- **Timeframe:** 3 days

#### Task M4.3.5: Add TOF KPI to Dashboard
- **Owner:** Abi
- **Input:** Visual requirement (Task M4.3.4), CDL data (Task M4.3.2)
- **Output:** TOF KPI displayed on dashboard
- **DoD:** KPI displays correctly, filters work
- **Blocker:** Tasks M4.3.3, M4.3.4 complete
- **Timeframe:** 3 days

---

### STORY M4.4: Add SRE PSKUs

**Owner:** Karol (Data), Jayshree (Req), Abi (Visuals)  
**Sprint:** 4  
**Visual Component:** SRE PSKU detail table

#### Task M4.4.1: Define SRE PSKU Requirements
- **Owner:** Jayshree
- **Input:** PSKU definition, SRE requirements
- **Output:** Requirement doc specifying PSKU granularity
- **DoD:** Approved by SRE team
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M4.4.2: Add PSKU Dimension to SRE Data Pipeline
- **Owner:** Karol
- **Input:** SRE source data, PSKU mapping (Task M4.4.1)
- **Output:** SRE data with PSKU detail in CDL
- **DoD:** 100% accuracy verified
- **Blocker:** Task M4.4.1 complete
- **Timeframe:** 5 days

#### Task M4.4.3: Validate PSKU Data Quality
- **Owner:** Jayshree
- **Input:** SRE PSKU data (Task M4.4.2)
- **Output:** Validation report
- **DoD:** 100% accuracy confirmed
- **Blocker:** Task M4.4.2 complete
- **Timeframe:** 2 days

#### Task M4.4.4: Create SRE PSKU Visual Requirement
- **Owner:** Jayshree
- **Input:** PSKU data
- **Output:** Visual requirement doc (table with PSKU drill-down)
- **DoD:** Approved by Abi
- **Parallel:** Tasks M4.4.1-3
- **Timeframe:** 3 days

#### Task M4.4.5: Add SRE PSKU Table to Dashboard
- **Owner:** Abi
- **Input:** Visual requirement (Task M4.4.4), CDL data (Task M4.4.2)
- **Output:** Dashboard table displaying SRE by PSKU
- **DoD:** PSKU drill-down working, filters functional
- **Blocker:** Tasks M4.4.3, M4.4.4 complete
- **Timeframe:** 5 days

---

### STORY M4.5: Add SRE Targets

**Owner:** Jayshree (Req), Karol (Data), Abi (Visuals)  
**Sprint:** 4  
**Visual Component:** SRE targets comparison dashboard  
**Note:** Targets to be defined by leadership

#### Task M4.5.1: Define SRE Targets with Leadership
- **Owner:** Jayshree
- **Input:** SRE historical data, business objectives
- **Output:** Target values for each SRE KPI by market/channel (to be confirmed by leadership)
- **DoD:** Targets approved by leadership
- **Blocker:** CRITICAL - Requires stakeholder input
- **Timeframe:** 5-7 days (external dependency)

#### Task M4.5.2: Build SRE Targets Data Store
- **Owner:** Karol
- **Input:** SRE targets (Task M4.5.1)
- **Output:** Target values stored in CDL, linked to SRE KPIs
- **DoD:** Targets accessible for comparison
- **Blocker:** Task M4.5.1 complete
- **Timeframe:** 3 days

#### Task M4.5.3: Create SRE vs. Target Visual Requirement
- **Owner:** Jayshree / Abi
- **Input:** Target data (Task M4.5.2)
- **Output:** Visual requirement doc (comparison tables, variance highlighting, trend charts)
- **DoD:** Design approved
- **Blocker:** Task M4.5.2 complete
- **Timeframe:** 3 days

#### Task M4.5.4: Build SRE Targets Dashboard (Variance & Comparison)
- **Owner:** Abi
- **Input:** Visual requirement (Task M4.5.3), CDL data
- **Output:** Dashboard showing SRE metrics vs. targets with color-coded variance
- **DoD:** Variance highlighted, drill-downs working
- **Blocker:** Task M4.5.3 complete
- **Timeframe:** 5 days

---

## EPIC M5: Transition L1–L2 Operations to AMS

**Owner:** Jayshree (Req), Karol (Data), AMS (External)  
**Target:** Sprint 5-6 (Sep 4 - Sep 30)  
**Status:** To be scheduled

---

### STORY M5.1: Define & Document CPS for AMS Transition

**Owner:** Jayshree (Req)  
**Sprint:** 5  
**Visual Component:** CPS documentation

#### Task M5.1.1: Define AMS Transition Scope
- **Owner:** Jayshree
- **Input:** Current operations, AMS capability assessment
- **Output:** Scope doc specifying L1-L2 operations to transition
- **DoD:** Approved by leadership & AMS
- **Blocker:** None (requires AMS coordination)
- **Timeframe:** 5 days

#### Task M5.1.2: Document Current Processes (Runbooks)
- **Owner:** Jayshree / Karol
- **Input:** Existing operational procedures
- **Output:** Comprehensive runbooks for all operational tasks
- **DoD:** All processes documented, reviewed, validated
- **Blocker:** None
- **Timeframe:** 7 days

#### Task M5.1.3: Define SLAs for AMS Operational Support
- **Owner:** Jayshree
- **Input:** Current performance targets, user requirements
- **Output:** SLA document specifying response times, uptime, data refresh SLAs
- **DoD:** SLAs approved by leadership & AMS
- **Blocker:** Task M5.1.1 complete
- **Timeframe:** 5 days

#### Task M5.1.4: Define AMS Staffing Plan
- **Owner:** Jayshree
- **Input:** Operational requirements, AMS resource availability
- **Output:** Staffing plan specifying roles, hours, coverage
- **DoD:** Staffing approved by leadership & AMS
- **Blocker:** Task M5.1.1 complete
- **Timeframe:** 5 days

#### Task M5.1.5: Create Transition Plan & Cutover Schedule
- **Owner:** Jayshree
- **Input:** Scope (M5.1.1), runbooks (M5.1.2), SLAs (M5.1.3), staffing (M5.1.4)
- **Output:** Detailed transition plan with cutover schedule
- **DoD:** Plan approved, cutover date confirmed
- **Blocker:** Tasks M5.1.1-4 complete
- **Timeframe:** 3 days

---

### STORY M5.2: Knowledge Transfer & Training

**Owner:** Jayshree (Req), Karol (Data), AMS (External)  
**Sprint:** 5-6  
**Visual Component:** Training materials, documentation

#### Task M5.2.1: Develop AMS Training Curriculum
- **Owner:** Jayshree / Karol
- **Input:** Runbooks (M5.1.2), system architecture, operational workflows
- **Output:** Comprehensive training program (theory, hands-on exercises)
- **DoD:** Curriculum covers all L1-L2 tasks
- **Blocker:** Task M5.1.2 complete
- **Timeframe:** 5 days

#### Task M5.2.2: Conduct AMS Technical Training
- **Owner:** Karol / Jayshree
- **Input:** Training curriculum (Task M5.2.1)
- **Output:** AMS team trained on data pipelines, CDL, troubleshooting
- **DoD:** Training sessions completed, AMS team competent
- **Blocker:** Task M5.2.1 complete
- **Timeframe:** 5 days

#### Task M5.2.3: Conduct AMS Operational Training
- **Owner:** Jayshree
- **Input:** Training curriculum (Task M5.2.1)
- **Output:** AMS team trained on operations, user support, escalation procedures
- **DoD:** Training sessions completed, AMS ready for operations
- **Blocker:** Task M5.2.1 complete
- **Timeframe:** 5 days

#### Task M5.2.4: Run Parallel Operations (AMS shadow/observation)
- **Owner:** Jayshree / Karol / AMS
- **Input:** Training (Tasks M5.2.2-3)
- **Output:** AMS observes and participates in real operations
- **DoD:** AMS demonstrates competency, issues logged and resolved
- **Blocker:** Tasks M5.2.2-3 complete
- **Timeframe:** 5 days

#### Task M5.2.5: Conduct Cutover & Go-Live
- **Owner:** Jayshree / Karol / AMS
- **Input:** Transition plan (M5.1.5), parallel operations (M5.2.4)
- **Output:** Operations formally transferred to AMS
- **DoD:** AMS fully responsible, all support procedures working
- **Blocker:** Task M5.2.4 complete
- **Timeframe:** 2 days

---

## EPIC M6: Deliver Trend Visibility & Refreshed Visual Experience

**Owner:** Abi (Visuals), Jayshree (Req), Karol (Data)  
**Target:** Sprint 5-6 (Sep 4 - Sep 30)  
**Status:** Design in progress (Lingaro)

---

### STORY M6.1: Add KPI Trend Visuals for SRE

**Owner:** Abi (Visuals), Jayshree (Req), Karol (Data)  
**Sprint:** 5  
**Visual Component:** SRE trend charts

#### Task M6.1.1: Define SRE Trend Requirements
- **Owner:** Jayshree
- **Input:** User feedback, analytics requirements
- **Output:** Requirement doc specifying trend metrics, time periods, visualizations
- **DoD:** Approved by SRE team & leadership
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M6.1.2: Prepare SRE Historical Data for Trends
- **Owner:** Karol
- **Input:** SRE historical data (M1.3), trend requirements (Task M6.1.1)
- **Output:** Historical SRE data indexed for trend analysis
- **DoD:** Data available for all time periods specified
- **Blocker:** Task M6.1.1 complete
- **Timeframe:** 3 days

#### Task M6.1.3: Design Trend Visualizations (Charts & Graphs)
- **Owner:** Abi
- **Input:** Trend requirements (Task M6.1.1), historical data (Task M6.1.2)
- **Output:** Design mockups for trend charts (line charts, forecasts, variance bands)
- **DoD:** Design validated with users
- **Blocker:** Tasks M6.1.1-2 complete
- **Timeframe:** 3 days

#### Task M6.1.4: Build SRE Trend Dashboard
- **Owner:** Abi
- **Input:** Design (Task M6.1.3), CDL data (Task M6.1.2)
- **Output:** Interactive trend charts on dashboard
- **DoD:** Charts display correctly, drill-downs work, performance acceptable
- **Blocker:** Task M6.1.3 complete
- **Timeframe:** 5 days

#### Task M6.1.5: Validate Trend Data & Visualizations
- **Owner:** Jayshree
- **Input:** Trend dashboard (Task M6.1.4)
- **Output:** Validation report confirming accuracy
- **DoD:** 100% accuracy confirmed, trends visually accurate
- **Blocker:** Task M6.1.4 complete
- **Timeframe:** 2 days

---

### STORY M6.2: Deploy Lingaro-Designed Visual Refresh (User-Validated)

**Owner:** Abi (Visuals), Vitoria (Validation), Jayshree (Req)  
**Sprint:** 5-6  
**Visual Component:** Complete dashboard visual redesign

#### Task M6.2.1: Review Lingaro Design Mockups
- **Owner:** Abi
- **Input:** Lingaro design deliverables
- **Output:** Design review & technical feasibility assessment
- **DoD:** Design feasible, technical questions resolved with Lingaro
- **Blocker:** None
- **Timeframe:** 3 days

#### Task M6.2.2: Validate Lingaro Design with Leadership & Users
- **Owner:** Vitoria / Jayshree
- **Input:** Lingaro design mockups (Task M6.2.1)
- **Output:** User validation report confirming design acceptance
- **DoD:** Design approved by leadership & key users
- **Blocker:** Task M6.2.1 complete
- **Timeframe:** 5 days

#### Task M6.2.3: Create Implementation Requirements for Visual Refresh
- **Owner:** Jayshree / Abi
- **Input:** Validated design (Task M6.2.2)
- **Output:** Detailed technical requirements for Abi (layout, components, responsive design, accessibility)
- **DoD:** Requirements document approved
- **Blocker:** Task M6.2.2 complete
- **Timeframe:** 3 days

#### Task M6.2.4: Implement Lingaro Visual Refresh
- **Owner:** Abi
- **Input:** Implementation requirements (Task M6.2.3)
- **Output:** Dashboard visually refreshed per Lingaro design
- **DoD:** All design elements implemented, responsive, performance validated
- **Blocker:** Task M6.2.3 complete
- **Timeframe:** 7 days

#### Task M6.2.5: Conduct Final UAT & Testing
- **Owner:** Jayshree / Vitoria / Abi
- **Input:** Refreshed dashboard (Task M6.2.4)
- **Output:** UAT report, bug fixes, performance validation
- **DoD:** All bugs fixed, performance acceptable, user sign-off obtained
- **Blocker:** Task M6.2.4 complete
- **Timeframe:** 5 days

#### Task M6.2.6: Deploy Visual Refresh to Production
- **Owner:** Abi
- **Input:** UAT approved (Task M6.2.5)
- **Output:** Refreshed dashboard live in production
- **DoD:** Deployment successful, no issues, users notified
- **Blocker:** Task M6.2.5 complete
- **Timeframe:** 1 day

---

## Backlog Items (Post-Sept 30)

These items are not part of core Milestones 1-6 but should be tracked for future sprints:

### Backlog Story B1: Sell In, Sell Out, Trade Inventory Improvement
- **Owner:** TBD
- **Effort:** TBD
- **Description:** Comprehensive improvement of Sell In, Sell Out, and trade inventory data

### Backlog Story B2: WWMD Share Enhancement
- **Owner:** TBD
- **Effort:** TBD
- **Description:** Enhance WWMD (World-Wide Market Data) share visibility

### Backlog Story B3: HHP New Contract Review & Connection
- **Owner:** TBD
- **Effort:** TBD
- **Description:** Review HHP new contracts and integrate into Command Center

### Backlog Story B4: Explore OSA SKUs
- **Owner:** TBD
- **Effort:** TBD
- **Description:** Explore additional OSA SKU granularity

### Backlog Story B5: Fabric - Split by Segment (Liquid & Powder)
- **Owner:** Jayshree
- **Effort:** TBD
- **Description:** Separate Fabric data by segment (Liquid vs. Powder) in dashboard

### Backlog Story B6: SRE Color Coding to Targets
- **Owner:** Abi
- **Effort:** TBD
- **Description:** Implement color-coded visual indicators for SRE performance vs. targets

### Backlog Story B7: Confirm Media Help Pending
- **Owner:** Jayshree
- **Effort:** TBD
- **Description:** Confirm pending items with Media team

### Backlog Story B8: DOH & Sell Out JAS Sideloads
- **Owner:** TBD
- **Effort:** TBD
- **Description:** Maintain DOH & Sell Out sideloads for JAS market

### Backlog Story B9: HHP Hierarchy Review in Gold Table
- **Owner:** Jayshree
- **Effort:** TBD
- **Description:** Review and update HHP hierarchy in Gold Table

### Backlog Story B10: Document & Add Methodology
- **Owner:** Abi / Jayshree
- **Effort:** TBD
- **Description:** Ongoing documentation of methodology updates

### Backlog Story B11: Add Schedule for Update Dates
- **Owner:** Abi
- **Effort:** TBD
- **Description:** Document official update dates/schedules for all metrics

---

## End of Epics & Stories

