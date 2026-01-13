# Account Lockout & Audit Logging Configuration (Windows)

## Objective
Implement and validate account lockout and audit logging controls to prevent brute-force attacks, detect suspicious activity, and support incident response and audit requirements.

---

## Environment
- Windows virtual machine (isolated lab)
- Local administrator account
- Local Security Policy (secpol.msc)
- Windows Security Event Log
- No production or real user data

---

## Security Focus
- Preventive security controls (account lockout)
- Detective security controls (audit logging)
- Authentication monitoring
- Audit readiness

---

## Tasks Performed
- Configured account lockout thresholds and durations
- Enabled auditing for logon events, account management, and policy changes
- Reviewed default vs hardened audit settings
- Verified audit policy configuration using command-line tools
- Identified and remediated audit coverage gaps

---

## Validation & Evidence
Audit policy configuration was validated using:

```powershell
auditpol /get /category:*
```
Authentication events were reviewed in the Windows Security log, including:
- **Event ID 4624** - Successful logon
- **Event ID 4625** - Failed logon

---

## Compliance Alignment 
- **ISO/IEC 27001**: A.12 - Logging and monitoring
- **NIST SP 800-53**: AU-2, AU-6 - Audit events and review
- **CIS Controls**: Control 8 - Audit Log Management

---

## Risk & Security Considerations
- Lack of account lockout controls increases brute-force attack risk
- Insufficient logging reduces visibility into security incidents
- Excessive lockout settings may impact availability

---

## Key Takeaways
- Preventive and detective controls work together to reduce risk
- Logging without review provides limited security value
- Proper audit configuration supports detection, response, and compliance

---

## Skills Demonstrated
- Account lockout configuration
- Windows audit policy management
- Security event analysis
- Preventive vs detective control identification
- Audit and compliance mapping


