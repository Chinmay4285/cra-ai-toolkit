# Quick Start Guide — Get Up and Running with CRA AI Copilot

> **For Clinical Research Associates who want to start using Claude to learn their study, prepare for monitoring visits, and develop CRA judgment.**

---

## 📋 What Do You Need Right Now?

Pick your situation:

### "I'm completely new — Where do I start?"
→ Go to: `DIST/START-HERE.md` (5-minute read)

### "I'm ready to set up Claude"
→ Go to: `DIST/CLAUDE-SETUP.md` (step-by-step guide)

### "I need to see examples before I commit"
→ Go to: `DIST/EXAMPLE-WORKFLOWS.md` (real conversation examples)

### "I need a quick reference while using Claude"
→ Go to: `DIST/CRA-SKILL-MENU.md` (printable command reference)

### "I want to understand the security/compliance implications"
→ Go to: `DIST/PRIVACY-AND-SAFE-USE.md` (safety guidance)

---

## ⚡ The 3-Minute Setup (If You're Ready)

### Step 1: Open Claude
Go to **claude.ai** (or your organization's Claude access)

### Step 2: Create a Project
Name it something like: `Study XYZ — CRA Copilot`

### Step 3: Upload Documents
Upload protocol, amendments, and other approved study documents

### Step 4: Add Master Prompt
Copy `DIST/MASTER-CRA-PROMPT.md` → Paste into Claude Project Instructions

### Step 5: Add Study Context
Copy `DIST/STUDY-CONTEXT-TEMPLATE.md` → Fill in → Paste into Claude

### Step 6: Start Using
Try: `/teach primary endpoint`

**Total time: ~5 minutes. You're ready to learn your study.**

---

## 🎯 Common Workflows at a Glance

### "I don't understand this study"
```
/teach study design and treatment arms
/diagram patient journey
/onepage critical procedures
/quiz me on inclusion criteria
/find-gaps
```

### "Monitoring visit is tomorrow"
```
/visit-prep
/onepage critical procedures
/rapid-review
/questions
```

### "I want to memorize the protocol"
```
/teach [topic]
/quizlet [topic]
/quiz [topic]
/recap
```

### "Compare two protocol versions"
```
/compare protocol v1 vs amendment 2
/detect inconsistencies
/questions this raises
```

### "Practice difficult scenarios"
```
/simulate
[answer Claude's scenario]
[get feedback]
[next scenario]
```

---

## 📚 What Commands Can You Use?

See `DIST/CRA-SKILL-MENU.md` for the complete list.

Quick examples:
- `/teach` — Explain a concept clearly
- `/eli5` — Explain simply
- `/diagram` — Create a visual
- `/quizlet` — Make flashcards
- `/quiz` — Test yourself
- `/visit-prep` — Prepare for monitoring visit
- `/simulate` — Practice scenarios

---

## ❓ Quick FAQ

**Q: Do I need GitHub or developer tools?**
A: No. Just Claude and the files in `DIST/`.

**Q: Can I print the reference materials?**
A: Yes! Print `CRA-SKILL-MENU.md` and keep it at your desk.

**Q: Is this safe to use?**
A: Read `DIST/PRIVACY-AND-SAFE-USE.md` to verify it aligns with your organization's policies.

**Q: Can I share this with colleagues?**
A: Yes, share the `DIST/` folder. They can get started the same way.

**Q: What if Claude gives me wrong information?**
A: Tell Claude immediately: "That doesn't match my protocol." Claude will correct itself. Always verify study-specific answers against your protocol.

---

## 🚀 Next Step

**Pick one:**

1. **New to this?** → Open `DIST/START-HERE.md`
2. **Ready to set up?** → Open `DIST/CLAUDE-SETUP.md`
3. **Want examples?** → Open `DIST/EXAMPLE-WORKFLOWS.md`
4. **Need reference?** → Open `DIST/CRA-SKILL-MENU.md`

---

**Everything else in this repository is developer/maintainer documentation. You don't need it.**

**Just use the `DIST/` folder. That's it.** 🚀

Choose your situation below and follow the exact workflow. Each takes 5-15 minutes to get results.

---

## Situation 1: I Just Got a New Study and Need to Understand It Quickly

**Time: 15 minutes**

### What You Do:

**Step 1** (2 min): Gather documents
- Study protocol (required)
- Study design (optional but helpful)

**Step 2** (3 min): Fill out basic info
- Open: `00-Foundation/study-context-template.md`
- Fill in: Study name, phase, indication, population
- Keep this document; you'll reuse it

**Step 3** (10 min): Start the Study Brain
- Open: `01-Study-Brain/study-expert.md`
- Copy the entire prompt to Claude
- Paste this into the same conversation:
  - Your completed study-context-template.md
  - Your study protocol (full text or key sections)
- Message Claude: **"Analyze this study. I'm a new CRA. What are the most important things for me to know?"**

### Result:
Claude gives you a structured understanding of the study. You now have a "Study Brain" that understands your entire study.

### Next:
Ask follow-up questions like:
- "Why is this visit required?"
- "What's the difference between the primary and secondary endpoints?"
- "Show me the visit schedule as a table"

---

## Situation 2: I Need to Understand One Specific Thing

**Time: 5 minutes**

### What You Do:

**Choose your approach based on the concept:**

#### It's abstract or hard to visualize
→ Use: `03-Visual-Learning/teach-with-diagram.md`

**Copy the prompt** → Paste into Claude → Include your study protocol context → Paste the specific section you don't understand → Submit

**You get back:** A diagram that explains the concept, plus step-by-step explanation.

#### It's a procedure, visit, or process
→ Use: `03-Visual-Learning/process-flow.md`

**Same approach as above.**

#### It's a concept or term
→ Use: `02-Understand/teach-me.md`

**Copy the prompt** → Paste into Claude → Give context about what you already know → Ask your specific question → Submit

**You get back:** Clear explanation with clinical research context.

#### It's complex and I learn better from stories
→ Use: `02-Understand/explain-like-a-story.md`

**Copy the prompt** → Paste into Claude → Ask: "Tell me the story of [this concept]" → Submit

**You get back:** A narrative explanation with characters, consequences, and CRA takeaways.

---

## Situation 3: I Have a Monitoring Visit Next Week

**Time: 20 minutes to prepare**

### What You Do:

**Step 1** (5 min): Load Study Brain
- If you haven't already, follow **Situation 1** above
- Create a Claude conversation with your Study Brain and protocol

**Step 2** (15 min): Use monitoring visit prep
- Open: `07-CRA-Workflow/monitoring-visit-prep.md`
- Copy the prompt to Claude
- Include:
  - Your study context
  - Any previous monitoring visit notes/action items
  - Your protocol
  - Anything you know about site performance
- Submit

**You get back:** Prioritized checklist of what to check, what questions to ask, what documents to review, and what to verify.

### During the Visit:
Keep this checklist nearby. Refer to it as you work through site records.

### After the Visit:
- Open: `07-CRA-Workflow/monitoring-visit-followup.md`
- Copy the prompt to Claude
- Paste your visit notes
- Get: Organized action items, follow-ups, and documentation needs

---

## Situation 4: I Need to Learn and Remember This Study

**Time: 30 minutes to set up; ongoing as you study**

### What You Do:

**Step 1**: Start with Situation 1 (Create Study Brain)

**Step 2**: Generate flashcards
- Open: `04-Memorization/quizlet-generator.md`
- Copy prompt to Claude
- Include your study protocol and context
- Get: Quizlet-formatted flashcards
- Import into Quizlet app and study

**Step 3**: Use multiple learning modes
- Week 1:
  - Use `02-Understand/teach-me.md` for confusing concepts
  - Use `03-Visual-Learning/teach-with-diagram.md` for processes
  - Use `04-Memorization/flashcards.md` to practice

- Week 2:
  - Use `04-Memorization/scenario-quiz.md` to test understanding
  - Use `02-Understand/compare-concepts.md` to connect ideas
  - Use `04-Memorization/multiple-choice-quiz.md`

- Week 3+:
  - Use `04-Memorization/rapid-review.md` before meetings
  - Use `08-Training/personal-cra-tutor.md` for adaptive testing
  - Use `09-Advanced/knowledge-gap-detector.md` to find weak spots

**Step 4**: Test yourself
- Use: `04-Memorization/scenario-quiz.md`
- Copy prompt to Claude
- Get realistic CRA scenarios to solve
- Claude evaluates your responses and teaches

---

## Situation 5: I Found Something That Seems Wrong or Inconsistent

**Time: 10-15 minutes**

### Scenario A: Two documents seem to conflict

**What You Do:**
- Open: `06-Cross-Document/inconsistency-detector.md`
- Copy prompt to Claude
- Paste both documents (or the conflicting sections)
- Paste your study context
- Ask: "Are these documents consistent?"

**You get back:** Analysis of conflicts, clarification, and what needs verification.

### Scenario B: I think something's missing from the protocol

**What You Do:**
- Open: `05-Document-Intelligence/missing-information.md`
- Copy prompt to Claude
- Paste the protocol
- Ask: "What important information might be missing?"

**You get back:** Potential gaps, missing specifications, and clarification questions.

### Scenario C: One protocol is old, one is new — what changed?

**What You Do:**
- Open: `06-Cross-Document/change-impact-analysis.md`
- Copy prompt to Claude
- Paste the OLD version and NEW version
- Ask: "What changed between these versions, and how does it affect CRA work?"

**You get back:** Marked-up changes, impact analysis, and what sites need to know.

---

## Situation 6: There's a Problem at a Site

**Time: 15-20 minutes**

### What You Do:

**Step 1**: Use Site Issue Analysis
- Open: `07-CRA-Workflow/site-issue-analysis.md`
- Copy prompt to Claude
- Include:
  - Your study context
  - Protocol
  - Details of the problem
  - Any previous issues at this site
  - Site staff involved

**Step 2**: Get back:
- Root cause analysis
- Risk categorization
- Recommended follow-up
- Questions to ask the site
- Documentation recommendations

**Step 3**: Consider using Additional Prompts:
- If a specific protocol requirement was violated: `07-CRA-Workflow/protocol-deviation-analysis.md`
- If you need to prioritize multiple issues: `09-Advanced/issue-triage.md`
- If you need to find root causes: `09-Advanced/root-cause-analysis.md`

---

## Situation 7: I Want to Test My Knowledge (Self-Quiz)

**Time: 20-30 minutes**

### What You Do:

**Option A: Multiple Choice**
- Open: `04-Memorization/multiple-choice-quiz.md`
- Copy prompt to Claude
- Include your study context
- Ask: "Quiz me on [specific topic]"
- Claude gives questions; you answer
- Claude grades you and explains answers

**Option B: Scenario-Based**
- Open: `04-Memorization/scenario-quiz.md`
- Copy prompt to Claude
- Include study context + protocol
- Claude presents realistic CRA scenarios
- You decide what to do
- Claude evaluates your judgment

**Option C: Adaptive Tutor**
- Open: `08-Training/personal-cra-tutor.md`
- Copy prompt to Claude
- Include full study context
- Claude analyzes your weak areas and creates custom quiz
- Get feedback and recommendations

**Option D: Rapid Fire**
- Open: `04-Memorization/rapid-review.md`
- Copy prompt to Claude
- Ask: "Give me a 5-minute rapid-fire review of the study"
- Claude covers essential facts quickly

---

## Situation 8: I Need to Explain This to Someone Else

**Time: 10-15 minutes**

### What You Do:

**Choose who you need to explain it to:**

#### Explaining to a new CRA
→ Use: `02-Understand/beginner-to-expert.md`

**Copy prompt** → Tell Claude the new person's background → Ask: "Explain [concept] for a CRA new to this study" → Submit

#### Explaining to a site coordinator or investigator
→ Use: `07-CRA-Workflow/question-generator.md`

**Copy prompt** → Include study context → Ask: "Generate questions I should ask the site about [topic]"

#### Explaining to a project manager/non-clinical person
→ Use: `02-Understand/explain-simply.md`

**Copy prompt** → Ask: "Explain [concept] in a way a non-clinical project manager would understand"

#### Explaining in writing (email/communication)
→ Use: `07-CRA-Workflow/monitoring-visit-followup.md` (for professional communication templates)

---

## Situation 9: I'm Preparing for a Job Interview or Need to Refresh My Knowledge Quickly

**Time: 30 minutes**

### What You Do:

**Step 1**: Use rapid review
- Open: `04-Memorization/rapid-review.md`
- Copy prompt to Claude
- Include study context
- Ask: "Give me the 2-minute version of what I need to know about this study"

**Step 2**: Use critical thinking prep
- Open: `08-Training/critical-thinking.md`
- Copy prompt to Claude
- Ask: "Give me 5 tough questions about this study and my approach to it"

**Step 3**: Use scenario simulator
- Open: `08-Training/scenario-simulator.md`
- Copy prompt to Claude
- Ask: "Give me realistic scenarios I might face as a CRA on this study"

**You get back:** Knowledge summary, tough questions with explanation, and scenarios to think through.

---

## Situation 10: I Don't Know What I Don't Know

**Time: 20 minutes**

### What You Do:

- Open: `09-Advanced/knowledge-gap-detector.md`
- Copy prompt to Claude
- Include:
  - Your study context
  - Protocol
  - Answers to recent quizzes or questions you've attempted
  - Any monitoring visit notes or performance data
- Ask: "What are my knowledge gaps? Where should I focus?"

**You get back:**
- Strongest areas
- Weakest areas
- Concepts to revisit
- Recommended next lesson
- Focused quiz on weak areas

---

## Situation 11: I Need to Create a Comprehensive Study Summary

**Time: 30-45 minutes**

### What You Do:

**For a 1-page summary:**
- Open: `05-Document-Intelligence/one-page-summary.md`
- Copy prompt to Claude
- Paste entire protocol
- Get: Concise 1-page overview

**For a detailed summary:**
- Open: `05-Document-Intelligence/document-summary.md`
- Copy prompt to Claude
- Paste protocol
- Get: Structured summary with all sections

**For just the key points:**
- Open: `05-Document-Intelligence/key-points.md`
- Copy prompt to Claude
- Paste protocol
- Get: Most essential facts only

---

## Situation 12: I Need to Compare Multiple Study Requirements

**Time: 20-30 minutes**

### What You Do:

- Open: `06-Cross-Document/requirement-matrix.md`
- Copy prompt to Claude
- Paste all relevant documents (protocol, SAP, ICF, monitoring plan, etc.)
- Ask: "Create a matrix showing [requirement type] across all these documents"

**Example:**
- "Show me all visit windows in one table"
- "Show me eligibility criteria from protocol vs. ICF"
- "Compare safety reporting requirements across all documents"

**You get back:** Clear matrix/table showing how requirements align across documents.

---

## Pro Tips

### 1. **Keep One Main Study Brain Conversation Going**
Don't start new Claude conversations for each question. Use the same conversation that has your study context and protocol. Claude remembers everything and gives better answers.

### 2. **Start with the Study Brain**
Before using specialized prompts, make sure you've created a Study Brain conversation with your complete study context. This gives Claude what it needs to give you good answers.

### 3. **Reuse Your Study Context**
Fill out `00-Foundation/study-context-template.md` once, then paste it into every Claude conversation. It's your reference document and saves time.

### 4. **Know Your Workflow**
- First time with study → Situation 1
- Confused about something → Situation 2
- Monitoring visit coming → Situation 3
- Need to learn everything → Situation 4
- Something seems wrong → Situation 5

### 5. **Verify Important Information**
When Claude gives you an answer about your study:
- Always cross-check critical information against the actual protocol
- Ask Claude: "Where in the protocol does it say that?"
- Remember: Claude is a thinking tool, not an authority

### 6. **Customize Prompts for Your Needs**
These are starting points. Adapt them:
- Add specific details about your study
- Ask follow-up questions
- Request different output formats
- Combine prompts for specialized use cases

### 7. **Use PDF Conversion if Needed**
If you have PDF protocols:
- Convert to text using a tool like Adobe or online converter
- Copy-paste the text into Claude
- Claude works with text, not files

---

## When to Use Each Prompt: Decision Tree

```
START: What do I need help with?

├─ LEARNING & UNDERSTANDING
│  ├─ Concept unclear? → teach-me.md
│  ├─ Need visual? → teach-with-diagram.md
│  ├─ Prefer story? → explain-like-a-story.md
│  ├─ Comparing ideas? → compare-concepts.md
│  └─ Advanced explanation? → beginner-to-expert.md
│
├─ MEMORIZATION & TESTING
│  ├─ Need flashcards? → quizlet-generator.md
│  ├─ Want quick quiz? → multiple-choice-quiz.md
│  ├─ Realistic scenarios? → scenario-quiz.md
│  ├─ Adaptive testing? → personal-cra-tutor.md
│  └─ Last-minute review? → rapid-review.md
│
├─ DOCUMENTS
│  ├─ Understand one protocol? → protocol-analyzer.md
│  ├─ Summarize it? → document-summary.md
│  ├─ Key points only? → key-points.md
│  ├─ Find red flags? → red-flags.md
│  ├─ Find gaps? → missing-information.md
│  └─ Extract terms? → terminology-extractor.md
│
├─ COMPARING DOCUMENTS
│  ├─ Compare 2+ docs? → compare-documents.md
│  ├─ Find conflicts? → inconsistency-detector.md
│  ├─ Create matrix? → requirement-matrix.md
│  ├─ Analyze changes? → change-impact-analysis.md
│  └─ Version comparison? → what-changed-detector.md
│
├─ WORKFLOW & VISITING
│  ├─ Prepare for visit? → monitoring-visit-prep.md
│  ├─ Follow up after visit? → monitoring-visit-followup.md
│  ├─ Site has problem? → site-issue-analysis.md
│  ├─ Deviation occurred? → protocol-deviation-analysis.md
│  ├─ Understand query? → query-analysis.md
│  ├─ Track action items? → action-items.md
│  └─ Generate questions? → question-generator.md
│
├─ TRAINING & JUDGMENT
│  ├─ Adaptive tutoring? → personal-cra-tutor.md
│  ├─ Critical thinking? → critical-thinking.md
│  ├─ Practice scenarios? → scenario-simulator.md
│  ├─ Mock visit? → mock-monitoring-visit.md
│  └─ Interview prep? → interview-prep.md
│
├─ ADVANCED ANALYSIS
│  ├─ Find risks? → risk-based-review.md
│  ├─ Root cause? → root-cause-analysis.md
│  ├─ Prioritize issues? → issue-triage.md
│  ├─ Find assumptions? → assumption-detector.md
│  └─ Find weak areas? → knowledge-gap-detector.md
│
└─ FOUNDATION
   ├─ Set up study? → study-context-template.md
   ├─ Start Study Brain? → study-expert.md
   └─ Learn system? → This file + CLAUDE-USAGE-GUIDE.md
```

---

## Troubleshooting Quick Reference

| Problem | Solution |
|---------|----------|
| Claude seems confused | Reload the Study Brain prompt + your protocol |
| Claude makes up information | Use source-grounding-rules.md; ask for citation |
| Claude keeps forgetting things | You're in a different conversation; use the same one |
| Answer doesn't match what I need | Add more specific context; ask clarifying questions |
| Output is too long/short | Ask Claude: "Please provide a [X-minute version/one-page summary]" |
| Diagram isn't helpful | Try a different visual prompt or ask for a different format |
| Quiz is too easy/hard | Ask Claude to adjust difficulty level |
| Don't know which prompt to use | Check "When to Use Each Prompt" decision tree above |

---

**You're ready to start. Pick your situation above and begin.**

The more you use this system, the faster and better your results will be.
