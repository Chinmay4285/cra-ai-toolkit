# 📖 Complete Guide: Using CRA AI Toolkit in Claude

Welcome! This document walks you through everything you need to know to use this toolkit.

**TL;DR:** Download the `DIST/` folder, copy-paste two files into Claude, and you're done. Takes 5 minutes.

---

## TABLE OF CONTENTS

1. [What This Is](#what-this-is)
2. [Who This Is For](#who-this-is-for)
3. [Quick Start (5 Minutes)](#quick-start-5-minutes)
4. [Detailed Installation Guide](#detailed-installation-guide)
5. [How to Use Commands](#how-to-use-commands)
6. [Example Workflows](#example-workflows)
7. [FAQ & Troubleshooting](#faq--troubleshooting)
8. [Safety & Privacy](#safety--privacy)

---

## WHAT THIS IS

**CRA AI Toolkit** is a collection of Claude prompts and templates specifically designed for Clinical Research Associates.

It transforms Claude into a personal **Study Expert, Learning Coach, and Monitoring Visit Assistant** that:

- 📚 **Explains** complex protocols and procedures
- 🎓 **Teaches** through quizzes, stories, diagrams, and flashcards
- ✅ **Prepares** you for monitoring visits with checklists
- 🔍 **Finds** inconsistencies, gaps, and risks in documents
- 🧠 **Helps you develop** CRA judgment through scenarios and practice
- 📝 **Creates** reference materials (one-pagers, flowcharts, timelines)

**Key Principle:** Everything is grounded in YOUR study documents. No generic answers. No hallucinations.

---

## WHO THIS IS FOR

✅ **Perfect for:**
- Clinical Research Associates learning a new study
- CRAs preparing for monitoring visits
- Site coordinators needing rapid study training
- Anyone who needs to deeply understand clinical research protocols
- Teams wanting structured Claude integration into their workflow

✅ **No prior experience needed:**
- No AI knowledge required
- No coding or technical skills
- No GitHub experience
- Just you, Claude, and your study documents

---

## QUICK START (5 MINUTES)

### What You'll Need:
- A Claude account (free or subscription at https://claude.ai)
- Your study Protocol (PDF or text)
- 5 minutes

### The Process:
1. **Create a Claude Project**
2. **Upload your study documents**
3. **Paste two files** from this toolkit:
   - `MASTER-CRA-PROMPT.md` → Project Instructions
   - `STUDY-CONTEXT-TEMPLATE.md` → First chat message (filled in)
4. **Done!** Start asking questions

### That's It!

You now have a personal Study Copilot.

---

## DETAILED INSTALLATION GUIDE

### Step 1: Get the Files (1 minute)

**Option A: Just the Essential Files (Recommended for CRAs)**
- Download the **`DIST/` folder** from this repository
- This folder has everything you need (8 files, ~50 KB)
- Discard the rest of the repository

**Option B: Everything (For Managers/Researchers)**
- Clone or download the entire repository
- See `INDEX.md` for what each file does

### Step 2: Open Claude (30 seconds)

1. Go to https://claude.ai (or your organization's Claude system)
2. Click **Projects** in the left sidebar
3. Click **New Project** or **+ Create**
4. Name it: `Study [Name] — CRA Copilot`
   - Example: `Study ABC-2024-001 — CRA Copilot`
5. Click **Create**

### Step 3: Upload Documents (1-2 minutes)

1. In your Claude Project, find the **Upload** or **Attach** button (+)
2. Select your study documents:
   - Start with **Protocol**
   - Add **amendments**, **SAP**, **monitoring plan**, etc.
   - You can upload 10+ documents
3. Wait for all files to upload (✅ checkmark appears)

Claude can now "read" your entire study.

### Step 4: Add Master Prompt (1 minute)

1. Open file: **`DIST/MASTER-CRA-PROMPT.md`**
2. Select all text: **Ctrl+A** (Windows) or **Cmd+A** (Mac)
3. Copy: **Ctrl+C** or **Cmd+C**
4. In Claude Project, click **Settings** (⚙️)
5. Find **"Instructions"** field
6. Paste: **Ctrl+V** or **Cmd+V**
7. Click **Save**

Claude is now your CRA Study Copilot!

### Step 5: Add Study Context (1 minute, Optional but Recommended)

1. Open file: **`DIST/STUDY-CONTEXT-TEMPLATE.md`**
2. Fill in the blanks:
   - Study name, protocol number
   - Design, phases, visits
   - Key criteria, endpoints
   - Anything you want Claude to know
3. Copy: **Ctrl+A** → **Ctrl+C**
4. In Claude chat, paste: **Ctrl+V**
5. Send the message

Claude now understands YOUR specific study.

### Step 6: Start Using!

Try these first questions:
```
Tell me about the primary endpoint and why it matters
```

```
/teach inclusion criteria
```

```
/diagram patient journey
```

---

## HOW TO USE COMMANDS

The toolkit supports 20+ **commands** for common CRA tasks.

### Command Format

Type commands like this:
```
/command [topic]
```

Example:
```
/teach primary endpoint
```

### Available Commands by Category

#### 📚 **Understanding**
| Command | Use | Example |
|---------|-----|---------|
| `/teach [topic]` | Explain clearly with study context | `/teach inclusion criteria` |
| `/eli5 [topic]` | Explain simply (like you're 5) | `/eli5 protocol deviation` |
| `/story [topic]` | Explain through narrative | `/story what happens at enrollment` |
| `/compare A vs B` | Highlight differences | `/compare protocol v1 vs v2` |
| `/compare_studies A and B` | Compare two complete studies in detail | `/compare_studies Study ABC-101 and Study XYZ-202` |

#### 🎨 **Visual Learning**
| Command | Use | Example |
|---------|-----|---------|
| `/diagram [topic]` | Create flowchart/timeline/map | `/diagram patient journey` |
| `/timeline` | Full study timeline | `/timeline` |
| `/visit-workflow` | Procedures for a visit | `/visit-workflow visit 2` |

#### 📝 **Memorization & Testing**
| Command | Use | Example |
|---------|-----|---------|
| `/onepage [topic]` | One-page reference sheet | `/onepage critical procedures` |
| `/quizlet [topic]` | Create Quizlet flashcards | `/quizlet inclusion criteria` |
| `/quiz [topic]` | Interactive multiple-choice test | `/quiz me on visits` |
| `/testme [topic]` | Quiz with teaching included | `/testme primary endpoint` |
| `/rapid-review` | 2-minute fact review | `/rapid-review` |

#### 📄 **Document Analysis**
| Command | Use | Example |
|---------|-----|---------|
| `/summarize [doc]` | Comprehensive summary | `/summarize protocol` |
| `/key-points [doc]` | Essential facts only | `/key-points SAP` |
| `/red-flags [doc]` | Find risks/gaps/ambiguities | `/red-flags monitoring plan` |
| `/terms [doc]` | Extract & define terminology | `/terms protocol` |

#### 🔍 **Finding Issues**
| Command | Use | Example |
|---------|-----|---------|
| `/detect` | Find conflicts between documents | `/detect` |
| `/what-changed [v1 → v2]` | Show amendment impacts | `/what-changed v1 → amendment 1` |
| `/find-gaps` | Identify missing understanding | `/find-gaps in my knowledge` |

#### 🏥 **CRA Workflow**
| Command | Use | Example |
|---------|-----|---------|
| `/visit-prep [site]` | Pre-visit checklist | `/visit-prep site ABC` |
| `/visit-followup` | Post-visit action items | `/visit-followup` |
| `/deviation [situation]` | Assess if it's a deviation | `/deviation patient missed window` |
| `/questions` | Generate CRA questions | `/questions to ask at site visit` |
| `/issue-analysis [problem]` | Analyze a site issue | `/issue-analysis data missing` |

#### 🎓 **Learning & Development**
| Command | Use | Example |
|---------|-----|---------|
| `/simulate [scenario]` | Practice realistic scenarios | `/simulate major protocol deviation` |
| `/risk-review` | Review study risks | `/risk-review` |
| `/mentor [question]` | Get guidance from expert | `/mentor how should I handle this` |

#### 🔄 **Context**
| Command | Use | Example |
|---------|-----|---------|
| `/recap` | Review today's learning | `/recap` |
| `/reset [new context]` | Reset context | `/reset [paste new context]` |

---

## EXAMPLE WORKFLOWS

### Workflow 1: "I Just Got a New Study — Understand It Fast"

You're new to Study ABC and have 1 hour to get oriented. Here's what to do:

**Setup (5 min):**
1. Create Claude Project
2. Upload protocol
3. Add Master Prompt
4. Add study context

**Learning (55 min):**
1. **/teach study design and objectives** (5 min)
2. **/diagram patient journey** (5 min)
3. **/onepage critical procedures** (5 min)
4. **/quiz me on inclusion criteria** (10 min)
5. **/find-gaps in my understanding** (10 min)
6. Ask specific questions about unclear areas (15 min)

**Result:** You understand the study design, patient pathway, critical procedures, inclusion criteria, and know what to study further.

---

### Workflow 2: "Monitoring Visit Tomorrow — Quick Prep"

You have a monitoring visit at Site ABC tomorrow. Here's your 1-hour prep:

1. **/visit-prep site ABC** (15 min) — Get comprehensive checklist
2. **/onepage critical procedures for site ABC** (10 min) — Quick reference
3. **/questions to ask at site** (10 min) — Generate smart questions
4. **/quiz me on protocol requirements** (10 min) — Knowledge check
5. **/rapid-review** (5 min) — 2-minute fact review
6. Print and review offline

**Result:** You're confident, prepared, and have a structured checklist and question list.

---

### Workflow 3: "Learn & Memorize the Study — Deep Learning"

You want to master this study for future reference. Multi-session approach:

**Session 1 - Concepts:**
- `/teach primary endpoint`
- `/eli5 inclusion criteria`
- `/story patient journey`

**Session 2 - Visual:**
- `/diagram patient journey`
- `/diagram visit schedule`
- `/timeline from enrollment to follow-up`

**Session 3 - Memorization:**
- `/quizlet critical procedures` → Export to Quizlet app
- `/quiz me` → Test yourself
- `/testme inclusion criteria` → Quiz with teaching

**Session 4 - Application:**
- `/simulate inclusion edge case` → Practice judgment
- `/simulate protocol deviation scenario` → Develop decision-making
- `/risk-review` → Understand risks

**Result:** You deeply understand the study and can teach others.

---

### Workflow 4: "Compare Two Protocol Versions"

Amendment just came out. How different is it?

1. Upload both versions (original + amendment)
2. `/what-changed original → amendment 1`
3. `/compare original vs amendment`
4. `/detect inconsistencies`
5. Ask about specific changes that affect your site

**Result:** You know exactly what changed and what you need to do differently.

---

## FAQ & TROUBLESHOOTING

### **Q: I uploaded documents but Claude doesn't know about them**

**A:** Make sure you're in a Claude **Project**, not a regular chat. Projects preserve uploaded documents. Regular chats don't.

**How to check:**
- You should see your Project name at the top of the page
- Project has "Files" or "Documents" showing your uploads
- If you're in a regular chat, create a new Project

---

### **Q: Claude doesn't recognize my commands (like `/teach`)**

**A:** The Master Prompt wasn't added to Project Instructions.

**How to fix:**
1. Go to Project **Settings** (⚙️)
2. Find **"Instructions"** field
3. Paste entire `MASTER-CRA-PROMPT.md` file
4. Click **Save**
5. Refresh the page
6. Try `/teach` again

---

### **Q: Claude gives generic answers instead of study-specific**

**A:** Claude needs more context. Either:

1. **You didn't add the Master Prompt** (see above)
2. **You didn't paste Study Context** as first message
3. **Your Study Context was too vague**

**How to fix:**
- Open `STUDY-CONTEXT-TEMPLATE.md`
- Fill in all the blanks thoroughly
- Paste into chat
- Try your question again

---

### **Q: I'm not sure if I should upload this document to Claude**

**A:** Check with your manager or compliance team. Claude doesn't use your documents to train its model (unless you opt in), but follow your organization's policies.

Generally safe to upload:
- ✅ Study protocol (public document, needed for work)
- ✅ Monitoring plans
- ✅ Visit schedules
- ✅ Procedure manuals

Generally avoid:
- ❌ Documents with patient names
- ❌ Actual patient data
- ❌ Highly confidential info not needed for your work

---

### **Q: Can I share my Claude Project with my team?**

**A:** No, Claude Projects are personal. But you can:
1. Share the DIST/ folder
2. Each team member sets up their own Project
3. Everyone follows the same setup steps

Everyone ends up with their own personal Study Copilot.

---

### **Q: What if I forget my study context?**

**A:** You can:
1. Paste it again in a new message (Claude will remember)
2. Use `/reset [new context]` command
3. Create a new Project and start over

---

### **Q: Can I use this for multiple studies?**

**A:** Yes! Create a separate Claude Project for each study.

Example:
- Project 1: `Study ABC-2024 — CRA Copilot`
- Project 2: `Study XYZ-2025 — CRA Copilot`

Each project is independent with its own documents and context.

---

### **Q: Claude seems confused or gives contradictory answers**

**A:** Tell Claude directly:
```
You're giving me contradictory information. Please re-read the protocol 
section on [topic] and clarify. Include where your information comes from.
```

Claude will acknowledge the confusion and reference specific document sections.

---

## SAFETY & PRIVACY

### Document Security
- ✅ **Stored securely** — Claude encrypts documents
- ✅ **Private to you** — Only you can see your Project
- ✅ **Not used for training** — Your data doesn't train Claude (unless you opt in)
- ✅ **You control it** — You can delete documents anytime

### Best Practices
1. **Only upload authorized documents** — Check with compliance
2. **De-identify if possible** — Remove unnecessary patient names
3. **Don't paste patient data** — Chat messages are less private than uploaded files
4. **Follow company policy** — Use Claude the way your organization approves

### Red Flags
- ❌ Don't upload actual patient data/case report forms
- ❌ Don't paste participant names
- ❌ Don't upload documents marked "Confidential - Limited Distribution" without permission
- ❌ Don't bypass your organization's AI usage policy

---

## ADDITIONAL RESOURCES

In the `DIST/` folder you'll find:

- **INSTALL.md** — Step-by-step installation guide
- **START-HERE.md** — Quick orientation
- **CRA-SKILL-MENU.md** — Printable command reference
- **EXAMPLE-WORKFLOWS.md** — Detailed example scenarios
- **PRIVACY-AND-SAFE-USE.md** — Safety & compliance guidance

In the full repository, also see:

- **INDEX.md** — Complete file structure and descriptions
- **PHASE-2-COMPLETION-SUMMARY.md** — Technical overview
- **PHASE-2-HANDOFF.md** — How this was built

---

## NEXT STEPS

1. ✅ Download the `DIST/` folder
2. ✅ Follow the installation steps above
3. ✅ Try your first command: `/teach study design`
4. ✅ Explore more commands
5. ✅ Share with your team!

---

## QUESTIONS?

Start a conversation in Claude with your Study Copilot. It can help you figure things out!

Example question:
```
I'm not sure how to use this toolkit. Can you walk me through getting started?
```

---

**Happy learning! 🚀**
