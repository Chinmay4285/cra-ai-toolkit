# Guide: How to Use These Prompts with Claude

This guide explains the practical mechanics of using this toolkit effectively with Claude.

---

## The Core Principle: Context Matters

The single most important principle:

**One Claude conversation + all your study materials = Smart Claude that understands your entire study**

Multiple scattered conversations = Claude answering each question in isolation (worse).

---

## Step 1: Set Up Your Main Study Brain Conversation

### First Time: Create Your Study Context

1. **Download and fill out:** `00-Foundation/study-context-template.md`
2. **Fill in basic facts:**
   - Study name, sponsor, protocol number
   - Therapeutic area, indication, phase
   - Study design, patient population
   - Treatment arms, visit schedule
   - Primary endpoints, key procedures
3. **Save this file.** You'll use it repeatedly.

### Create the Conversation

1. **Open a new Claude conversation**
2. **In the first message to Claude, include:**

   ```
   PART 1: Copy the entire Study Brain prompt
   [Get from: 01-Study-Brain/study-expert.md]
   
   PART 2: Your study context
   [Paste your completed study-context-template.md]
   
   PART 3: Your protocol
   [Paste full text of current study protocol]
   
   PART 4: Request
   [Your first question or: "Please analyze this study and prepare to help me understand it."]
   ```

3. **Send it to Claude**

4. **Claude responds** with structured understanding of your study

5. **KEEP THIS CONVERSATION OPEN.** This is your Study Brain session.

### Result:
You now have a Claude conversation that knows your entire study and can answer follow-up questions with full context.

---

## Step 2: Ask Questions in the Study Brain Conversation

Once the Study Brain is loaded with your protocol, you can ask:

- "Explain the eligibility criteria"
- "Why is screening visit required?"
- "What's the difference between the primary and secondary endpoints?"
- "Show me the visit schedule as a diagram"
- "Create flashcards for the safety requirements"
- "Quiz me on the visit windows"

**Claude maintains context.** It remembers your study, your previous questions, and your level of understanding. This is powerful because:
- You don't repeat information
- Claude gives answers tailored to YOUR study (not generic)
- You build on previous conversations
- It's much faster

---

## Step 3: When to Use Specialized Prompts

The Study Brain handles most needs. But for specialized tasks, you have focused prompts.

### Situation A: Using a Specialized Prompt in the SAME Conversation

**If you're continuing the Study Brain conversation:**

Just ask Claude using that specialized prompt's approach:

```
In the Study Brain conversation, say:

"Use the [prompt name] approach to create flashcards for this study."

or

"Pretend you're using the visual-learning prompt: show me the 
visit workflow as a diagram."

or

"Help me prepare for monitoring using the visit-prep approach: 
here's what happened at the site [details]..."
```

Claude understands and applies that approach while keeping your study context.

### Situation B: Using a Specialized Prompt in a SEPARATE Conversation

Sometimes you want a fresh conversation for a focused task (e.g., comparing two documents side-by-side).

**Steps:**

1. **Open a NEW Claude conversation**
2. **Copy the specialized prompt** from the toolkit
3. **In the same message, include:**
   - The specialized prompt
   - Your study context (paste study-context-template.md)
   - The specific documents/information for this task
4. **Your specific request**
5. **Send to Claude**

**Advantage:** Clean, focused conversation without scrolling through previous discussion.

**Disadvantage:** Claude doesn't have context of previous questions, so use this for tasks that stand alone.

**When to use separate conversations:**
- Deep document analysis (comparing protocol versions, checking for inconsistencies)
- Focused quizzing (you want a fresh quiz, not building on previous answers)
- When the prompt is very different from your Study Brain conversation

**When NOT to use separate conversations:**
- Quick follow-up questions
- Building on previous understanding
- Anything that benefits from study context

---

## Step 4: Structure Your Information Correctly

Claude works best when information is clearly organized. Follow this pattern:

### Pattern A: Quick Question in Study Brain
```
I have a question about [specific topic].

What does "endpoint adjudication" mean in the context of 
the [Study Name] study?
```

**Claude uses context to give study-specific answer.**

### Pattern B: Asking for Specialized Output in Study Brain
```
Using the [prompt type] approach:

I need flashcards for the eligibility criteria. 
Generate 10 flashcard pairs.
```

**Claude applies that prompt's thinking style while keeping study context.**

### Pattern C: Using a Specialized Prompt Standalone
```
[PASTE ENTIRE PROMPT FROM TOOLKIT]

Here's my study context:
[PASTE STUDY-CONTEXT-TEMPLATE.MD]

Here's the information to analyze:
[PASTE PROTOCOL, DOCUMENT, OR SPECIFIC SECTION]

My question: [YOUR SPECIFIC REQUEST]
```

**Claude follows the prompt's detailed instructions with your specific information.**

### Pattern D: Comparing Documents
```
[PASTE SPECIALIZED PROMPT FOR COMPARISON]

Here's my study context:
[PASTE STUDY CONTEXT]

OLD DOCUMENT:
[PASTE VERSION 1]

NEW DOCUMENT:
[PASTE VERSION 2]

What changed, and what's the CRA impact?
```

**Claude compares systematically using the prompt's framework.**

---

## Step 5: Handle Large Documents

Claude has limits on how much text you can paste. For large protocols:

### Option 1: Section by Section
```
"I'm going to paste the protocol in sections. 
After each section, I'll ask you questions."

[PASTE SECTION 1]

Claude answers questions about Section 1, then you proceed to Section 2.
```

### Option 2: Key Sections Only
```
"Instead of the full protocol, here are the most important sections:

- Study Design (pages X-Y)
- Visit Schedule (page Z)
- Eligibility Criteria (pages A-B)
- Primary Endpoint (pages C-D)

[PASTE THESE SECTIONS]

Please understand the study based on these key sections."
```

### Option 3: Convert PDF to Text
If you have a PDF protocol, convert it to plain text using:
- Adobe Acrobat (export as text)
- Online converters (smallpdf.com, etc.)
- Copy-paste if the PDF isn't too long

Then paste the text into Claude.

### Option 4: Let Claude Manage It
```
"I'm going to paste a large protocol. 
Please acknowledge when you've read it, then ask me 
what you need clarification on."

[PASTE]

Claude: "I've read the protocol. What questions do you have?"
```

---

## Step 6: Iterative Refinement

Claude doesn't always get it perfect the first time. Refine:

### If Output Doesn't Match What You Need:

**Clarify the goal:**
```
"That's not quite what I needed. Let me clarify:

I need [specific outcome], not [what you gave me].

Can you revise to include [specific requirement]?"
```

**Adjust format:**
```
"Can you format this as a table instead of paragraphs?"

"Make this more concise (one page, not three)."

"Add more detail to the methodology section."
```

**Change perspective:**
```
"I'm the site coordinator, not the CRA. 
Revise this for what a site coordinator needs to know."
```

**Deepen explanation:**
```
"I still don't understand why this visit window is 14 days, not 7. 
Explain the reasoning based on the protocol."
```

---

## Step 7: Verify Important Information

This is critical. Claude can make mistakes. For any important conclusion:

### Ask Claude to Source It:

```
"You said [Claude's conclusion]. 

Show me the exact text from the protocol that supports this. 
What page or section?"
```

### If Claude Can't Source It:

```
"I can't find that in the protocol. 
Is this your inference, or is it stated explicitly?"
```

### If You Spot an Error:

```
"I think you misread that. The protocol actually says [correct text]. 
Can you re-analyze based on this correction?"
```

---

## Step 8: Know When to Stop Using Claude

Claude is amazing for:
- ✅ Understanding concepts
- ✅ Organizing information
- ✅ Creating flashcards
- ✅ Practice quizzes
- ✅ Identifying potential inconsistencies
- ✅ Brainstorming questions
- ✅ Explaining study design

Claude is NOT for:
- ❌ Making final regulatory/compliance decisions
- ❌ Medical judgments about patient eligibility
- ❌ Authoritative legal interpretation
- ❌ Critical safety decisions (always verify with qualified person)
- ❌ Any conclusion that affects patient safety without verification

**When in doubt:** Verify with the actual protocol, your Study Manager, Monitor, or Sponsor.

---

## Step 9: Use Commands for Efficiency

Once Claude has your Study Brain loaded, you can use short commands:

```
In the Study Brain conversation, you can say:

/teach me about [topic]
/diagram of [process]
/quiz me on [topic]
/flashcards for [topic]
/compare [concept 1] vs [concept 2]
/find risks in [section of protocol]
/find gaps in [section]
/find inconsistencies in [two things]
/visit prep for [upcoming visit]
/explain like I'm [specific audience]
/story about [concept]
/what's the impact if [scenario]
```

Claude will understand these abbreviations in the context of your Study Brain conversation.

---

## Step 10: Build Your Knowledge Over Time

### Week 1:
- Load Study Brain once
- Ask 5-10 understanding questions
- Don't start over; keep the conversation going

### Week 2:
- Use the same conversation
- Generate flashcards once, study them offline
- Ask deeper questions

### Week 3:
- Take practice quizzes in Study Brain
- Ask "why" and "what if" questions
- Claude helps you think critically

### Month 2+:
- Keep the conversation for context
- Use specialized prompts for analysis
- Test yourself regularly
- Claude adapts to your knowledge level

---

## Common Mistakes to Avoid

### ❌ Mistake 1: Starting a New Conversation for Each Question
**Why bad:** Claude loses context; answers are generic.

**Fix:** Keep one Study Brain conversation going throughout your involvement with the study.

### ❌ Mistake 2: Pasting Entire PDF Without Context
**Why bad:** Claude doesn't know what to focus on; answers can be disorganized.

**Fix:** Give Claude direction: "I'm a CRA learning this study. What are the most critical things for me to know?"

### ❌ Mistake 3: Accepting Claude's Answer Without Verification
**Why bad:** Claude can hallucinate study-specific facts.

**Fix:** Ask "Where in the protocol does it say that?" Always spot-check critical information.

### ❌ Mistake 4: Using the Toolkit Without Study Context
**Why bad:** You waste time providing the same background in each prompt.

**Fix:** Always include study-context-template.md with every prompt.

### ❌ Mistake 5: Treating Claude as the Authority
**Why bad:** Claude is a thinking tool, not an official source.

**Fix:** Use Claude to understand, then verify with official documents, Study Manager, Monitor, or Sponsor.

---

## Performance Tips

### For Faster, Better Answers:

1. **Be specific.** 
   - ❌ "Explain the study"
   - ✅ "Explain why patients must complete the washout period before screening"

2. **Provide context.**
   - ❌ "What's the visit schedule?"
   - ✅ "Why does the study have a visit at week 4 but not week 3, given the washout requirement?"

3. **Ask follow-up questions.**
   - ✅ "That makes sense. But what if a patient missed the week 2 visit—how does that affect visit 3?"

4. **Request specific formats.**
   - ✅ "Show this as a table, not paragraphs"
   - ✅ "Give me the 2-minute version"
   - ✅ "Format this as a flowchart"

5. **Build on previous answers.**
   - ✅ "Earlier you said X. Does that also apply to Y?"

### For Better Study Brain Setup:

1. **Paste complete protocol sections, not fragments.**
   - Claude understands context better with more text

2. **Include your study context document.**
   - Gives Claude essential reference information

3. **Tell Claude your role.**
   - "I'm a CRA new to clinical research"
   - "I'm an experienced CRA but new to this therapeutic area"
   - This helps Claude calibrate explanation level

---

## Example: Full Workflow

### Day 1: Setup (15 minutes)

```
Step 1: Fill out study-context-template.md
Step 2: Create new Claude conversation
Step 3: Paste Study Brain prompt + study context + protocol
Step 4: Ask: "Analyze this study and help me understand it"
Step 5: Close for now (keep conversation open)

Time: Done
```

### Day 2: First Learning (20 minutes)

```
Step 1: Open the Study Brain conversation (same one)
Step 2: Ask: "I don't understand the visit windows. 
        Why is it 7±3 days for visit 2 but 14±7 days for visit 3?"
Step 3: Claude explains with protocol references
Step 4: Ask follow-up: "What happens if a patient comes on day 5 
        instead of day 7 for visit 2?"
Step 5: Claude explains implications

Time: 20 minutes; learned important concept
```

### Day 3: Preparing for Monitoring Visit (25 minutes)

```
Step 1: Open Study Brain conversation
Step 2: Ask: "I have a monitoring visit next week. 
        What should I focus on? Previous visit had issues with 
        source data verification."
Step 3: Claude gives prioritized checklist
Step 4: In same conversation, ask: "Give me specific questions 
        I should ask about source data."
Step 5: Claude generates questions

Time: 25 minutes; visit preparation done
```

### Day 7: Quiz Yourself (30 minutes)

```
Step 1: Open Study Brain conversation (or new conversation if focus-quiz)
Step 2: Ask: "Quiz me on eligibility criteria. 
        Give me 10 questions, multiple choice."
Step 3: Work through quiz; Claude grades and explains
Step 4: Ask: "What areas should I study more?"
Step 5: Claude identifies weak areas

Time: 30 minutes; self-assessment complete
```

---

## When to Use Multiple Conversations

### Use ONE Study Brain Conversation for:
- Learning the study
- General questions
- Ongoing understanding
- Building knowledge
- Most follow-up questions

### Use SEPARATE Conversations for:
- Deep comparison of multiple complex documents
- Specialized analysis (risk review, root cause analysis)
- When you want a "fresh" conversation without scroll
- Focused quizzing sessions
- When output gets very long and hard to navigate

**Key:** Keep your main Study Brain conversation. Use secondary conversations as needed, but always reference back to Study Brain for study understanding.

---

## Troubleshooting

| Problem | Diagnosis | Solution |
|---------|-----------|----------|
| Claude gives wrong information about study | Missing or incomplete protocol context | Reload protocol + re-ask question with more context |
| Claude seems confused by my question | Unclear what I'm asking | Provide more specific context and clearer question |
| Claude won't stop talking | Too much detail | Ask for "concise version" or "one-paragraph summary" |
| Claude forgets previous answers | Using different conversation | Keep using same conversation throughout study |
| Output format not what I need | Didn't specify format | Ask "Please format as [table/list/diagram/etc.]" |
| Not confident in Claude's answer | Hallucination risk | Ask "Show me the exact text from the protocol supporting this" |

---

## Remember:

This toolkit works because **you provide full context to Claude once, then Claude maintains it throughout the conversation.**

The more complete your initial setup, the better every subsequent answer will be.

**Invest 15 minutes in setup.** Save hours of learning and preparation.
