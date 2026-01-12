# Disk Encryption & Data Protection (BitLocker - Windows)

## Objective
Implement and validate full-disk encryption to protect data at rest on a Windows system, aligned with recognized security frameworks and audit expectations.

---

## Environment
- Windows virtual machine (isolated lab)
- BitLocker enabled without TPM
- Local administrative access
- No production or real user data

---

## Security Focus 
- Data-at-rest protection
- Cryptographic key management
- Control validation and audit evidence generation

---

## Tasks Performed
- Enabled BitLocker full-disk encryption on the system drive without TPM
- Configured appropriate key protectors
- Verified encryption status using command-line utilities
- Reviewed recovery key handling and secure storage considerations
- Mapped technical controls to security frameworks

 ---
 
 ## Validation & Evidence
 Encryption status and key protectors were verified with:

```powershell
manage-bde -status
```

---

## Compliance alignment
- **ISO/IEC 27001**: A.10 - Cryptographic controls
- **NIST SP 800-53**: SC-12, SC-28 - Cryptographic key establishment and protection
- **CIS Controls**: Control 3 - Data Protection

---

## Risk & Security Considerations
- Importance of secure recovery key storage
- Risks associated with improper key handling
- Impact of disk encryption on incident response and asset disposal

---

## Key Takeaways
- Disk encryption is a foundational control for protecting sensitive data
- Command-line verification is critical for audit compliance
- Technical controls must be paired with documented processes

---

## Skills Demonstrated
- Disk encryption implementation
- Command-line security validation
- Cryptographic control awareness
- Compliance and audit mapping
