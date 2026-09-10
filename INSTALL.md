# 🚀 Installation & Setup Guide: CRA AI Toolkit in Claude

**Time needed:** 5-10 minutes  
**Technical skill required:** None (copy-paste only)  
**Cost:** Free (uses Claude subscription you already have)

---

## WHAT YOU'LL HAVE WHEN DONE

After setup, you'll have a personal **Claude Project** that acts as your:
- Study expert (answers questions about your protocol)
- Learning coach (creates quizzes, explains concepts)
- Monitoring visit assistant (generates checklists and prep materials)
- Document analyst (finds gaps, inconsistencies, risks)
- Memory aid (flashcards, one-page reference sheets)

All powered by Claude, all in one place, all with your study documents.

---

## STEP-BY-STEP INSTALLATION

### BEFORE YOU START
Gather your study documents:
- ✅ Protocol (most important)
- ✅ Protocol Amendments (if any)
- ✅ SAP or Study Design Document (optional but recommended)
- ✅ Monitoring Plan or Site Instructions (if available)
- ✅ Visit Schedule or Timeline (if separate document)
- ✅ Any other documents you need for your CRA work

⚠️ **Check with your manager/compliance:** Make sure your organization approves uploading these documents to Claude.

---

### STEP 1: Open Claude and Create a Project (2 minutes)

1. **Open your web browser** and go to **https://claude.ai**
2. **Log in** with your Claude account (if your organization uses Claude through a different system, use that instead)
3. Look for **Projects** in the left sidebar menu or top menu
4. Click **"New Project"** or **"+ Create Project"**
5. **Name your project:**
   ```
   Study [Protocol Number] — CRA Copilot
   ```
   Example: `Study ABC-2024-001 — CRA Copilot`

6. Click **Create** or **Save**

You're now in an empty project. ✅

---

### STEP 2: Upload Your Study Documents (2-3 minutes)

1. In your Claude Project, look for an **Upload**, **Attach**, or **+** button
2. Click it
3. Select your documents from your computer:
   - Start with the **Protocol** (most important)
   - Add amendments, SAP, or other key documents
   - You can upload 10+ documents if needed
4. Wait for each document to finish uploading (Claude will show a ✅)

✅ Claude can now "read" all your study documents.

**Note:** Documents stay private to this project. Only you can see them.

---

### STEP 3: Add the Master Prompt to Project Instructions (2 minutes)

This tells Claude to become your **CRA Study & Learning Copilot.**

1. In your Claude Project, find **Settings** (⚙️ icon, usually top right)
2. Click **Settings** or **Project Settings**
3. Find the **"Instructions"** field (might be labeled "System Prompt", "Context", or "Custom Instructions")
4. **Download or open** this file: `MASTER-CRA-PROMPT.md`
   - Location: In the `DIST/` folder of this toolkit
   - Or copy it from your computer
5. **Copy the entire file:**
   - Select all text (Ctrl+A or Cmd+A)
   - Copy (Ctrl+C or Cmd+C)
6. **Paste into Claude's Instructions field:**
   - Click in the Instructions field
   - Paste (Ctrl+V or Cmd+V)
7. **Save** the settings

Claude has now been instructed to be your personal CRA Study & Learning Copilot. ✅

---

### STEP 4: (Highly Recommended) Add Your Study Context (1-2 minutes)

**Study Context** tells Claude specific facts about YOUR study. This makes all answers tailored to your protocol, not generic.

1. **Download or open** this file: `STUDY-CONTEXT-TEMPLATE.md`
   - Location: In the `DIST/` folder of this toolkit
2. **Fill in the blanks** with your study information:
   - Study name and protocol number
   - Therapeutic area (what condition it treats)
   - Study phase (Phase 1, 2, 3, 4, observational, etc.)
   - Study design (randomized, open-label, cross-over, etc.)
   - Patient population and key inclusion/exclusion criteria
   - Number of visits and visit schedule
   - Primary and secondary endpoints
   - Study duration
   - Any other key details
3. **Save your filled-in template** (or just copy it)
4. In your Claude Project chat window, **paste your context** as the **first message**
5. Send it

Claude now has context about YOUR study and will tailor everything. ✅

---

### STEP 5: Start Using Your CRA Copilot (Now!)

You're ready! Claude now has:
- ✅ Your study documents
- ✅ Master CRA Prompt (instructions)
- ✅ Your study context (optional but recommended)

**Try asking:**
```
Tell me about the primary endpoint and why it matters for CRA work.
```

or

```
/teach inclusion criteria
```

---

## QUICK COMMAND REFERENCE

Use these commands for faster interactions:

| **I Want To...** | **Type This** | **Example** |
|---|---|---|
| Understand something | `/teach [topic]` | `/teach primary endpoint` |
| Simple explanation | `/eli5 [topic]` | `/eli5 protocol deviation` |
| See a diagram | `/diagram [topic]` | `/diagram patient journey` |
| Story format | `/story [topic]` | `/story what happens at enrollment` |
| One-page summary | `/onepage [topic]` | `/onepage critical procedures` |
| Create flashcards | `/quizlet [topic]` | `/quizlet inclusion criteria` |
| Take a quiz | `/quiz [topic]` | `/quiz me on visits` |
| Prep for monitoring | `/visit-prep` | `/visit-prep` |
| Find knowledge gaps | `/find-gaps` | `/find-gaps in my understanding` |
| Compare two things | `/compare A vs B` | `/compare protocol version 1 vs amendment` |
| Practice scenarios | `/simulate [situation]` | `/simulate a major protocol deviation` |
| Generate questions | `/questions` | `/questions to ask at site visit` |

**Or just ask naturally:**
- "What should I look for during monitoring?"
- "Why is this visit required?"
- "Quiz me on the visit schedule"
- "Show me the enrollment criteria as a table"

---

## EXAMPLE FIRST QUESTIONS TO ASK

Once you're set up, here are good questions to start with:

### 1. "Understand the Big Picture"
```
/teach study design and objectives
```
Claude will explain the whole study design and why it's structured this way.

### 2. "Learn the Patient Journey"
```
/diagram patient journey from enrollment to final visit
```
Claude will create a visual timeline of what patients do.

### 3. "Quick Knowledge Check"
```
/quiz me on inclusion criteria
```
Claude will quiz you with 5 multiple-choice questions.

### 4. "Prepare for a Visit"
```
/visit-prep
```
Claude will create a monitoring visit checklist.

### 5. "Find What You Don't Know"
```
/find-gaps in my understanding of the study
```
Claude will identify areas that might be unclear or need more attention.

---

## ❓ TROUBLESHOOTING

### "The documents didn't upload properly"
- Check file size (Claude works best with documents under 10 MB)
- Try uploading one document at a time
- Refresh the page and try again

### "Claude doesn't remember the Master Prompt"
- Make sure you pasted it into **Project Instructions**, not into a chat message
- Save the settings (there should be a Save button)
- Start a new message in the project; Claude should now recognize commands like `/teach`

### "Claude gives generic answers instead of study-specific"
- You might not have pasted the Master Prompt correctly
- Or you haven't added your study context yet
- Try pasting your study context as the first chat message

### "I'm not getting the right kind of answers"
- Try being more specific: instead of "Tell me about the study", try `/teach primary endpoint`
- Add more details in your study context
- Tell Claude: "Only use information from the documents I provided"

### "I uploaded the wrong document"
- You can delete a document from a Claude project
- In your Project Settings, find "Files" or "Documents"
- Delete the wrong file and upload the correct one

### "I forgot to add the Master Prompt"
- No problem! Go to Project Settings → Instructions
- Paste the Master Prompt now
- Refresh the chat window

---

## 🔒 PRIVACY & SECURITY

**Your documents are private:**
- Only you can see documents in your Claude Project
- Claude doesn't use your documents to train its models (unless you opt into sharing for product improvement)
- Your organization controls how you use Claude
- Follow your company's policies for document security

**Best practices:**
- Only upload documents you're authorized to share
- Check with compliance if you're unsure
- Don't upload documents with unnecessary patient names or identifying information
- De-identify sensitive information if possible

See `DIST/PRIVACY-AND-SAFE-USE.md` for more detailed privacy guidance.

---

## 📚 EXAMPLE WORKFLOWS

### Workflow 1: "I Just Got a New Study"
1. Upload protocol
2. Add Master Prompt to settings
3. Add study context
4. `/teach study design and objectives`
5. `/diagram patient journey`
6. `/onepage critical procedures`
7. `/quiz me` to test yourself

### Workflow 2: "Monitoring Visit Tomorrow"
1. `/visit-prep` — get comprehensive checklist
2. `/onepage critical procedures for [Site Name]`
3. `/questions to ask the site`
4. `/quiz me on key requirements`

### Workflow 3: "Learning & Memorizing the Study"
1. `/teach primary endpoint`
2. `/eli5 inclusion criteria`
3. `/quizlet [topic]` — export to Quizlet app for more practice
4. `/quiz me` → test yourself
5. `/find-gaps` — identify unclear areas

---

## ✅ YOU'RE DONE!

You now have a personal Study & Learning Copilot.

**Your CRA Copilot can:**
- Answer questions about your study anytime
- Create learning materials (quizzes, flashcards, summaries)
- Help you prepare for monitoring visits
- Find inconsistencies or gaps in documentation
- Explain complex concepts simply
- Help you develop CRA judgment

**Next steps:**
- Start with a simple question: `Tell me about the primary endpoint`
- Explore commands: Try `/teach`, `/diagram`, `/quiz`
- Share this with your team — they can set up independently

---

## 📞 NEED MORE HELP?

- **Command reference:** See `DIST/CRA-SKILL-MENU.md`
- **Example workflows:** See `DIST/EXAMPLE-WORKFLOWS.md`
- **Privacy & safety:** See `DIST/PRIVACY-AND-SAFE-USE.md`
- **Full toolkit:** See `INDEX.md` for complete file structure
- **Technical details:** See `PHASE-2-HANDOFF.md` for how the toolkit was built

---

**Questions?** Your CRA Copilot is ready to help. Just ask!
