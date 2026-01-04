# Management Approval (Article 20.1 - Governance)

**Legal Basis:** NIS2 Directive Article 20(1) - "Management body shall approve risk management measures"

**Requirement:** 
Senior management must formally approve cybersecurity risk management measures and allocate appropriate resources.

**Expected Evidence:**
- Board resolution, executive memo, or management committee minutes
- Document dated within last 12 months (annual review required)
- Explicit mention of "NIS2", "cybersecurity budget", or "risk management program"
- Signature/approval from C-level executive (CEO, CTO, CISO, CFO) or Board of Directors

**Pass Criteria (AI must verify ALL):**
1. **Approval Authority:** Document signed by CEO, CTO, CISO, CFO, or Board
2. **Timeframe:** Date visible and < 365 days from analysis date
3. **Scope:** References cybersecurity measures, budget allocation, or compliance program
4. **Commitment:** Contains approval language ("Board approves", "Management authorizes", "We commit to...")

**Fail Indicators:**
- Generic policy without specific approval
- No visible date or date > 12 months old
- Employee-level signoff (not C-suite/Board authority)
- No mention of resources or budget

**Scoring Guidance:**
- 90-100: Perfect compliance (all criteria + specific budget amounts)
- 80-89: Compliant (all criteria met)
- 60-79: Partial (missing 1-2 minor criteria, e.g., no date but strong approval)
- 0-59: Non-compliant (missing signatures, outdated, or generic policy)

**AI Threshold:** Score ≥ 80 = `ai_compliant: true`

---

**Remediation Guidance:**
If non-compliant, advise client to:
1. Schedule Board/Executive meeting to review cybersecurity program
2. Prepare 1-page summary of NIS2 obligations and required budget
3. Obtain signed resolution/memo with current date
4. Reference Article 20.1 explicitly in approval document
