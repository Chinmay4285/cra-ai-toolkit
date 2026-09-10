# Inconsistency Detector: Find Conflicts Between Documents

## PURPOSE
Systematically compare multiple study documents to identify conflicts, contradictions, and inconsistencies that need clarification.

## WHEN TO USE
When you have multiple study documents (protocol, ICF, SAP, monitoring plan, etc.) and want to ensure they're aligned.

## WHAT TO PROVIDE
- Your study context
- All documents to compare (at minimum: protocol + one other document)
- Specific topics to compare (or "all topics")

## EXPECTED OUTPUT
Table of inconsistencies with evidence from both documents, severity assessment, and recommendations.

---

# INCONSISTENCY DETECTOR PROMPT

```
COPY FROM HERE
========================================================================================

You are systematically comparing multiple study documents to identify conflicts, 
contradictions, and inconsistencies.

COMPARISON METHODOLOGY:

For each major topic, check:
- Visit schedule and timing
- Inclusion/exclusion criteria
- Endpoint definitions
- Procedures and assessments
- Safety monitoring
- Blinding status
- Treatment duration and doses
- Study objectives
- CRA/Site responsibilities
- Prohibited medications
- Data requirements

FOR EACH INCONSISTENCY FOUND:

1. WHAT'S DIFFERENT?
   Document A states: [Exact quote]
   Document B states: [Exact quote]

2. WHERE ARE THEY?
   - Document A: [Name, Section, Page]
   - Document B: [Name, Section, Page]

3. WHY THIS MATTERS
   - Clinical impact: [If relevant]
   - CRA impact: [How does this affect CRA work]
   - Site impact: [How would sites interpret this]
   - Compliance impact: [If relevant]

4. SEVERITY ASSESSMENT
   
   CRITICAL:
   - Affects patient safety
   - Affects inclusion/exclusion
   - Affects primary endpoint
   - Affects regulatory compliance
   - Requires immediate clarification
   
   IMPORTANT:
   - Affects data quality or study conduct
   - Could cause site confusion
   - Should be clarified before monitoring
   
   MINOR:
   - Affects wording or clarity only
   - Doesn't affect actual procedures
   - Could be editorial difference

5. LIKELY EXPLANATION
   - Which document is more likely correct?
   - Is this an error or intentional difference?
   - Is there a reason for the difference?

6. RECOMMENDATION
   - Should this be flagged to Sponsor?
   - Should sites be notified?
   - Does it need amendment?
   - Can it be clarified in Study Manager guidance?

FINAL SUMMARY TABLE:

| Inconsistency | Documents | Section | Severity | Impact | Recommendation |
|---|---|---|---|---|---|
| [Issue] | [Doc A vs Doc B] | [Topics] | [C/I/M] | [Impact summary] | [Action] |

========================================================================================
END PROMPT
```

---

## HOW TO USE THIS ANALYSIS

**Before Monitoring Starts:**
- Compare protocol, ICF, and monitoring plan
- Identify inconsistencies before sites see them
- Resolve with Sponsor/Study Manager

**Before Your First Visit:**
- Know which inconsistencies are known issues
- Know how to explain them to sites if needed
- Have answers ready for site questions

**During Monitoring:**
- If site raises an inconsistency, you're prepared
- You can explain or escalate appropriately

**Document Management:**
- Track all known inconsistencies
- Update when amendments occur
- Share with other sites if relevant

---

## COMMON INCONSISTENCIES TO WATCH FOR

- **Visit windows:** Protocol says ±3 days, but monitoring plan shows ±7 days
- **Eligibility:** Age 21-65 in protocol, but ICF says 18+
- **Endpoints:** Primary endpoint defined differently in protocol vs. SAP
- **Procedures:** Protocol requires lab on day 1, SAP says baseline labs
- **Timing:** SAP shows visit at week 12, but protocol says week 14
- **Blinding:** Protocol says double-blind, but investigator instructions clarify site is unblinded
- **Safety reporting:** Different timelines in protocol vs. monitoring plan

---

## WHEN TO FLAG AN INCONSISTENCY TO SPONSOR

**MUST FLAG IMMEDIATELY:**
- Safety-related differences
- Efficacy/endpoint definition differences
- Eligibility criteria differences (protocol vs. ICF)
- Treatment/dose differences
- Any potential regulatory concern

**SHOULD FLAG SOON:**
- Visit schedule/window differences
- Data collection procedure differences
- Monitoring frequency differences
- CRA responsibility differences

**CAN CLARIFY WITH STUDY MANAGER:**
- Wording differences (same meaning)
- Editorial inconsistencies
- Format differences

---

## INTEGRATING WITH YOUR STUDY BRAIN

In a separate conversation (or your Study Brain), ask:
- "Compare the protocol and ICF - find inconsistencies"
- "Check the monitoring plan against the protocol"
- "Are there conflicts between how the SAP and protocol define the primary endpoint?"

Include both documents in the conversation.

---

## WHEN TO USE RELATED PROMPTS

- **For detailed document analysis:** Use `/05-Document-Intelligence/protocol-analyzer.md`
- **For finding red flags:** Use `/05-Document-Intelligence/red-flags.md`
- **For finding gaps:** Use `/05-Document-Intelligence/missing-information.md`
- **For creating requirements matrix:** Use `/06-Cross-Document/requirement-matrix.md`
