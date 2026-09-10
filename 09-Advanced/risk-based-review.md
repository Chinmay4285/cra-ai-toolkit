# Risk-Based Review: Identify Potential Issues and Concerns

## PURPOSE
Perform a systematic risk assessment of your study to identify potential safety, compliance, data quality, and operational risks. Categorize findings by severity.

## WHEN TO USE
When preparing for monitoring visits, analyzing site performance, or looking for hidden concerns. Great for: risk-based monitoring planning, safety assessment, compliance verification.

## WHAT TO PROVIDE
- Your study context
- Your protocol
- Optionally: previous monitoring data, site-specific information, or which aspect of the study to focus on

## EXPECTED OUTPUT
Systematic risk assessment organized by severity (low/medium/high), with evidence, impact, and recommended verification for each finding.

---

# RISK-BASED REVIEW PROMPT

```
COPY FROM HERE
========================================================================================

You are conducting a risk-based review to identify potential issues in this study.

RISK ANALYSIS FRAMEWORK:

For each potential risk, assess:

1. RISK IDENTIFICATION
   - What is the potential risk or concern?
   - Where in the protocol does this appear?
   - Why is this a risk?

2. SEVERITY CATEGORIZATION
   
   LOW RISK:
   - Unlikely to occur or minimal impact if it does
   - Can be managed through routine monitoring
   - Non-critical to study success or patient safety
   
   MEDIUM RISK:
   - Could occur and has meaningful impact
   - Requires specific monitoring or prevention
   - Important for data quality or compliance
   
   HIGH RISK:
   - Likely impact on patient safety, study integrity, or compliance
   - Requires robust prevention and monitoring
   - Could lead to protocol violations or safety events
   - Requires escalation if identified

3. EVIDENCE & REASONING
   - What in the protocol suggests this risk?
   - Why would this be a problem on this particular study?
   - What historical data supports this concern?
   - What site factors might contribute?

4. POTENTIAL IMPACT
   - Patient safety impact: [None / Minor / Major]
   - Data quality impact: [None / Minor / Major]
   - Compliance impact: [None / Minor / Major]
   - Study success impact: [None / Minor / Major]

5. MONITORING STRATEGY
   - How should this be monitored?
   - What specifically should the CRA look for?
   - What questions should be asked?
   - What source documents should be verified?
   - How often?

6. PREVENTION STRATEGY
   - What can be done BEFORE the risk occurs?
   - What site training is needed?
   - What procedures/tools would help?
   - What investigator communication is needed?

7. ESCALATION CRITERIA
   - At what point should this be escalated?
   - Who should be notified?
   - What is the escalation process?

RISK CATEGORIES:

Organize findings by type:

A. PATIENT SAFETY RISKS
   - [Risk 1]: [Categorization] - [Summary]
   - [Risk 2]: [Categorization] - [Summary]

B. DATA QUALITY RISKS
   - [Risk 1]: [Categorization] - [Summary]
   - [Risk 2]: [Categorization] - [Summary]

C. COMPLIANCE/PROTOCOL RISKS
   - [Risk 1]: [Categorization] - [Summary]
   - [Risk 2]: [Categorization] - [Summary]

D. OPERATIONAL/ENROLLMENT RISKS
   - [Risk 1]: [Categorization] - [Summary]
   - [Risk 2]: [Categorization] - [Summary]

E. DESIGN-SPECIFIC RISKS
   - [Risk 1 specific to this study's design]: [Categorization] - [Summary]
   - [Risk 2]: [Categorization] - [Summary]

COMPREHENSIVE RISK TABLE:

| Risk | Severity | Evidence | Impact | Monitor | Prevent | Escalate If |
|---|---|---|---|---|---|---|
| [Risk 1] | [L/M/H] | [Protocol basis] | [Impact summary] | [How] | [How] | [Trigger] |

FINAL RECOMMENDATIONS:

1. High-Risk Priorities: [List top 3-5 risks requiring immediate attention]
2. CRA Focus Areas: [Where to concentrate monitoring efforts]
3. Site Communication: [What to discuss with investigator/coordinator]
4. Study Modifications: [If applicable, modifications to reduce risk]
5. Timeline: [When to address each risk category]

========================================================================================
END PROMPT
```

---

## WHAT RISKS TO LOOK FOR

**Patient Safety Risks:**
- Vulnerable populations not adequately protected
- Safety monitoring gaps
- Procedures that could harm if done incorrectly
- Drug interactions with common medications
- Special populations (pregnancy, organ dysfunction)

**Data Quality Risks:**
- Complex assessments prone to error
- Subjective endpoint measurements
- Visit windows too tight
- Multiple assessments in one visit (time constraints)
- Assessment timing constraints (e.g., must be before dosing)

**Compliance Risks:**
- Complex eligibility criteria
- Multiple prohibited medications
- Challenging visit windows
- Blinding procedures that are hard to maintain
- Investigator or site coordination needed

**Enrollment Risks:**
- Restrictive eligibility criteria
- Difficult patient population to reach
- Invasive procedures deterring enrollment
- Seasonal/geographic challenges
- Screen failure risk

**Study Design Risks:**
- Washout periods that are difficult
- Unusual endpoints hard to measure
- Treatment duration too long
- Visit schedule too frequent
- Placebo with active comparator (sites want better drug)

---

## HOW TO USE YOUR RISK ASSESSMENT

**During Site Selection:**
- Use risk assessment to identify high-risk investigator/site capability gaps
- Provide extra training at high-risk sites

**Visit Planning:**
- Prioritize monitoring time to high-risk areas
- Develop targeted verification procedures for medium/high risks

**Site Communication:**
- Share high-risk areas with investigators
- Emphasize importance of specific procedures
- Offer support for challenging requirements

**Ongoing Monitoring:**
- Track whether high-risk areas actually occur
- Adjust monitoring based on reality vs. prediction
- Escalate when predicted risks materialize

**Lessons Learned:**
- After monitoring, note which predicted risks actually occurred
- Update your risk assessment based on reality
- Share learnings with other sites

---

## RISK ADJUSTMENT BASED ON SITE PERFORMANCE

Initial risk assessment is theoretical. Adjust based on:
- **Site's clinical expertise:** Experienced sites can handle complex procedures
- **Site's GCP knowledge:** Well-trained sites less likely to have compliance issues
- **Previous study participation:** Repeating study → know what to expect
- **Demonstrated performance:** If site excels, reduce monitoring of that area
- **Historical issues:** If site struggled before, increase monitoring

---

## RED FLAGS DURING MONITORING

Watch for these triggers that a predicted risk is becoming real:

- ⚠️ First data discrepancy between source and EDC on a safety parameter
- ⚠️ Patient enrolled who "almost" met eligibility (borderline)
- ⚠️ Procedure documented but source documentation missing
- ⚠️ Repeated deviation on the same requirement
- ⚠️ Site staff confusion about a procedure
- ⚠️ Missed assessment on a safety-critical timepoint
- ⚠️ Site asking if they "have to" do a procedure (compliance risk)

When these occur, escalate your monitoring for that risk area.

---

## INTEGRATING WITH YOUR STUDY BRAIN

In your Study Brain conversation, ask:
- `/find risks in [section of protocol]`
- `/risk assessment of this study`
- `What are the high-risk areas I need to focus on?`

Claude will identify study-specific risks using your protocol.

---

## WHEN TO USE RELATED PROMPTS

- **For identifying gaps:** Use `/05-Document-Intelligence/missing-information.md`
- **For finding inconsistencies:** Use `/06-Cross-Document/inconsistency-detector.md`
- **For root cause analysis:** Use `/09-Advanced/root-cause-analysis.md`
- **For monitoring visits:** Use `/07-CRA-Workflow/monitoring-visit-prep.md`
