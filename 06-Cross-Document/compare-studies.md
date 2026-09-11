# /compare_studies: Compare Two Studies

## Purpose

Use this skill to compare two different clinical studies in a detailed, source-grounded way. The goal is to show what the studies share, how they differ, and what those differences mean for CRA work.

This skill is for comparing study-level designs, protocols, procedures, populations, endpoints, operational requirements, and risks. It is not a substitute for the current approved protocol, sponsor guidance, medical review, or company procedures.

## How to Use It in Claude

1. Upload the current approved documents for both studies to your Claude Project, or clearly identify which uploaded files belong to each study.
2. Label the studies before asking for the comparison. For example:
   - Study A: Protocol ABC-101, Version 3.0
   - Study B: Protocol XYZ-202, Version 2.1
3. Type:

```text
/compare_studies Study A and Study B
```

You can narrow the request:

```text
/compare_studies Study A and Study B, focusing on visit schedules and monitoring risks
```

If the studies or document versions are unclear, ask Claude to identify the ambiguity before comparing them.

## Required Behavior

When this command is used, Claude must:

1. Confirm the two studies and document versions being compared.
2. List the source documents used for each study.
3. State any missing documents, unclear labels, or version limitations before analysis.
4. Use only the supplied study documents for study-specific claims unless the user explicitly asks for external context.
5. Cite the source document, section, and page when available.
6. Separate findings into:
   - **Confirmed:** directly stated in a source document.
   - **Inferred:** a reasonable conclusion that is not explicitly stated.
   - **Unknown:** not available in the provided documents.
   - **Needs verification:** appears inconsistent, outdated, or dependent on a current approved version.
7. Avoid treating one study's requirements as if they apply to the other study.
8. Flag conflicts between documents instead of silently resolving them.
9. Explain practical implications without prescribing actions beyond the user's authority.

## Comparison Framework

Compare the studies across the following areas. If an area is not available, mark it as **Not found in provided documents** rather than guessing.

### 1. Study Identity and Status

- Protocol number and study title
- Sponsor or program, if provided
- Phase and study status
- Document versions and effective dates
- Investigational product or intervention
- Therapeutic area and condition

### 2. Scientific and Clinical Design

- Primary objective
- Secondary and exploratory objectives
- Study type: interventional or observational
- Randomization and allocation
- Blinding or masking
- Control or comparator
- Treatment arms and dosing strategy
- Study duration and follow-up
- Sample size and enrollment targets
- Key stratification or subgroups

### 3. Participant Population

- Target population
- Age range and demographic requirements
- Disease severity or stage
- Inclusion criteria
- Exclusion criteria
- Prior or concomitant treatment requirements
- Washout periods
- Re-screening rules
- Discontinuation or withdrawal criteria

### 4. Visit and Assessment Schedule

- Screening and baseline requirements
- Visit names and timing
- Visit windows
- Required assessments at each visit
- Laboratory, imaging, ECG, or other procedures
- Patient-reported outcomes
- Safety assessments
- End-of-treatment and follow-up visits
- Missed visit or out-of-window handling

### 5. Endpoints and Data Requirements

- Primary endpoint definitions
- Secondary endpoint definitions
- Exploratory endpoints
- Measurement instruments and timing
- Safety variables
- Data collection requirements
- Source data expectations
- Query and reconciliation implications

### 6. Investigational Product and Accountability

- Administration route and schedule
- Dose modification rules
- Storage and temperature requirements
- Dispensing and return requirements
- Accountability records
- Preparation or handling requirements
- Adherence assessment
- Prohibited medications or procedures

### 7. Safety and Reporting

- Adverse event collection period
- Serious adverse event requirements
- Special safety events
- Pregnancy reporting
- Laboratory or vital-sign thresholds
- Escalation timelines
- Emergency unblinding rules
- Safety follow-up expectations

### 8. Operational and CRA Implications

- Monitoring intensity and likely focus areas
- Source data verification or review expectations
- Essential documents
- Training requirements
- Site staff responsibilities
- Central or remote data review
- Risk indicators and issue escalation
- Common compliance vulnerabilities

## Required Output Format

Use this structure unless the user asks for a different format.

### 1. Comparison Scope

- Study A:
- Study B:
- Documents reviewed:
- Documents missing or unclear:
- Version and date limitations:

### 2. Executive Summary

Provide 5-10 high-value findings:

- The most important similarities
- The most important differences
- Differences likely to affect patient safety
- Differences likely to affect data quality
- Differences likely to affect site operations or monitoring

### 3. Similarities

Use a table:

| Area | Shared Feature | Evidence | CRA Relevance |
|---|---|---|---|
| Design, population, visits, endpoints, safety, or operations | What both studies share | Study A and Study B sources | Why the similarity matters |

Only include a similarity when it is supported by both studies. Explain meaningful differences in wording or thresholds even when the high-level topic is shared.

### 4. Differences

Use a detailed table:

| Area | Study A | Study B | Evidence | Practical Impact |
|---|---|---|---|---|
| Topic | Requirement or feature in Study A | Requirement or feature in Study B | Sources and sections | Effect on CRA/site/patient/data work |

Prioritize differences that could cause a team member to accidentally apply the wrong study requirement.

### 5. Detailed Analysis by Area

Explain the comparison area by area. Include:

- What changed or differs
- Why the difference may matter
- What a CRA should pay attention to
- What should be verified with the sponsor, medical monitor, or study team
- Any dependency on document version or local procedure

Do not invent rationale. If the reason is not stated, label it as unknown and describe only the operational consequence that follows from the documented difference.

### 6. CRA Risk and Attention Matrix

Use a prioritized table:

| Priority | Difference or similarity | Risk type | Why it matters | Verification or follow-up |
|---|---|---|---|---|
| High, medium, or low | Finding | Patient safety, data quality, compliance, or operations | Specific concern | Appropriate next check |

Mark a finding **High** only when the source documents support a potentially significant safety, compliance, data integrity, or operational consequence.

### 7. Practical Checklist

Create two separate checklists:

**Before working on both studies**
- Confirm current approved versions.
- Confirm which requirements apply to each study.
- Separate study-specific templates, trackers, and reference materials.
- Review differences in eligibility, visits, endpoints, safety, and escalation.

**During monitoring or study work**
- Verify the correct protocol and study documents are being used.
- Check study-specific visit windows and assessments.
- Confirm study-specific safety and deviation processes.
- Document unresolved differences and obtain appropriate clarification.

Tailor the checklist to the findings. Do not present generic steps as study requirements.

### 8. Questions to Resolve

List focused questions for the sponsor, project manager, medical monitor, or site team. Include the source of the uncertainty and why clarification matters.

### 9. Final Limitations

State what was not available, what could not be confirmed, and which findings require review against the current approved documents or company procedures.

## Optional Comparison Modes

If the user specifies a mode, adapt the output:

- **`/compare_studies A and B --quick`**: executive summary, top similarities, top differences, and top risks.
- **`/compare_studies A and B --cra`**: emphasize monitoring, site operations, source data, deviations, and questions.
- **`/compare_studies A and B --clinical`**: emphasize population, intervention, assessments, endpoints, and safety.
- **`/compare_studies A and B --visits`**: focus on visit schedule, windows, procedures, and missed-visit handling.
- **`/compare_studies A and B --documents`**: focus on document versions, conflicts, missing information, and traceability.

These modes change the emphasis, not the source-grounding rules.

## High-Value Comparison Scenarios

Use these focused scenarios when the user wants more than a generic side-by-side summary:

### Similar Studies, Different Eligibility

Compare two studies in the same disease area and identify thresholds, prior-treatment rules, washout periods, and exclusion criteria that could lead to cross-study enrollment errors.

### Same Visit Name, Different Requirements

Compare visits with the same label, such as "Baseline" or "Week 12," and show differences in timing, windows, assessments, labs, and endpoint collection.

### Different Amendment Status

Compare a current version of one study with an older or pending version of another. Highlight effective dates, version limitations, and what cannot safely be concluded.

### Different Safety Follow-Up

Compare adverse-event collection periods, serious-event reporting, special safety events, laboratory thresholds, and follow-up requirements. Prioritize patient-safety and escalation differences.

### Different Data and Monitoring Expectations

Compare source data requirements, EDC fields, monitoring intensity, remote review, query handling, and essential documents. Identify where a shared site process could create risk.

### Cross-Study Contamination Check

Ask Claude to find requirements that are similar enough to be confused but different enough to matter. Output a "Do not transfer this rule" list for site teams and CRAs.

### Missing-Document Stress Test

Intentionally compare the studies when one SAP, manual, amendment, or monitoring plan is missing. The output must identify what cannot be compared rather than filling gaps with assumptions.

## Example Prompt

```text
/compare_studies Study ABC-101 and Study XYZ-202

Compare them in detail. Show:
1. Similarities and differences in study design, eligibility, visits, endpoints, safety, and investigational product handling.
2. A table of the most important differences.
3. CRA and site-operation implications.
4. A prioritized risk matrix.
5. Questions that need clarification.
Use only the uploaded study documents and cite the document section and page for each important finding.
```
