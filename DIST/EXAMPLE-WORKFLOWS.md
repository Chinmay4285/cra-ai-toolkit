# Example Workflows — Real Claude Conversations

These are realistic examples of how you might use the CRA AI Copilot. Each example shows a complete workflow with actual questions, Claude's responses (summarized), and next steps.

---

## EXAMPLE 1: "I Just Got a New Study — Help Me Understand It"

### Scenario
You're a CRA assigned to a new study. You have the protocol, SAP, and monitoring plan uploaded. You want to understand it quickly and be ready to screen patients.

### Workflow

**Step 1: Get Study Overview**
```
You: /teach study design and treatment arms

Claude: [Explains the design type, randomization, treatment groups]
        Covers: why this design was chosen, implications for CRA work
        Mentions: blinding requirements, handling of protocol deviations
        
Claude offers: → See as diagram → Explore eligibility requirements → Create quick reference
```

**Step 2: Understand Patient Journey**
```
You: /diagram patient journey

Claude: [Creates flowchart showing screening → enrollment → treatment visits → follow-up]
        Shows: decision points, assessment windows, timing
        Labels: key procedures at each step, compliance requirements
```

**Step 3: Get Quick Reference**
```
You: /onepage critical procedures and eligibility

Claude: [Produces one-page reference with:
        - 5 key inclusion criteria
        - 5 key exclusion criteria
        - Critical procedures at each visit
        - Common deviations to watch for
        - Enrollment/visit windows]
```

**Step 4: Identify Knowledge Gaps**
```
You: /find-gaps

Claude: You now understand:
        ✓ Study design and patient flow
        ✓ Basic eligibility criteria
        ✓ Visit procedures
        
        Recommended next steps:
        → Understand primary endpoint and how it's measured
        → Explore safety monitoring requirements
        → Learn about protocol deviations specific to this study
        
You: /teach primary endpoint

Claude: [Explains endpoint definition, measurement timing, data collection]
        Clarifies: how it differs from secondary endpoints, why it matters
```

**Step 5: Test Yourself**
```
You: /quiz eligibility criteria

Claude: Question 1 of 5: A 22-year-old patient with condition ABC approaches you about the study. Their baseline lab is slightly outside acceptable range. Are they eligible?

You: [Your answer]

Claude: Let's break this down... [Teaches the principle]
        Next question...
```

### Result
After this workflow, you have:
✅ Understanding of study design  
✅ Visual map of patient flow  
✅ Quick reference guide  
✅ Identified remaining gaps  
✅ Tested knowledge of eligibility  

---

## EXAMPLE 2: "Monitoring Visit Tomorrow — Prep in 20 Minutes"

### Scenario
Your monitoring visit is tomorrow. You need to prepare efficiently but thoroughly.

### Workflow

**Step 1: Get Monitoring Checklist**
```
You: /visit-prep

Claude: [Generates comprehensive pre-visit checklist:
        BEFORE THE VISIT:
        - Chart review (patients, enrollment, ongoing treatments)
        - Data verification (source documents match CRF)
        - Outstanding data queries
        - Previous action items from last visit
        - Documentation review (regulatory binder, ICF files)
        
        AT THE VISIT:
        - Patient screening/enrollment verification
        - Current patient status review
        - Safety assessment
        - Competency check of coordinators
        - Device/equipment calibration
        
        BRING TO VISIT:
        - Current protocol and amendments
        - Monitoring checklist
        - Query list
        - Study coordinator contact info
        
        PRIORITY ITEMS FOR YOUR SITE:
        - [Your specific site issues from previous visits]
        - [Known enrollment challenges]
        - [Any pending regulatory items]]
```

**Step 2: Quick Reference**
```
You: /onepage procedures for this site

Claude: [One-page reference showing:
        - Your site enrollment status
        - Patient visit windows and who's overdue
        - Key procedures performed at this visit type
        - Compliance history
        - Known issues to focus on]
```

**Step 3: Rapid Fact Refresh**
```
You: /rapid-review

Claude: [2-minute version with critical facts:
        30-SECOND VERSION (key facts):
        - Primary endpoint definition
        - Visit timing and windows
        - 3 most common deviations at this site
        
        5-SECOND REVIEW (just the basics):
        - Study phase and patient flow
        - Your site's enrollment number
        
        2-MINUTE REVIEW (deeper):
        [More detail on procedures, timing, compliance requirements]]
```

**Step 4: Generate Smart Questions**
```
You: /questions

Claude: [Smart questions to ask the site, organized by category:
        ENROLLMENT & ELIGIBILITY:
        - "Can you walk me through your current screening log?"
        - "Any challenges with eligibility assessment?"
        
        SAFETY & COMPLIANCE:
        - "How are you managing [specific safety monitoring requirement]?"
        - "Any near-misses or safety concerns since last visit?"
        
        DATA QUALITY:
        - "Why is Patient #003's baseline lab missing?"
        - "How are you handling the [specific data element]?"
        
        PROTOCOL ADHERENCE:
        - "Patient #005 missed a visit by 6 days — tell me about that"
        - "Any protocol deviations we should discuss?"]
```

### Result
After this workflow, you:
✅ Have comprehensive visit checklist  
✅ Know your site's specific priorities  
✅ Have key facts reviewed  
✅ Have smart questions prepared  

**Total time: ~15 minutes of prep work**

---

## EXAMPLE 3: "Compare Protocol Versions — Find What Changed"

### Scenario
You received Amendment 2 to the protocol. You need to quickly understand what changed and how it impacts your site's work.

### Workflow

**Step 1: Side-by-Side Comparison**
```
You: /compare protocol original vs amendment 2

Claude: [Creates comparison table showing:
        
        SECTION          ORIGINAL              AMENDMENT 2
        ────────────────────────────────────────────────
        Primary Endpoint Definition 1          Modified Definition 1a
        Visit Windows    ±3 days              ±5 days (some visits)
        Safety Monitoring Every visit         Weeks 0, 2, 8, 12, then every 4 weeks
        Lab Reqs         Full panel every visit    Reduced panel from week 24 onward
        etc.]
```

**Step 2: Find Conflicts**
```
You: /detect

Claude: I've reviewed both versions. Here are the differences:

        CRITICAL CHANGES (your site must adapt):
        ✓ Amendment 2 extends visit windows by 2 days
        ✓ This gives more flexibility for your patient scheduling
        ✓ BUT: Baseline visit window remains ±3 days
        
        IMPORTANT CHANGES (affects procedures):
        ✓ Lab panel is reduced starting week 24
        ✓ Notify your lab of this change
        
        MINOR CHANGES (note for reference):
        ✓ Terminology updated in Section 4.2
        ✓ Formatting change in CRF (no impact on data)
```

**Step 3: Understand CRA Impact**
```
You: /teach changes and what they mean for CRA work

Claude: The amendment makes three key changes to your work:

        1. VISIT SCHEDULING (affects your calendar)
           - Baseline: Still ±3 days (no change) — STRICT
           - Other visits: Now ±5 days (was ±3) — MORE FLEXIBLE
           - Impact: You have more time to coordinate patient visits
           - Action: Update your patient visit calendar
           
        2. LAB MONITORING (affects coordinators)
           - Full panel through week 12
           - Reduced panel starting week 24 (different draw order)
           - Impact: Educate your lab and coordinators on the change
           - Action: Notify lab staff before enrollment
           
        3. DOCUMENTATION (affects your regulatory binder)
           - Amendment 2 becomes effective [date]
           - Site must use Amendment 2 for any NEW enrollments
           - Existing patients continue on their protocol version
           - Action: Date your regulatory documents clearly
```

### Result
After this workflow, you:
✅ Understand exactly what changed  
✅ Know which changes are critical vs. minor  
✅ Know how to implement changes at your site  
✅ Can educate your team on amendments  

---

## EXAMPLE 4: "Quiz Yourself — Test Knowledge"

### Scenario
You want to make sure you can answer questions confidently at monitoring visits.

### Workflow

**Step 1: Start Quiz**
```
You: /quiz eligibility and deviations

Claude: Question 1 of 10:

        A patient is 76 years old with a baseline lab slightly elevated.
        The protocol says "18-75 years old" and "Lab value <X."
        
        What do you tell the site about this patient's eligibility?
```

**Step 2: Answer and Get Feedback**
```
You: They don't meet criteria. We can't enroll.

Claude: ✓ CORRECT, with nuance:
        
        You correctly identified that the patient doesn't meet both criteria.
        
        KEY PRINCIPLE:
        When ANY inclusion criterion is not met, the patient is ineligible.
        This is an "AND" requirement, not "OR".
        
        WHAT TO DISCUSS WITH SITE:
        - Is the age documented correctly?
        - Can the lab be repeated within acceptable timeframe?
        - Are there protocol exceptions that apply? (Get sponsor approval)
        
        Next question...
```

**Step 3: Continue Testing**
```
Claude: Question 2 of 10: [Next scenario about deviations]

You: [Answer]

Claude: [Feedback and teaching]
        
        [Continue through 10 questions]
```

**Step 4: Review Results**
```
Claude: QUIZ COMPLETE ✓

        Your Score: 9/10 (90%)
        
        Strengths:
        ✓ Excellent understanding of eligibility criteria
        ✓ Good instinct for when to escalate to sponsor
        
        Areas to Review:
        → Protocol deviations (1 question missed)
        → Consider: /teach protocol deviations
        
        Ready to quiz again, or explore another topic?
```

### Result
After this workflow, you:
✅ Tested your knowledge  
✅ Got immediate feedback  
✅ Understood why you were right or wrong  
✅ Identified areas to review  

---

## EXAMPLE 5: "Practice a Difficult Scenario — Develop Judgment"

### Scenario
You want to practice responding to challenging site situations before they happen.

### Workflow

**Step 1: Start Scenario**
```
You: /simulate difficult monitoring visit scenario

Claude: Here's a realistic scenario:

        You arrive at the site for monitoring visit. The site coordinator tells you:
        
        "Patient #005 missed their week 8 visit by 7 days due to work travel.
        We just saw them yesterday (day 8). We didn't report it yet because
        we wanted to see if you'd approve it as on-time."
        
        How do you respond?
        What do you do next?
```

**Step 2: Give Your Response**
```
You: I need to report this as a deviation because the visit window was missed.
     I'll document it, notify the sponsor, and let them decide if we can continue.

Claude: EXCELLENT APPROACH. Let me break down what you did right and what to consider:

        ✓ YOU CORRECTLY IDENTIFIED: This is a protocol deviation
          - Window was ±3 days, visit was 8 days late
          - Definition of deviation: visit outside window
        
        ✓ YOU CORRECTLY DECIDED: Report to sponsor
          - Site's preference doesn't matter; protocol deviation must be reported
        
        → CONSIDER ALSO:
          - Determine: Is this a MAJOR or MINOR deviation?
            (Usually major = affects primary endpoint, minor = administrative)
          - Ask site: Why did they delay reporting?
            (Helps you identify training needs or site compliance issues)
          - Check: Does this patient need any additional assessments due to timing?
        
        PRINCIPLE YOU DEMONSTRATED:
        Deviation reporting is not negotiable; your judgment is about
        severity assessment and follow-up actions, not whether to report.
```

**Step 3: Next Scenario**
```
Claude: Here's another scenario (slightly more complex):

        Patient #002 completed all study procedures for week 12 visit.
        After leaving, the coordinator realizes they forgot to collect
        one required lab sample.
        
        Site asks: "Can they come back tomorrow?"
        How do you respond?
```

**Step 4: Continue**
```
You: [Your response]

Claude: [Feedback and next scenario, escalating difficulty]
```

### Result
After this workflow, you:
✅ Practiced realistic scenarios  
✅ Got coaching on judgment calls  
✅ Learned principles behind decisions  
✅ Built confidence for actual situations  

---

## EXAMPLE 6: "Create Study Materials — Teach Your Team"

### Scenario
You need to train your site coordinator on protocol eligibility criteria.

### Workflow

**Step 1: Create Quizlet Flashcards**
```
You: /quizlet create cards for inclusion criteria

Claude: Here are Quizlet-ready flashcards:

        LEVEL 1 (Memorization):
        Q: What is the age range for study eligibility?
        A: 18-75 years old
        
        Q: What is the minimum baseline lab value?
        A: ≥50 (or reference range for your study)
        
        ... [20-30 flashcards in Quizlet format]
        
        LEVEL 2 (Understanding):
        Q: A 17-year-old meets all other criteria. Why can't we enroll?
        A: Age requirement is 18-75. Anyone outside this range doesn't meet inclusion criteria, regardless of how well they match otherwise.
        
        ... [10-15 understanding cards]
        
        LEVEL 3 (Application):
        Q: Patient A is 19, Patient B is 78, Patient C is 45.
        A: C is eligible for age; A and B are not.
        
        [Ready to copy to Quizlet]
```

**Step 2: Create One-Page Reference**
```
You: /onepage eligibility criteria for my coordinator training

Claude: [Produces single-page summary:
        - 5 inclusion criteria (prioritized by importance)
        - 5 exclusion criteria (with examples)
        - What to do if uncertain
        - Escalation contacts]
```

**Step 3: Story Format for Memorable Learning**
```
You: /story how a patient goes through eligibility screening

Claude: [Narrative walkthrough:
        "Picture this: A patient calls your site interested in the study...
        They provide their medical history...
        You screen them against each criterion...
        Here's how that conversation might go...
        Here are the decision points..."]
```

### Result
After this workflow, you:
✅ Have Quizlet cards for deeper learning  
✅ Have one-page reference for quick lookup  
✅ Have story format for memorable teaching  
✅ Can train your coordinator confidently  

---

## TIPS FOR USING WORKFLOWS

### 1. Adapt the Order
These workflows aren't rigid. You can:
- Skip steps
- Reorder based on your needs
- Combine workflows
- Add your own questions

### 2. Save What Works
Claude remembers your conversation. You can:
- Refer back to earlier answers
- Ask Claude to update or clarify previous responses
- Build on previous teaching

### 3. Use Multiple Commands
Don't feel limited to one command per topic:
- `/teach` then `/diagram` then `/quiz` all on the same topic works great
- Claude builds understanding progressively

### 4. Customize for Your Study
Every example here assumes you've:
- Uploaded your study documents
- Provided your study context
- Set up Master CRA Prompt in Claude

Adapt the examples to your specific study details.

---

## WHAT IF SOMETHING DOESN'T WORK?

**Command didn't work?**
- You can always ask conversationally instead
- `/quiz` can be replaced with: "Can you quiz me?"
- Claude is flexible with how you ask

**Answer wasn't what you expected?**
- Tell Claude: "Can you explain this differently?" or "That was too simple, go deeper"
- Claude will adjust
- Provide feedback: "I need more focus on..."

**Claude gave you incorrect information?**
- Tell Claude immediately: "I think that's wrong based on my protocol"
- Claude will check and correct itself
- This helps Claude learn your specific study

---

## NEXT STEPS

1. **Pick a scenario** from above that matches your current situation
2. **Open Claude** with your study documents and Master Prompt loaded
3. **Try the workflow** — adapt as needed for your study
4. **See what works best for you**

Different CRAs use these tools differently. Experiment and find your style!

---

**Ready to try a workflow? Pick one above and get started!** 🚀
