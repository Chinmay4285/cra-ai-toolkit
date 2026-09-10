# How to Set Up CRA AI Copilot with Claude

This guide walks you through setting up your personal CRA Study & Learning Copilot. **It takes about 5 minutes.**

You do **NOT** need to understand GitHub, programming, or technical concepts. This is just copying and pasting text into Claude.

---

## STEP 1: Open Claude

Go to **https://claude.ai** in your web browser.

If your organization uses Claude through a different system or app, use that instead.

Log in if needed.

---

## STEP 2: Create a New Project

A **Project** in Claude is a dedicated space for all your conversation about one study.

1. Click the **"Projects"** menu or button
2. Click **"New Project"** or **"+ New"**
3. Give it a name like:
   - `Study ABC-123 — CRA Copilot`
   - `XYZ Protocol — Learning & Reference`
   - `Study 2024-001 Learning Hub`

   (Pick any name that helps you identify this study)

4. Click **Create** or **Save**

You should now be in an empty project.

---

## STEP 3: Upload Your Study Documents

Claude can read documents you upload. Gather the study documents you're authorized to use:

### Recommended Documents to Upload:
- **Protocol** — The main study document (usually a PDF)
- **Protocol Amendments** — If there are changes to the original protocol
- **SAP** (Statistical Analysis Plan) — If available and authorized
- **ICF** (Informed Consent Form) — If authorized
- **Monitoring Plan** — CRA-specific guidance
- **Study Manuals** — Procedure manuals, safety manuals, etc.
- **Other Approved Documents** — IB (Investigator's Brochure), CRF instructions, etc.

### ⚠️ IMPORTANT — Check Before Uploading:
- **Is this document authorized for AI use in your organization?** Ask your supervisor or compliance team if you're unsure
- **Does it contain unnecessary patient information?** De-identify if possible
- **Are there confidentiality restrictions?** Follow your company's policies

### How to Upload:
1. In your Claude Project, look for an **"Upload"**, **"Attach"**, or **"+"** button
2. Click it
3. Select your document files from your computer
4. Confirm upload

Claude will read and remember these documents throughout your conversation.

---

## STEP 4: Add the Master Prompt to Project Instructions

The **Master CRA Prompt** tells Claude to become your Study & Learning Copilot. This is the most important step.

### How to Add Instructions:

1. In your Claude Project, find **"Settings"**, **"Project Settings"**, or a **"⚙️"** icon
2. Find the **"Instructions"** field (sometimes called "System Prompt", "Context", or "Project Instructions")
3. Open the file `MASTER-CRA-PROMPT.md` from this folder
4. **Select All** the text (Ctrl+A or Cmd+A)
5. **Copy** (Ctrl+C or Cmd+C)
6. Go back to Claude's Instructions field
7. **Paste** (Ctrl+V or Cmd+V)
8. Click **Save** or confirm

Claude should now understand its role as your CRA Copilot.

---

## STEP 5: (Optional but Recommended) Add Your Study Context

**Study Context** tells Claude key facts about your specific study. This helps Claude tailor all answers to your study instead of being generic.

### How to Add Context:

1. Open the file `STUDY-CONTEXT-TEMPLATE.md` from this folder
2. **Fill in the blanks** with your study information
   - Study Name
   - Protocol Number
   - Therapeutic Area
   - Study Design
   - Visit Schedule
   - Key Eligibility Criteria
   - Primary Endpoint
   - etc.

   You don't need to fill in everything. Fill in what you know. You can add more later.

3. When done, **Copy** your filled context (Ctrl+A, then Ctrl+C)
4. Go to Claude's chat window (in your Project)
5. Paste your context in the first message
6. Send the message

Claude will remember this context for the rest of your conversation.

---

## STEP 6: Start Chatting

You're ready! Claude now has:
✅ Your study documents  
✅ Master CRA Prompt (instructions)  
✅ Study Context (optional)

Try asking Claude something about your study:

**Examples:**
- `Tell me about the primary endpoint`
- `What are the inclusion criteria?`
- `Create a one-page summary of the protocol`
- `/diagram patient journey`
- `/quiz me on the visit schedule`
- `/visit-prep`

---

## OPTIONAL: Use Commands for Faster Interactions

The Master Prompt supports **commands** for common tasks. You can type:

```
/teach inclusion criteria
```

Instead of:

```
Please explain the inclusion criteria to me clearly with study-specific details and explain why it matters for CRA work.
```

Both work fine. Use whichever feels natural to you.

### Quick Command Reference:
- **`/teach`** — Explain a concept
- **`/eli5`** — Explain simply
- **`/story`** — Tell it as a narrative
- **`/diagram`** — Create a visual
- **`/summarize`** — Quick summary
- **`/onepage`** — One-page cheat sheet
- **`/quizlet`** — Create flashcards
- **`/quiz`** — Test yourself
- **`/visit-prep`** — Prepare for monitoring visit
- **`/simulate`** — Practice scenario

For a complete list, see `CRA-SKILL-MENU.md`.

---

## TROUBLESHOOTING

### "I uploaded documents but Claude can't see them"
- Wait a few seconds for documents to fully upload
- Reload the page
- Try uploading again
- Check that the files are PDFs, Word docs, or text (Claude supports most formats)

### "Claude is giving me generic answers about CRA work"
- Make sure you pasted the Master CRA Prompt into Project Instructions (not just in chat)
- Provide your Study Context (fill in `STUDY-CONTEXT-TEMPLATE.md` and paste it)
- Ask Claude to be more specific: "Answer based on this specific study's protocol"

### "Claude forgot my study documents in a long conversation"
- Use the `/reset` command to refresh context
- Paste your Study Context again
- For very long conversations, start a new conversation in the same Project (it will still have the Instructions and documents)

### "I want to change something"
- You can edit Claude's Project Instructions anytime (go to Settings)
- You can update your Study Context anytime (paste new version in chat)
- You can upload more documents anytime (click Upload again)

### "The commands aren't working"
- Commands (like `/teach`, `/quiz`) work naturally in Claude conversation
- If a command doesn't work, you can always ask conversationally:
  - Instead of `/teach inclusion criteria`
  - Say: `Can you explain the inclusion criteria clearly?`
- Both approaches work fine

---

## MANAGING MULTIPLE STUDIES

If you're working on multiple studies:
- Create a **separate Project for each study**
- Name them clearly (Study ABC vs. Study XYZ)
- Upload each study's documents to its own Project
- Each Project will have the same Master CRA Prompt, so they'll work the same way

Claude keeps conversations separate by Project, so you won't mix up studies.

---

## SECURITY & PRIVACY

✅ **Safe Practices:**
- Only upload documents your organization permits
- De-identify unnecessary patient information
- Follow your company's AI usage policy
- Don't share your Claude Project link with others (unless authorized)
- Remember: Claude stores conversations for safety review

⚠️ **Check First:**
- Ask your supervisor if unsure about uploading something
- Check your company's AI usage policy
- Verify the documents are authorized for this use

📖 **More Detail:**
See `PRIVACY-AND-SAFE-USE.md` in this folder for full guidance.

---

## NEXT STEPS

1. ✅ You've read this guide
2. 🔧 Complete Steps 1-6 above (takes ~5 minutes)
3. 📖 Try an example from `EXAMPLE-WORKFLOWS.md`
4. 🎓 Use `CRA-SKILL-MENU.md` as a quick reference

**That's it. You're ready to learn your study with Claude!**

---

## QUICK REFERENCE

| Step | What to Do | Time |
|------|-----------|------|
| 1 | Open claude.ai | 30 sec |
| 2 | Create new Project | 1 min |
| 3 | Upload study documents | 2 min |
| 4 | Add Master Prompt to Instructions | 1 min |
| 5 | (Optional) Add Study Context | 1 min |
| 6 | Start chatting | 30 sec |
| **Total** | | **~5 minutes** |

---

**Questions?** Try asking Claude directly! It can explain anything in this toolkit.

**Ready?** Open Claude now. 🚀
