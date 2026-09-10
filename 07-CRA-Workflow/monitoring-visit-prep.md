# Monitoring Visit Prep: Pre-Visit Preparation

## PURPOSE
Prepare thoroughly for a monitoring visit. Get a comprehensive checklist of what to verify, what to prepare, key documents to review, and important questions to ask.

## WHEN TO USE
1-2 weeks before a scheduled monitoring visit. Use this to create your visit preparation plan.

## WHAT TO PROVIDE
- Your study context
- Your protocol
- Which visit type you're preparing for (or timepoint)
- Any previous monitoring visit notes or site-specific challenges (optional)

## EXPECTED OUTPUT
Comprehensive preparation checklist organized by: critical items to verify, documents to gather, procedures to review, questions to ask, and risk areas to focus on.

---

# MONITORING VISIT PREP PROMPT

```
COPY FROM HERE
========================================================================================

You are preparing a CRA for a monitoring visit.

PREPARATION STRUCTURE:

1. VISIT OVERVIEW
   - What visit is this? (screening, baseline, week 4, etc.)
   - What's the key purpose of this visit?
   - What assessments/procedures are scheduled?
   - What's the visit window? What dates are acceptable?

2. CRITICAL ITEMS TO VERIFY
   Items that MUST be verified at this visit (or documented as missing):
   
   [ ] [Item 1] - verify [specific requirement]
   [ ] [Item 2] - verify [specific requirement]
   
   For each item, include:
   - What exactly to look for
   - Where should it be documented (EDC, case report form, source, etc.)
   - What would be a deviation or problem
   - What to do if it's missing/wrong

3. SOURCE DATA VERIFICATION CHECKLIST
   
   Documents to review and verify:
   [ ] Medical records - verify [specific items]
   [ ] Signed informed consent - verify [requirements]
   [ ] Lab results - verify [which labs, compare to EDC]
   [ ] Vital signs - verify [procedures]
   [ ] [Other source documents specific to this visit]
   
   For each:
   - What % verification required?
   - What common errors do sites make?
   - What inconsistencies should raise concerns?

4. PROCEDURAL VERIFICATION
   Procedures that should have happened at this visit:
   
   [ ] [Procedure 1]
     - Check that: [specific verification]
     - Ask site: [specific question]
   
   [ ] [Procedure 2]
     - Check that: [specific verification]
     - Ask site: [specific question]

5. SAFETY ITEMS TO VERIFY
   Safety requirements for this visit phase:
   
   [ ] Adverse events - ask about any issues since last visit
   [ ] Prohibited medications - verify none were given
   [ ] Safety labs (if due) - verify completed and reviewed
   [ ] [Other safety items specific to this study]

6. DATA QUALITY CHECKS
   Common data issues to look for:
   
   [ ] EDC entries match source documents (compare [specific items])
   [ ] Dates correct (visit date, procedure dates, assessment dates)
   [ ] Required fields all completed (not blank/unknown)
   [ ] Values reasonable (no data entry errors, impossible values)
   [ ] Query responses entered correctly
   [ ] [Study-specific data quality issues]

7. STUDY-SPECIFIC RISK AREAS
   Areas where THIS SITE or THIS STUDY often has problems:
   
   [Based on previous visits / study design / known challenges]
   - High-risk area 1: [Risk] - Extra verification needed: [what to check]
   - High-risk area 2: [Risk] - Extra verification needed: [what to check]
   - High-risk area 3: [Risk] - Extra verification needed: [what to check]

8. QUESTIONS TO ASK THE SITE
   Structured questions organized by topic:
   
   ENROLLMENT & ELIGIBILITY:
   - [Question 1]
   - [Question 2]
   
   VISIT PROCEDURES:
   - [Question 1]
   - [Question 2]
   
   DATA QUALITY:
   - [Question 1]
   - [Question 2]
   
   SAFETY:
   - [Question 1]
   - [Question 2]
   
   OPEN ISSUES FROM PREVIOUS VISIT:
   - [Question 1 regarding previous action item]
   - [Question 2 regarding previous concern]

9. DOCUMENTS TO GATHER BEFORE THE VISIT
   
   [ ] Current protocol (bring the version the site should be using)
   [ ] Previous visit notes and action items
   [ ] Enrollment status and tracking
   [ ] Current EDC data printout
   [ ] Safety reports (if available)
   [ ] Any recent queries or concerns
   [ ] Site contact list

10. ENROLLMENT STATUS GOING INTO THIS VISIT
    - Total enrolled to date at this site: [X]
    - Expected to be enrolled by next visit: [X]
    - Are we on track? Any delays?
    - Are there screen failures? If so, why?

11. OPEN ISSUES FROM PREVIOUS VISIT
    - [Action item 1] - Status?
    - [Action item 2] - Status?
    - [Question 1] - Has this been resolved?
    - [Concern 1] - Has this improved?

12. VISIT LOGISTICS
    - Site contact: [Name, number]
    - Expected visit duration: [X hours]
    - Number of patients to see: [X]
    - Materials needed: [List]
    - Schedule: [Specific appointment times if known]

13. AFTER-VISIT PLAN
    Timeline for follow-up:
    - Day of visit: [Actions]
    - Within 1 day: [Actions]
    - Within 1 week: [Actions]

========================================================================================
END PROMPT
```

---

## HOW TO USE YOUR VISIT PREP

**1 Week Before Visit:**
- Read through entire prep checklist
- Gather all documents listed in section 9
- Review previous visit notes (section 11)
- Refresh your memory on visit procedures

**2-3 Days Before Visit:**
- Review sections 2-4 (Critical items, SDV checklist, procedures)
- Review questions (section 8)
- Plan your route/timing

**Morning of Visit:**
- Quick review of sections 2, 5, 8
- Print or load the checklist
- Bring all documents

**During Visit:**
- Check items off as you verify
- Take detailed notes in the "Verification" column
- Document any deviations immediately
- Ask all questions even if you think you know the answer

**After Visit:**
- Review notes same day
- Identify any follow-up needed
- Document action items
- Plan any escalations

---

## TIPS FOR EFFECTIVE VISITS

1. **Ask, Don't Assume**
   - Even if you think you know the answer, ask the site
   - "Help me understand..." approach
   - "Can you walk me through how you..."

2. **Verify Everything**
   - Don't rely on memory or last visit
   - Check source documents against EDC
   - Look for patterns (if one date is wrong, check others)

3. **Document Thoroughly**
   - Date, time, who was present
   - What you verified and what you found
   - What was discussed
   - Any deviations noted
   - Follow-up needed

4. **Be Professional but Collaborative**
   - Sites want to do good work
   - Approach as "let's solve this together"
   - Praise good practices
   - Offer help with problems

5. **Follow Safety First**
   - If you discover a safety issue, escalate immediately
   - Don't wait to report safety concerns

---

## INTEGRATING WITH YOUR STUDY BRAIN

In your Study Brain conversation, ask:
- `/visit prep for [visit type]`

Claude will generate this comprehensive prep using your specific study context.

---

## WHEN TO USE RELATED PROMPTS

- **After the visit:** Use `/07-CRA-Workflow/monitoring-visit-followup.md`
- **For detailed questions:** Use `/07-CRA-Workflow/question-generator.md`
- **For analyzing a problem:** Use `/07-CRA-Workflow/site-issue-analysis.md`
- **For understanding procedures:** Use `/02-Understand/teach-me.md`
