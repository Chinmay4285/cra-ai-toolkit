# Protocol Analyzer: Deep Dive Document Analysis

## PURPOSE
Perform a comprehensive structural analysis of your study protocol. Understand the protocol's organization, identify key sections, extract critical requirements, and spot gaps.

## WHEN TO USE
When you first receive a protocol and need to understand its structure. Use this to orient yourself before using other prompts.

## WHAT TO PROVIDE
- Your study protocol (full document or major sections)

## EXPECTED OUTPUT
Structured analysis covering: document organization, key sections, critical requirements, potential gaps, and recommended focus areas.

---

# PROTOCOL ANALYZER PROMPT

```
COPY FROM HERE
========================================================================================

You are analyzing a clinical study protocol to help a CRA understand its structure 
and content.

ANALYSIS STRUCTURE:

1. DOCUMENT OVERVIEW
   - Title, version, date
   - Sponsor, therapeutic area, phase
   - Geographic scope
   - Primary objective (1-2 sentences)

2. DOCUMENT ORGANIZATION
   Map out the protocol's structure:
   - What's in each major section?
   - Where would a CRA find information about [visits/procedures/eligibility/etc.]?
   - Is the organization logical?
   - Are there sections that should be together but aren't?

3. PROTOCOL DESIGN ESSENTIALS
   Extract the core study design:
   - Study design type (RCT, open-label, etc.)
   - Patient population (inclusion/exclusion)
   - Treatment arms and procedures
   - Visit schedule and procedures at each visit
   - Primary and secondary endpoints
   - Safety monitoring plan
   - Duration and phases

4. CRA-CRITICAL SECTIONS
   Identify and summarize:
   - CRA responsibilities (if explicitly stated)
   - Monitoring plan and source data verification requirements
   - Protocol deviation definitions and reporting
   - Documentation requirements
   - Investigator responsibilities that affect CRA work
   - Safety escalation procedures

5. KEY REQUIREMENTS MATRIX
   Create a table of:
   | Requirement | Where Stated | Why It Matters | CRA Impact |
   |---|---|---|---|
   | [Req 1] | [Section X, page Y] | [Reason] | [CRA action] |
   
   Include 15-20 most important requirements

6. CRITICAL NUMBERS & FACTS
   Extract all important numbers:
   - Visit windows (±days)
   - Enrollment target
   - Treatment duration
   - Age range
   - Key lab values or cutoffs
   - Safety thresholds
   - Any percentages or ratios

7. TERMINOLOGY GLOSSARY
   List study-specific terms with definitions:
   - What acronyms does this study use?
   - Are there unusual definitions of common terms?
   - What procedure/assessment names are study-specific?

8. POTENTIAL GAPS OR AMBIGUITIES
   Identify unclear sections:
   - What's not well-specified?
   - Where could sites interpret differently?
   - What might cause confusion?
   - What needs verification with Study Manager?

9. HIGH-RISK AREAS FOR CRA ATTENTION
   Flag areas where problems often occur:
   - Complex eligibility criteria
   - Tight visit windows
   - Multiple assessments in one visit
   - Procedures done at home vs. site
   - Safety-critical procedures
   - Blinding-related procedures

10. RECOMMENDED CRA FOCUS AREAS
    Top 5 things the CRA must know cold:
    1. [Critical fact]
    2. [Critical fact]
    3. [Critical fact]
    4. [Critical fact]
    5. [Critical fact]

========================================================================================
END PROMPT
```

---

## HOW TO USE THIS ANALYSIS

**After receiving your analysis:**

1. **Understand the organization**
   - Know where to find information when you need it

2. **Review the Requirements Matrix**
   - Study this first to grasp key requirements
   - Reference it when training or preparing

3. **Memorize Critical Numbers**
   - These appear frequently; memorizing them saves time

4. **Understand the Glossary**
   - Know your study's unique terminology
   - Use this when communicating with sites

5. **Note the Gaps**
   - If information is ambiguous, clarify with Study Manager before monitoring

6. **Focus on High-Risk Areas**
   - Plan extra verification/training for these topics
   - Watch these especially during monitoring

7. **Commit the Top 5 to Memory**
   - These are your essential study facts
   - Review before every monitoring visit

---

## FOLLOW-UP QUESTIONS TO ASK CLAUDE

After getting the protocol analysis:

- "For each high-risk area, what should I watch for during monitoring?"
- "Create a focused study guide just on [the critical section]"
- "Quiz me on the critical numbers and facts"
- "Create a one-page checklist from the CRA-critical sections"
- "Which of these requirements do sites most often violate?"

---

## WHEN TO USE OTHER PROMPTS

- **For understanding a specific concept:** Use `/02-Understand/teach-me.md`
- **For creating a summary:** Use `/05-Document-Intelligence/document-summary.md`
- **For detecting red flags:** Use `/05-Document-Intelligence/red-flags.md`
- **For finding inconsistencies:** Use `/06-Cross-Document/inconsistency-detector.md`
