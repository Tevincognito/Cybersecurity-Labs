# Local Security Policy & Account Hardening (Windows)

## Objective
Configure and validate local authentication policies to enforce a secure baseline, reduce credential-based attack risk, and support audit and compliance requirements.

---

## Environment
- Windows virtual machine (isolated lab)
- Local administrator account
- Local Security Policy (secpol.msc)
- No production or real user data

---

## Security Focus
- Authentication hardening
- Password policy enforcement
- Baseline security configuration
- Audit evidence generation

---

## Tasks Performed
- Reviewed and configured password policies (length, age, history)
- Evaluated account lockout policy settings
- Distinguished audit requirements vs enforcement controls
- Verified effective policy configuration using command-line tools
- Documented baseline settings as audit-ready evidence

---

## Validation & Evidence
Password and account policies were validated using:

```powershell
net accounts
```

---

## Compliance Alignment
- **ISO/IEC 27001**: A.9 - Access control
- **NIST SP 800-53**: IA-5 - Authenticator management
- **CIS Controls**: Control 5 - Account Management

---

## Risk & Security Considerations
- Weak password policies increase brute-force and credential-stuffing risk
- Inconsistent enforcement creates audit and compliance gaps
- Misconfigured lockout policies may cause denial-of-service conditions

---

## Key Takeaways
- Authentication baselines are foundational security controls
- Verification is as important as configuration
- Clear documentation supports audits and incident response

---

## Skills Demonstrated
- Authentication policy hardening
- Windows security baseline configuration
- Command-line policy validation
- Audit and compliance mapping
