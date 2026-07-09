COMMAND CENTER DASHBOARD - EMAIL TEMPLATE FOR AMS PENDING ITEMS REQUEST

TO: AMS Leadership Team
CC: Jayshree (Product Owner)
SUBJECT: Command Center Dashboard - AMS Transition Pending Items Assessment (Response Required by [DATE])

---

Dear AMS Team,

As we prepare for the transition of Command Center Dashboard L1-L2 operations to AMS (target: September 30, 2026), we need a comprehensive inventory of all pending items, gaps, and dependencies to ensure a smooth handoff.

Please respond to this structured request by [DATE]. Your detailed responses will inform our transition plan, training curriculum, and go-live readiness.

---

SECTION 1: OPERATIONAL READINESS

1.1 Current State Assessment
Please confirm the following regarding AMS's current capability to support Command Center:

   a) Has AMS reviewed the Command Center architecture documentation?
      [ ] Yes, fully reviewed
      [ ] Partially reviewed
      [ ] Not yet reviewed
      Please provide date of review: ___________

   b) Does AMS have access to all required systems (CDL, DGTM, Trade Panel, etc.)?
      [ ] Yes, full access
      [ ] Partial access (specify which systems): _________________________
      [ ] No access yet
      If not, please specify access request requirements: _____________

   c) Has AMS identified a primary technical contact for each of these areas?
      [ ] Data pipeline & ETL support
      [ ] Dashboard architecture & configuration
      [ ] Database administration (CDL, DGTM)
      [ ] User support & troubleshooting
      Please list names and contact information for each role: _____________

1.2 Pending System Access & Credentials
List all system access requests that are still pending:

   System Name | Purpose | Status | Expected Completion Date
   _____________________________________________________________

1.3 Pending Training or Certifications
Are there any certifications, tool training, or prerequisite trainings AMS requires before go-live?

   Training / Certification | Status | Target Completion | Owner
   _____________________________________________________________

---

SECTION 2: TECHNICAL & DATA DEPENDENCIES

2.1 Data Sources & Refresh Schedules
Please confirm AMS has documentation on all data sources and their refresh frequencies. List any sources where documentation is missing or requires clarification:

   Data Source | Current Status | Missing/Needs Clarification | Owner
   _____________________________________________________________

2.2 Known Data Quality Issues
Are there any known data quality issues, gaps, or reconciliation problems AMS should be aware of? Please list:

   Issue Description | Affected KPI/Source | Current Workaround | Target Resolution Date
   _____________________________________________________________

2.3 Pending Data Integrations
Identify any data integrations or connections that are not yet complete as of this assessment:

   Integration | Expected Completion | Owner | Impact if Delayed
   _____________________________________________________________

Examples:
   - Pacifico & Ladmar Sell Out/DOH sideloads
   - SRE Nielsen KPI migration to DGTM/CDL
   - OSA visibility (pending POS approvals)
   - SRE targets definition

2.4 Recurring Data Issues
Are there any recurring manual interventions, sideloads, or workarounds currently in place that AMS will need to maintain?

   Workaround | Frequency | Manual Steps Required | Estimated Time | Owner
   _____________________________________________________________

---

SECTION 3: DOCUMENTATION & RUNBOOKS

3.1 Runbook Gaps
Which operational runbooks do you need from Jayshree's team before go-live? (Check all that apply)

   [ ] Data refresh failure troubleshooting
   [ ] Dashboard performance degradation response
   [ ] Data accuracy validation procedures
   [ ] User access & permission management
   [ ] Emergency data rollback procedures
   [ ] SLA monitoring & alerting setup
   [ ] Incident escalation procedures
   [ ] Vendor communication (Nielsen, DGTM, CDL owners, etc.)
   [ ] Other (please specify): _________________________

3.2 Documentation Status
For each of the following, confirm the documentation status:

   Document | Available? | Complete? | Needs Update? | Notes
   ___________________________________________________________________
   Architecture & System Diagram | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   Data Dictionary | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   KPI Definitions & Formulas | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   Source System Integration Specs | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   Dashboard Configuration Guide | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   User Role & Permission Matrix | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   Vendor Contact List | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |

---

SECTION 4: SUPPORT & ESCALATION PROCEDURES

4.1 Escalation Matrix
Does AMS have clarity on escalation procedures for the following scenarios?

   Scenario | Escalation Owner | Response SLA | Acknowledged?
   ___________________________________________________________________
   Data discrepancy (±5% variance) | | | [ ] Y [ ] N
   Data missing for full refresh cycle | | | [ ] Y [ ] N
   Dashboard performance issues | | | [ ] Y [ ] N
   User access/permission issues | | | [ ] Y [ ] N
   Data security/compliance incident | | | [ ] Y [ ] N
   Vendor-side outage/issue | | | [ ] Y [ ] N

4.2 User Support Requirements
What user support capabilities does AMS plan to provide?

   Support Type | Hours of Operation | Response Time | Owner | Status
   ___________________________________________________________________
   Email support | | | |
   Phone support | | | |
   Dashboard training | | | |
   Ad-hoc queries/reports | | | |
   KPI explanation/guidance | | | |

---

SECTION 5: STAFFING & CAPACITY

5.1 Staffing Plan
Please provide AMS's proposed staffing plan:

   Role | Name | FTE | Start Date | Training Complete? | Notes
   ___________________________________________________________________
   Primary Data Operations Lead | | | | [ ] Y [ ] N |
   Secondary Data Operations Lead | | | | [ ] Y [ ] N |
   Dashboard Support Analyst | | | | [ ] Y [ ] N |
   Database Administrator | | | | [ ] Y [ ] N |

5.2 Capacity & Bandwidth
On a scale of 1-10, how confident is AMS in having sufficient capacity to support Command Center operations alongside existing responsibilities?

   Confidence Level: ___/10
   
   If below 7, please explain capacity constraints and potential gaps:
   _________________________________________________________________

5.3 Contingency Staffing
Does AMS have backup/contingency staffing in place for key roles during vacation, illness, or other absences?

   [ ] Yes, clearly documented
   [ ] Partial (some roles covered)
   [ ] No, not planned yet
   
   Please describe: _________________________________________________

---

SECTION 6: TECHNOLOGY & TOOLS

6.1 Monitoring & Alerting
Does AMS have the monitoring and alerting infrastructure in place for Command Center?

   Tool/Platform | Required? | Available? | Configured? | Owner
   ___________________________________________________________________
   Dashboard uptime monitoring | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   Data refresh success/failure alerts | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   Performance metrics dashboard | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   Incident ticketing system | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |
   Data lineage/impact analysis tools | [ ] Y [ ] N | [ ] Y [ ] N | [ ] Y [ ] N |

6.2 Change Management
Does AMS have a change management process in place? If yes, describe:

   [ ] Yes, describe process: _________________________________________
   [ ] No, please propose process: ____________________________________

6.3 Pending Tool Implementations
Are there any tools or platforms that AMS needs to implement before go-live?

   Tool | Purpose | Timeline | Owner | Blocker?
   ___________________________________________________

---

SECTION 7: TRAINING & READINESS

7.1 Training Requirements Checklist
Please confirm AMS has the training scheduled for the following topics:

   Topic | Scheduled Date | Attendees | Owner | Status
   ___________________________________________________________________
   Command Center architecture & data flow | | | | [ ] Complete [ ] Scheduled [ ] Not scheduled
   CDL/DGTM systems overview | | | | [ ] Complete [ ] Scheduled [ ] Not scheduled
   Data pipeline operations & troubleshooting | | | | [ ] Complete [ ] Scheduled [ ] Not scheduled
   Dashboard configuration & customization | | | | [ ] Complete [ ] Scheduled [ ] Not scheduled
   Vendor communication & escalation | | | | [ ] Complete [ ] Scheduled [ ] Not scheduled
   SLA management & reporting | | | | [ ] Complete [ ] Scheduled [ ] Not scheduled
   User support & issue resolution | | | | [ ] Complete [ ] Scheduled [ ] Not scheduled
   Dry-run operations (parallel operations) | | | | [ ] Complete [ ] Scheduled [ ] Not scheduled

7.2 Knowledge Transfer Format Preference
In what format does AMS prefer knowledge transfer? (Check all that apply)

   [ ] Documentation & runbooks (written)
   [ ] Video recordings of procedures
   [ ] Live training sessions (in-person or virtual)
   [ ] Hands-on labs/sandbox environment
   [ ] 1:1 pairing/mentoring
   [ ] Other: _________________________

---

SECTION 8: CRITICAL DEPENDENCIES & BLOCKERS

8.1 AMS-Side Blockers
Are there any AMS-internal dependencies, blockers, or risks that could impact go-live readiness?

   Blocker | Impact | Proposed Resolution | Target Resolution Date
   _________________________________________________________________

8.2 External Dependencies
Are there any external (vendor, third-party) dependencies AMS needs to flag?

   Dependency | Impact | Owner | Target Resolution Date
   _________________________________________________________________

---

SECTION 9: GO-LIVE READINESS

9.1 Readiness Assessment
On a scale of 1-10, how ready is AMS for Command Center go-live on September 30, 2026?

   Readiness Score: ___/10
   
   If below 8, what is required to increase readiness?
   _________________________________________________________________

9.2 Risks & Mitigation
What are AMS's top 3 risks for Command Center transition, and how will they be mitigated?

   Risk #1: _________________________________________________________________
   Mitigation: _____________________________________________________________
   
   Risk #2: _________________________________________________________________
   Mitigation: _____________________________________________________________
   
   Risk #3: _________________________________________________________________
   Mitigation: _____________________________________________________________

9.3 Go-Live Cutover Plan
Has AMS reviewed and agreed with the proposed cutover plan (target: September 30, 2026)?

   [ ] Yes, ready to proceed
   [ ] Yes, with modifications (please specify): _______________________
   [ ] No, not ready (please explain): ________________________________

---

SECTION 10: FOLLOW-UP ACTIONS & NEXT STEPS

10.1 Outstanding Questions
Does AMS have any outstanding questions or clarifications needed from Jayshree's team?

   Question | Topic | Priority (High/Medium/Low) | Required By
   _________________________________________________________________

10.2 Proposed Next Meeting
When should we schedule the next synchronization meeting to address pending items?

   Proposed Date/Time: _________________________________________________
   
   Recommended Attendees:
   - AMS Primary Contact: ___________________________________________
   - AMS Technical Lead: ___________________________________________
   - Jayshree (PO): [always included]
   - Karol (Data): [ ] needed [ ] not needed
   - Abi (Visuals): [ ] needed [ ] not needed

---

RESPONSE INSTRUCTIONS

Please complete this assessment and return by [DATE] to Jayshree at [EMAIL].

Format: Please use this same template and fill in all sections marked with [ ] or _____.

Clarity: If you cannot provide a complete answer, indicate "TBD" and specify the expected completion date.

Escalation: If you identify any HIGH-PRIORITY blockers, please notify Jayshree immediately (do not wait for full assessment submission).

---

THANK YOU

Thank you for your thorough assessment. Your detailed responses will ensure we have a comprehensive transition plan and maximize the likelihood of a successful go-live.

Please reach out with any questions about this request.

Best regards,
Jayshree
Product Owner, Command Center Dashboard

---

END OF EMAIL TEMPLATE
