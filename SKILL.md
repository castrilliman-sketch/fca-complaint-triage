---
name: fca-complaint-triage
description: Triage incoming UK consumer credit customer emails for FCA DISP compliance, CONC 7 vulnerability/arrears indicators, and 1 January 2027 COM001 regulatory reporting.
---

# FCA Consumer Credit Complaint & Arrears Triage (DISP / CONC 7 / COM001)

When asked to triage or process a customer email, complaint, or dispute:

1. **DISP Complaint Identification:** Determine whether the message meets the FCA DISP definition of a complaint (any oral or written expression of dissatisfaction, whether justified or not, alleging financial loss, material distress, or material inconvenience).
2. **CONC 7 & Vulnerability Screening:** Flag any indicators of vulnerability (health issues, bereavement, mental capacity, financial hardship, inability to pay, domestic abuse) or CONC 7 arrears/forbearance triggers.
3. **COM001 Taxonomy Mapping (Effective 1 Jan 2027):** Classify the primary product/service and root-cause category aligned with the FCA consolidated COM001 complaints return schema, noting whether it qualifies for Summary Resolution Communication (SRC) within 3 business days or requires a full 8-week formal DISP timeline.
4. **Statutory Deadlines:** Calculate from the date received (UK business days):
   - Prompt written acknowledgement date
   - 3-business-day SRC window
   - 4-week holding letter milestone
   - 8-week Final Response Letter (FRL) deadline
5. **Human-in-the-Loop Draft:** Output a structured **Complaints Log Row** (CSV/Markdown ready) and a **Draft Acknowledgement / SRC Letter** in plain English.
6. **Mandatory Guardrail:** Never send emails automatically. Always label drafts `[DRAFT — REQUIRES COMPLIANCE OFFICER APPROVAL]`.
