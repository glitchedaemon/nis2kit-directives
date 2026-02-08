# Security Directive: sec01 - Multi-Factor Authentication (MFA)

**Checklist Item ID:** `sec01`  
**Category:** Security  
**NIS2 Reference:** Article 21(2)(a) - Risk Management Measures  
**Compliance Requirement:** Multi-factor authentication must be implemented on all critical systems and privileged accounts.

---

## Compliance Criteria

### ✅ COMPLIANT if:
1. **MFA is actively enforced** on all administrator/privileged accounts
2. **At least 2 factors** are required (something you know + something you have/are)
3. **Coverage includes:**
   - Cloud admin consoles (AWS, Azure, Google Cloud)
   - VPN/Remote access systems
   - Financial systems
   - User management platforms
4. **Evidence shows:** Configuration screenshots, policy documents, or audit logs proving enforcement

### ❌ NON-COMPLIANT if:
- MFA is "planned" but not implemented
- Only applies to some accounts (partial deployment)
- Uses weak methods (SMS-only without hardware/app tokens)
- No documented enforcement policy
- Evidence shows optional/voluntary MFA

### ⚠️ PARTIAL if:
- MFA is implemented but coverage is incomplete (<80% of privileged accounts)
- Policy exists but enforcement is inconsistent
- Missing documentation of MFA methods used

---

## AI Analysis Instructions

**When analyzing uploaded evidence:**

1. **Extract** mentions of:
   - "multi-factor", "MFA", "2FA", "two-factor"
   - "authentication", "access control"
   - Specific vendors: "Duo", "Okta", "Microsoft Authenticator", "YubiKey"

2. **Score based on:**
   - **100**: Full MFA deployment with proof (screenshots, policy + audit logs)
   - **60-80**: Policy exists + partial evidence of implementation
   - **30-50**: MFA mentioned in plans but no proof of active use
   - **0-20**: No mention or explicitly stated as "not implemented"

3. **Generate feedback:**
   - **Gaps:** List which critical systems lack MFA
   - **Recommendations:** Suggest free/low-cost MFA solutions (Microsoft Authenticator, Google Authenticator)
   - **Next Steps:** "Enable MFA on [specific system], document configuration in security policy"

4. **Red Flags (Auto Non-Compliant):**
   - Document states "MFA not required"
   - Only SMS-based MFA (phishing vulnerable)
   - No MFA on cloud admin accounts

---

## Example Evidence Scenarios

**Scenario A: Compliant**
> "Our MFA policy requires all administrators to use Duo Security. Attached: Duo admin panel showing 15/15 users enrolled + quarterly audit log."

**Scenario B: Non-Compliant**
> "We plan to implement MFA in Q2 2026. Currently using password-only authentication."

**Scenario C: Partial**
> "MFA enabled on AWS root account and 3 IAM admins. Remaining 5 developer accounts pending enrollment."

---

## Metadata
- **Severity:** HIGH (Direct NIS2 requirement)
- **Effort to Comply:** LOW (Free tools available, ~2 hours setup)
- **Common Pitfall:** Treating MFA as "optional" for non-admin users (acceptable but must cover ALL privileged access)
