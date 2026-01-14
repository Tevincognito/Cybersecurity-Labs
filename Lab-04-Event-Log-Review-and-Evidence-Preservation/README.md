# Event Log Review & Evidence Preservation (Windows)

## Objective
Review Windows security event logs to identify authentication activity and preserve log evidence in a forensically sound manner to support investigations and audit requirements.

---

## Environment
- Windows virtual machine (isolated lab)
- Windows Security Event Log
- Event Viewer
- Local administrator account
- No production or real user data

---

## Security Focus
- Security event analysis
- Incident detection and investigation
- Evidence integrity and preservation
- Audit and compliance readiness

---

## Tasks Performed
- Reviewed Windows Security logs for authentication activity
- Identified successful and failed logon events
- Analyzed event timestamps, user accounts, and source systems
- Exported security logs in native format to preserve integrity
- Documented evidence handling considerations

---

## Validation & Evidence
Authentication activity was reviewed using the following event IDs:
- **Event ID 4624** – Successful logon
- **Event ID 4625** – Failed logon

Security logs were exported in native `.evtx` format to preserve integrity and support forensic analysis.

---

## Compliance Alignment
- **ISO/IEC 27001**: A.12 – Logging and monitoring
- **NIST SP 800-53**: AU-7, IR-4 – Audit reduction and incident handling
- **CIS Controls**: Control 8 – Audit Log Management

---

## Risk & Security Considerations
- Failure to preserve logs may hinder investigations
- Improper handling can compromise evidence integrity
- Incomplete logging reduces incident detection capability

---

## Key Takeaways
- Security logs provide critical visibility into system activity
- Evidence preservation is essential for investigations and audits
- Native log formats support integrity and chain-of-custody requirements

---

## Skills Demonstrated
- Windows event log analysis
- Security incident investigation
- Evidence preservation techniques
- Audit and compliance support
