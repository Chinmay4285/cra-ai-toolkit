# CRA AI Toolkit: The AI Operating System for Clinical Research Associates

Welcome to a **professional, interconnected AI system** designed specifically for Clinical Research Associates (CRAs) working with Claude.

This toolkit transforms how you:
- Understand complex clinical research protocols and documents
- Learn study designs, eligibility criteria, visit schedules, and procedures
- Memorize hundreds of facts, acronyms, and requirements
- Prepare for monitoring visits and site interactions
- Identify inconsistencies, gaps, and risks in study documentation
- Train yourself and improve your CRA judgment
- Manage study-specific knowledge throughout your involvement

---

## What This Is

**NOT** a collection of generic prompts.

**Rather** a cohesive "AI operating system" where:
- Each prompt has a specific, well-defined purpose
- Prompts work independently and together seamlessly
- The "Study Brain" maintains context throughout conversations
- Every prompt follows production quality standards
- All prompts are grounded in provided study documents (no hallucinations)
- The system grows with your knowledge of the study
- You minimize manual work: **Paste document → Paste prompt → Get useful output**

---

## Who This Is For

- **Clinical Research Associates** preparing for monitoring visits
- **New CRAs** learning clinical research concepts and procedures
- **Site coordinators and CRAs** needing rapid training on new studies
- **Study teams** that want structured Claude integration
- **Anyone** who needs to deeply understand clinical research documentation

**No prior AI experience required.** This toolkit is self-contained and designed for practical use.

---

## How to Get Started in 5 Minutes

### Step 1: Prepare Your Study Documents
Gather key documents:
- Study Protocol (current version)
- Study Design diagram or SAP
- Visit schedule
- Any other study materials

You do NOT need to provide everything at once. Start with the protocol.

### Step 2: Create Your Study Context
Open `00-Foundation/study-context-template.md` and fill in basic study information. This becomes your reference throughout your work with Claude.

### Step 3: Start the Study Brain
Open `01-Study-Brain/study-expert.md` and copy the entire prompt into a new Claude conversation.

Paste your study documents and study context into that same conversation.

Ask Claude: **"Analyze this study and prepare to help me understand it."**

### Step 4: Ask Questions
Now you can ask things like:
- "Why is this visit required?"
- "What should I look for during monitoring?"
- "Explain this endpoint."
- "Quiz me on eligibility criteria."
- "Show me the visit schedule as a diagram."

The Study Brain maintains context and understands your entire study.

### Step 5: Use Specialized Skills
As needed, use additional prompts from the toolkit:
- `/diagram` → Visual learning
- `/quiz` → Test yourself
- `/compare` → Compare documents
- `/visit-prep` → Prepare for monitoring visits
---

## 🚀 Getting Started with Claude

### The Fastest Way (5 Minutes, Copy-Paste Only)

1. **Go to claude.ai** (or your organization's Claude access)
2. **Create a New Project** called `Study [Name] — CRA Copilot`
3. **Upload your study documents** (Protocol, amendments, etc.)
4. **Open the `DIST/` folder** and copy-paste these files into Claude:
    - `MASTER-CRA-PROMPT.md` → Paste into **Project Instructions**
    - `STUDY-CONTEXT-TEMPLATE.md` → Fill in + paste into chat
5. **Done!** Start asking Claude questions about your study

### That's It!

You now have a personal Study & Learning Copilot that can:
- Explain protocols and procedures
- Create quizzes and flashcards
- Generate visit preparation checklists
- Find inconsistencies and gaps
- Answer your questions anytime
- Help you develop CRA judgment

**No GitHub, no coding, no technical knowledge required.** Just Claude.

---

## 📖 Detailed Setup Guide

For step-by-step instructions, see **`DIST/CLAUDE-SETUP.md`** (included in the distribution package).

---

## 🎯 Using Your CRA Copilot

Once set up, you can use powerful commands in Claude:

| What You Want | Type This |
|---|---|
| Explain a concept | `/teach inclusion criteria` |
| Simple explanation | `/eli5 protocol deviation` |
| Visual diagram | `/diagram patient journey` |
| Story format | `/story what happens at enrollment` |
| One-page reference | `/onepage critical procedures` |
| Create flashcards | `/quizlet eligibility criteria` |
| Take a quiz | `/quiz me on visit schedule` |
| Monitoring visit prep | `/visit-prep` |
| Find knowledge gaps | `/find-gaps in my understanding` |
| Practice scenarios | `/simulate a site issue` |
| Compare documents | `/compare protocol vs amendment` |

Or just ask naturally: *"Tell me about the primary endpoint"* or *"What should I look for during monitoring?"*

---

## 📁 How to Use This Repository

**For Clinical Research Associates (CRAs):**
- Download the **`DIST/`** folder (that's all you need!)
- See `DIST/START-HERE.md` for quick orientation
- See `DIST/CLAUDE-SETUP.md` for detailed setup

**For Managers/Training Teams:**
- Customize `00-START-HERE/MASTER-CRA-PROMPT.md` for your study specifics
- Share the entire repository or just the `DIST/` folder with your team
- Use `DIST/EXAMPLE-WORKFLOWS.md` to show how it works

**For Developers/Researchers:**
- See `INDEX.md` for complete file structure and descriptions
- See `PHASE-2-COMPLETION-SUMMARY.md` for technical details

---

## ❓ Common Questions

**Q: Is my study data safe?**  
A: You control what you upload to Claude. Follow your organization's policies for document sharing. See `DIST/PRIVACY-AND-SAFE-USE.md` for guidance.

**Q: Do I need to be technical?**  
A: No! This is copy-paste into Claude. No coding or GitHub knowledge needed.

**Q: Can I customize this for my study?**  
A: Yes! The Master Prompt and Study Context are templates you fill in.

**Q: What if Claude is slow or unavailable?**  
A: This toolkit works whenever Claude is available. No special setup needed.

**Q: Can I share this with my team?**  
A: Yes! Share the `DIST/` folder or the entire repository. Everyone can set up independently in Claude.

---

## 📞 Support & More Information

- **Quick Start:** See `DIST/START-HERE.md`
- **Detailed Setup:** See `DIST/CLAUDE-SETUP.md`
- **Example Workflows:** See `DIST/EXAMPLE-WORKFLOWS.md`
- **Command Reference:** See `DIST/CRA-SKILL-MENU.md`
- **Safety & Privacy:** See `DIST/PRIVACY-AND-SAFE-USE.md`
- **Full Index:** See `INDEX.md` (technical details and file structure)

---

## 🎓 Who Built This?

This toolkit was designed by CRAs and optimized specifically for how Clinical Research Associates work. Every prompt has been tested and refined for practical real-world use.

**Key Principle:** Your domain expertise matters more than AI. This system supports your judgment, it doesn't replace it.

---

## The System Architecture

```
                    ┌─────────────────────┐
                    │   STUDY CONTEXT     │
                    │ (Your study facts)  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    STUDY BRAIN      │
                    │ (Master prompt that │
                    │  understands entire │
                    │  study + maintains  │
                    │  context)           │
                    └──────────┬──────────┘
                               │
          ┌────────────────────┼────────────────────┐
          ▼                    ▼                    ▼
     LEARNING              ANALYSIS             WORKFLOW
          │                    │                    │
    ├─ Teach me            ├─ Document         ├─ Visit prep
    ├─ Diagrams               │  analysis       ├─ Visit followup
    ├─ Stories             ├─ Compare docs     ├─ Site issues
    ├─ Comparisons         ├─ Find gaps        ├─ Action items
    └─ Beginner→Expert     └─ Red flags        └─ Questions
          │                    │                    │
          └────────────────────┼────────────────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │  MEMORIZATION &     │
                    │  PRACTICE           │
                    │  Flashcards,        │
                    │  Quizzes,           │
                    │  Scenarios          │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │  BETTER CRA         │
                    │  JUDGMENT &         │
                    │  KNOWLEDGE          │
                    └─────────────────────┘
```

---

## Directory Structure

```
CRA-AI-Toolkit/
│
├── README.md                           ← You are here
├── QUICK-START.md                      ← Quick workflows (5 min)
├── CLAUDE-USAGE-GUIDE.md               ← How to use with Claude
│
├── 00-Foundation/
│   ├── master-instructions.md          ← Core principles
│   ├── study-context-template.md       ← Fill this in first
│   └── source-grounding-rules.md       ← Hallucination prevention
│
├── 01-Study-Brain/
│   ├── study-expert.md                 ← Master prompt (THE centerpiece)
│   ├── build-study-knowledge.md        ← Structured onboarding
│   ├── study-memory-refresh.md         ← Quick context reset
│   └── command-reference.md            ← Available commands
│
├── 02-Understand/
│   ├── teach-me.md                     ← Explain a concept clearly
│   ├── explain-simply.md               ← Simplify complex ideas
│   ├── explain-like-a-story.md         ← Story-based learning
│   ├── beginner-to-expert.md           ← Progressive difficulty
│   ├── compare-concepts.md             ← Compare two things
│   └── why-does-this-matter.md         ← Show relevance to CRA
│
├── 03-Visual-Learning/
│   ├── teach-with-diagram.md           ← Create diagrams
│   ├── process-flow.md                 ← Workflow diagrams
│   ├── study-timeline.md               ← Timeline visualization
│   ├── concept-map.md                  ← Relationship maps
│   ├── decision-tree.md                ← Decision logic
│   └── visit-workflow.md               ← Visit processes
│
├── 04-Memorization/
│   ├── quizlet-generator.md            ← Generate Quizlet cards
│   ├── flashcards.md                   ← Interactive flashcards
│   ├── multiple-choice-quiz.md         ← Multiple choice format
│   ├── scenario-quiz.md                ← Realistic situations
│   ├── rapid-review.md                 ← 10/5/2/30-second versions
│   └── spaced-repetition.md            ← Adaptive learning
│
├── 05-Document-Intelligence/
│   ├── protocol-analyzer.md            ← Deep protocol analysis
│   ├── document-summary.md             ← Structured summary
│   ├── one-page-summary.md             ← Single-page overview
│   ├── key-points.md                   ← Essential facts only
│   ├── red-flags.md                    ← Potential issues
│   ├── missing-information.md          ← Gaps and unknowns
│   └── terminology-extractor.md        ← Study acronyms/terms
│
├── 06-Cross-Document/
│   ├── compare-documents.md            ← Compare 2+ documents
│   ├── inconsistency-detector.md       ← Find conflicts
│   ├── requirement-matrix.md           ← Cross-document matrix
│   ├── change-impact-analysis.md       ← Protocol version changes
│   └── what-changed-detector.md        ← Old vs new analysis
│
├── 07-CRA-Workflow/
│   ├── monitoring-visit-prep.md        ← Before visit checklist
│   ├── monitoring-visit-followup.md    ← After visit tasks
│   ├── site-issue-analysis.md          ← Analyze site problems
│   ├── protocol-deviation-analysis.md  ← Deviation assessment
│   ├── query-analysis.md               ← Understand data queries
│   ├── action-items.md                 ← Action item management
│   └── question-generator.md           ← Generate smart questions
│
├── 08-Training/
│   ├── personal-cra-tutor.md           ← Adaptive tutor mode
│   ├── critical-thinking.md            ← Develop judgment
│   ├── scenario-simulator.md           ← Realistic scenarios
│   ├── mock-monitoring-visit.md        ← Practice visits
│   └── interview-prep.md               ← Interview training
│
├── 09-Advanced/
│   ├── risk-based-review.md            ← Risk categorization
│   ├── root-cause-analysis.md          ← Diagnose problems
│   ├── issue-triage.md                 ← Prioritize issues
│   ├── assumption-detector.md          ← Identify assumptions
│   └── knowledge-gap-detector.md       ← Find weak areas
│
└── templates/
    ├── study-context.md                ← Study reference (filled)
    ├── document-context.md             ← Single document info
    ├── site-context.md                 ← Site-specific info
    └── issue-context.md                ← Problem investigation
```

---

## Which Prompt Should I Use?

### "I don't understand this concept"
→ `02-Understand/teach-me.md`

### "I need to see this visually"
→ `03-Visual-Learning/teach-with-diagram.md`

### "I need to memorize these facts"
→ `04-Memorization/quizlet-generator.md` or `flashcards.md`

### "I have a monitoring visit next week"
→ `07-CRA-Workflow/monitoring-visit-prep.md`

### "These documents seem inconsistent"
→ `06-Cross-Document/inconsistency-detector.md`

### "I want to test my knowledge"
→ `04-Memorization/scenario-quiz.md` or `personal-cra-tutor.md`

### "I found a problem at the site"
→ `07-CRA-Workflow/site-issue-analysis.md`

### "I'm new and need to learn the whole study"
→ `01-Study-Brain/study-expert.md` + `build-study-knowledge.md`

### "I need to compare two protocol versions"
→ `06-Cross-Document/change-impact-analysis.md`

### "I want to identify hidden risks"
→ `09-Advanced/risk-based-review.md`

### "I don't know what I don't know"
→ `09-Advanced/knowledge-gap-detector.md`

---

## How to Get Better Answers from Claude

### 1. **Provide Full Study Context First**
Start by filling out `study-context-template.md` and load it into the Study Brain conversation. This prevents repetition and ensures consistency.

### 2. **Use the Study Brain for Everything**
Keep ONE Claude conversation going with the Study Brain and your study materials. Don't start new conversations for each question. Claude maintains context and can reference previous points.

### 3. **Use Specific Document Excerpts**
Instead of "What does this mean?" paste the actual text and say "What does this sentence mean?"

### 4. **Ask for Source Citations**
Request: "Cite the protocol section that supports your answer."

### 5. **Distinguish Between Fact and Interpretation**
Ask Claude: "Is this stated in the protocol, or is this your inference?"

### 6. **Leverage Comparison Prompts**
When comparing documents, use the specific comparison prompts rather than asking Claude to do it freeform.

---

## How to Work with PDFs

PDFs often need to be converted to text before use with Claude. Options:

1. **Copy-paste from PDF viewer** (simplest for shorter sections)
2. **Use PDF-to-text tools** (for full documents)
3. **Extract key sections** and provide context
4. **Provide page numbers** when referencing specific information

Claude works with pasted text, not file uploads of PDFs.

---

## How to Maintain Study Context

### The "Study Brain" Conversation
Create ONE Claude conversation that includes:
- Your `study-context-template.md`
- The full Study Brain prompt
- Your study documents (protocol, at minimum)

This conversation becomes your "knowledge base." Reference it whenever using specialized prompts.

### Switching Between Prompts
When using other prompts (diagrams, quizzes, etc.):
- Refer back to your Study Brain conversation for context
- OR include a brief context reminder in the specialized prompt
- You can have multiple Claude conversations, but the Study Brain should be your central hub

### Refreshing Context
Use `01-Study-Brain/study-memory-refresh.md` if Claude seems to have lost context during a long conversation.

---

## How to Avoid Hallucinations

This toolkit emphasizes **source grounding**. See `00-Foundation/source-grounding-rules.md` for detailed guidelines, but in brief:

### Claude Should:
- Only state facts that appear in your provided documents
- Clearly label inferences vs. facts
- Never invent study-specific information
- Ask clarifying questions when uncertain
- Cite the protocol section supporting important claims

### You Should:
- Provide complete study documents (or at least key sections)
- Correct Claude if it misstates something
- Verify important conclusions with actual documents
- Remember: Claude is a thinking tool, not an authority
- Always check critical information against the actual protocol

### Red Flags That Claude Is Hallucinating:
- ⚠️ "The protocol states..." but you don't see it
- ⚠️ Specific numbers, dates, or requirements with no source cited
- ⚠️ "This is a common regulatory requirement..." (without your document stating it)
- ⚠️ Complex medical conclusions about your study

If you spot these, ask Claude: **"Show me the exact text from the protocol supporting this."**

---

## Privacy & Data Safety

**IMPORTANT:** This toolkit may be used with confidential clinical research information.

### Before You Start:
- ✅ Check your organization's policies on AI tool usage
- ✅ Verify that Claude is approved for study documents at your organization
- ✅ Understand what information is confidential
- ✅ Know whether patient identifiable information is prohibited

### Best Practices:
- ✅ De-identify patient/site information whenever possible
- ✅ Use only approved tools for confidential study information
- ✅ Follow your organization's data protection procedures
- ✅ Don't assume that because a tool accepts data, the data is authorized for use
- ✅ Be cautious with unblinded information if blinding is critical to the study
- ✅ Follow all regulatory and company policies

### This Toolkit Does NOT Provide:
- Legal guidance on compliance
- Regulatory conclusions
- Company policy interpretation
- Security certifications

**You are responsible for ensuring compliance with your organization's policies and applicable regulations.**

---

## Limitations

### What This Toolkit Does Well:
- ✅ Helps you understand complex clinical research concepts
- ✅ Organizes and explains study documentation
- ✅ Supports learning and memorization
- ✅ Helps prepare for monitoring visits
- ✅ Identifies potential inconsistencies
- ✅ Supports critical thinking

### What This Toolkit Does NOT Do:
- ❌ Replace your actual study protocol or SOPs
- ❌ Make regulatory or compliance decisions
- ❌ Provide legal advice
- ❌ Substitute for qualified expert judgment
- ❌ Guarantee accuracy (always verify critical information)
- ❌ Handle real-time data or live clinical systems
- ❌ Make medical judgments about patient care

### Important Disclaimers:
- The toolkit works best with complete, current study documentation
- Claude's understanding depends on the information you provide
- Always verify critical information with the actual study documents
- When in doubt, ask your Study Manager, Sponsor, or Monitor
- Clinical research has legal and regulatory requirements beyond what this toolkit covers

---

## Getting the Most Value

### Week 1: Foundation
1. Fill out `study-context-template.md`
2. Start Study Brain with protocol
3. Explore the structure
4. Get comfortable with the system

### Week 2: Learning
1. Use teaching prompts to understand key concepts
2. Create visual diagrams of important processes
3. Generate flashcards for study facts
4. Take practice quizzes

### Week 3+: Application
1. Use workflow prompts for real monitoring visits
2. Use analysis prompts for document review
3. Use risk-based review for site issues
4. Continuously test and refine your knowledge

---

## Support & Troubleshooting

### "Claude says something I don't think is correct"
→ Follow the source-grounding rules: ask for the exact protocol text

### "Claude keeps forgetting things"
→ Reload the Study Brain conversation or use the memory-refresh prompt

### "I'm not getting useful output"
→ Check that you've provided sufficient context in the prompt
→ Review the specific prompt instructions carefully
→ Use more detailed follow-up questions

### "This prompt doesn't seem to fit my situation"
→ Adapt the prompt to your needs (they're starting points, not rigid templates)
→ Combine prompts for specialized use cases
→ Use critical-thinking mode to diagnose what you need

---

## Next Steps

1. **Read**: `QUICK-START.md` (specific workflows)
2. **Read**: `CLAUDE-USAGE-GUIDE.md` (practical tips)
3. **Do**: Fill out `00-Foundation/study-context-template.md`
4. **Do**: Start `01-Study-Brain/study-expert.md` with your protocol
5. **Explore**: Other prompts as needed

---

## Philosophy

This toolkit is built on the belief that:

- **Clinical research is complex**, but learnable through structured, multi-modal learning
- **CRAs need better tools** to manage complex study knowledge
- **AI can augment CRA judgment**, not replace it
- **Source grounding matters** — no hallucinated compliance claims
- **Practice and feedback** build expertise faster than passive reading
- **Visual learning, storytelling, and scenarios** work better than lists
- **A CRA's time is valuable** — tools should minimize busywork and maximize insight

This toolkit reflects that philosophy.

---

**Ready to get started?** Open `QUICK-START.md` and follow the workflow that matches your immediate need. You'll be productive in minutes.
