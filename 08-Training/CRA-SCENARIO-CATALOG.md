# CRA Scenario Catalog: Robust Practice Cases

Use this catalog with `/simulate` or the Scenario Simulator prompt. These scenarios are deliberately incomplete in realistic ways: the CRA must identify what is known, what is missing, and who needs to be consulted before acting.

## How to Run a Scenario

Ask Claude:

```text
/simulate [scenario name]
```

For a full practice session:

```text
/simulate a 5-scenario CRA judgment session using the scenario catalog
```

Claude should present one scenario at a time, wait for your response, and then provide feedback before continuing.

## Scenario Safety Rules

For every scenario, Claude should:

- Use fictional identifiers such as Patient 001 and Site 101.
- Never request or invent patient-identifiable information.
- Clearly label fictional dates, values, and facts.
- Ground study-specific decisions in uploaded documents.
- Never invent a protocol threshold, reporting deadline, or company process.
- Separate an educational exercise from a real operational decision.
- Ask what information is missing before recommending follow-up.
- Identify when the medical monitor, sponsor, investigator, safety team, or manager may need to be consulted.
- Avoid giving medical advice or making a final safety determination on behalf of qualified personnel.

## Scenario Difficulty Levels

### Level 1: Recognition

The important rule is present in the provided information. Practice identifying the requirement and citing the source.

### Level 2: Missing Information

Several plausible actions exist, but an important fact is missing. Practice asking targeted questions before acting.

### Level 3: Competing Priorities

Patient safety, data quality, timelines, and site relationships pull in different directions. Practice prioritizing risk.

### Level 4: Ambiguous Judgment

The protocol does not fully resolve the situation. Practice documenting uncertainty, escalating appropriately, and avoiding assumptions.

### Level 5: Multi-Study or Multi-Document Complexity

The situation includes an amendment, conflicting documents, or two studies with similar procedures. Practice preventing cross-study contamination.

## Scenario Library

### 1. Eligibility Discovered After Enrollment

**Situation:** A participant was enrolled, but a source document later suggests an exclusion criterion may have been present at baseline.

**Test:** What evidence must be reviewed? What is confirmed versus suspected? Who should be notified? What should not be concluded without medical or sponsor review?

### 2. Visit Outside the Window

**Situation:** A required visit occurred four days outside the allowed window. The site says the patient was unavailable and all assessments were completed.

**Test:** Check the exact window, identify affected endpoints and safety assessments, distinguish a deviation from a scheduling note, and define follow-up questions.

### 3. Missing Primary Endpoint Assessment

**Situation:** Most visit data are complete, but the primary endpoint assessment is missing for one participant.

**Test:** Determine whether the assessment can be recovered, what the protocol says about missed assessments, how the issue affects data quality, and what must be documented.

### 4. Safety Event With Conflicting Dates

**Situation:** The source note, EDC entry, and safety report show different event onset dates.

**Test:** Reconcile the source hierarchy, avoid changing medical facts, identify the safety reporting implications, and escalate unresolved discrepancies.

### 5. Repeated Site Process Error

**Situation:** The same visit procedure has been missed at three consecutive visits despite prior retraining.

**Test:** Move beyond repeating training. Assess root cause, risk, CAPA or action-plan needs, verification of effectiveness, and escalation thresholds.

### 6. Investigational Product Accountability Mismatch

**Situation:** Dispensed and returned quantities do not reconcile with the participant's dosing record.

**Test:** Separate arithmetic, documentation, adherence, storage, dispensing, and potential product-loss questions. Do not infer diversion or noncompliance without evidence.

### 7. Blinding Risk

**Situation:** A site staff member may have seen treatment assignment information in an email or source document.

**Test:** Protect the blind, identify who needs to know, distinguish suspected from confirmed unblinding, and follow the study-specific escalation path.

### 8. Amendment Transition Error

**Situation:** The site used the new consent form but appears to have followed an old visit schedule for one participant.

**Test:** Establish effective dates, participant applicability, retraining status, affected data, and the current approved requirement.

### 9. Competing Documents

**Situation:** The protocol and a study manual use different visit windows for the same timepoint.

**Test:** Do not choose the more convenient rule. Compare versions, identify document hierarchy, record the conflict, and formulate a focused clarification question.

### 10. Two Studies, Similar Procedures

**Situation:** A coordinator uses Study A's laboratory kit instructions for Study B because the studies have similar visit names.

**Test:** Detect cross-study contamination, identify affected participants and samples, contain further use, and determine what must be verified.

### 11. Protocol Versus Local Practice

**Situation:** The site follows a routine clinical workflow that differs from the protocol's required sequence.

**Test:** Distinguish standard care from study-required procedures and assess patient safety, endpoint validity, and deviation implications.

### 12. Remote Monitoring Limitation

**Situation:** A remote review cannot access a source document needed to verify a high-risk endpoint.

**Test:** Prioritize what can be reviewed remotely, document the limitation, avoid claiming verification, and plan appropriate follow-up.

### 13. Data Query Under Time Pressure

**Situation:** A database lock deadline is approaching, but a query response conflicts with source documentation.

**Test:** Do not optimize for speed at the expense of data integrity. Identify the authoritative source, required clarification, and escalation route.

### 14. Investigator Delegation Gap

**Situation:** A procedure was performed by a staff member whose delegation or training record is incomplete.

**Test:** Verify the delegation timeline, training evidence, procedure requirements, participant impact, and documentation gaps.

### 15. Screening Log and Enrollment Mismatch

**Situation:** The screening log lists more failures than the site reported in its enrollment update.

**Test:** Reconcile the populations and dates, protect confidentiality, identify reporting implications, and ask precise questions.

### 16. Compare-Studies Mix-Up

**Situation:** Two studies use the same disease area and similar visit names, but their eligibility thresholds and safety follow-up rules differ.

**Test:** Use `/compare_studies` to create a study-specific difference matrix, then explain which differences are most likely to cause operational errors.

## Required Debrief Format

After the CRA responds, Claude should provide:

1. **What you identified correctly**
2. **What information was missing**
3. **What assumptions could create risk**
4. **Protocol or document evidence**
5. **Possible next steps**, clearly labeled as options rather than orders
6. **Who may need to be consulted**
7. **Risk classification:** patient safety, data quality, compliance, operations, or multiple
8. **A harder variation** that changes one important fact
9. **One transferable principle**

## Facilitator Prompt

```text
Use the CRA Scenario Catalog to run a realistic, source-grounded practice session.

Choose one scenario at a time. Do not reveal the answer before I respond. Use
fictional identifiers only. After my response, evaluate my reasoning, identify
missing information and unsafe assumptions, cite the relevant study documents,
separate confirmed facts from inferences, identify appropriate escalation or
consultation, and present a harder variation. Do not invent protocol rules.
After five scenarios, summarize my strengths, recurring gaps, and recommended
next practice area.
```
