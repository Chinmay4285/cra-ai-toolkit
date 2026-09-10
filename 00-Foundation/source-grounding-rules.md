# Source Grounding Rules: Preventing Hallucinations

**Purpose:** This guide ensures Claude never invents study-specific information. All facts must come from provided study documents.

---

## The Core Rule

**Claude must NEVER state study-specific facts without a source in the provided documents.**

This is non-negotiable. It protects you from making decisions based on hallucinated information.

---

## What CAN Claude State Without Documentation?

✅ **General clinical research knowledge**
- "Phase III trials typically enroll larger patient populations than Phase II"
- "Double-blind means neither patient nor investigator knows treatment assignment"
- "Informed consent must be obtained before any study procedures"

✅ **Logical inferences from documented facts**
- If the protocol says "14-day washout" and you ask why, Claude can infer: "Long washout periods typically indicate the drug has a longer half-life or lingering effects"
- If the protocol requires weekly visits, Claude can infer: "This suggests the study is monitoring for frequent changes"

✅ **Clarifications and explanations**
- "This term usually means..."
- "In clinical research, this is typically..."
- "This is commonly interpreted as..."

---

## What CANNOT Claude State Without Documentation?

❌ **Study-specific facts, requirements, numbers, or procedures without documentation**

**Examples of hallucinations to prevent:**

**Scenario 1:**
❌ "Your protocol requires baseline labs at every screening visit" 
(Without the protocol explicitly stating this)

✅ "According to the protocol (page 5, Section 2.1), baseline labs must be completed at screening"

---

**Scenario 2:**
❌ "The study has 6 visits"
(If this isn't explicitly stated)

✅ "Based on the visit schedule you've provided, I count 6 visits: screening, baseline, weeks 2, 4, 8, and 12"

---

**Scenario 3:**
❌ "Patients are randomized 1:1 to treatment groups"
(Without documentation)

✅ "The protocol states randomization is 1:1 (page 8, Section 3.2)"

---

**Scenario 4:**
❌ "The primary endpoint is measured at 12 weeks"
(If only secondary endpoint section was provided)

✅ "I see the secondary endpoint is measured at 12 weeks, but I don't see the primary endpoint definition in the materials you provided. Can you share that section?"

---

## Hallucination Red Flags: What Claude Should NEVER Do

### ❌ Red Flag 1: State Specifics Without Citation
**Wrong:** "Your study requires blood work every other week"
**Right:** "The protocol (page 4) specifies blood work at these timepoints: [list]"

### ❌ Red Flag 2: Invent Details to Make an Answer Seem Complete
**Wrong:** "Your CRA responsibilities include monitoring adverse events, checking informed consent, and verifying source data on 100% of patient visits"
(Made up the 100% if not stated)

**Right:** "Based on what you've provided, CRA responsibilities include monitoring adverse events and checking informed consent. The protocol doesn't specify what percentage of visits require source data verification—you may need to check the monitoring plan for this detail"

### ❌ Red Flag 3: Use Vague Language That Masks Uncertainty
**Wrong:** "The study appears to require weekly visits"
(Unclear if this is from the protocol or an inference)

**Right:** "The protocol specifies weekly visits in the treatment phase (Section 3.1). In the follow-up phase, visits are monthly (Section 3.2)"

### ❌ Red Flag 4: Make Regulatory or Compliance Claims Without Authority
**Wrong:** "FDA regulations require that all serious adverse events be reported within 24 hours"
(This is generic; the study protocol takes precedence)

**Right:** "The protocol (page 10) requires serious adverse events to be reported to the Sponsor within 24 hours. Your regulatory team should confirm this meets FDA requirements"

### ❌ Red Flag 5: Assume When Uncertain
**Wrong:** "This patient doesn't meet inclusion criteria because they're over the age limit"
(Without seeing the actual age from source documents)

**Right:** "The protocol specifies the age range as [X to Y]. Based on the patient's documented birth date, verify whether they fall within this range"

---

## How to Handle Uncertainty: The Right Way

### When Information Is Missing:

**Step 1: State what you know**
"Based on the materials provided, the study has [X] visits"

**Step 2: State what you don't have**
"I don't have the protocol section that specifies [Y detail]"

**Step 3: Ask for clarification**
"Can you provide the section on [topic]?"

**Step 4: Suggest verification**
"To verify this, check [specific protocol section]"

### When Protocol Is Ambiguous:

**Step 1: Note the ambiguity**
"The protocol uses the term [X], which could mean either [A] or [B]"

**Step 2: Show both interpretations**
"Interpretation A would mean [consequence]"
"Interpretation B would mean [consequence]"

**Step 3: Suggest how to clarify**
"I recommend asking the Study Manager which interpretation applies"

### When You're Making an Inference:

**Step 1: Label it clearly**
"This is my inference, not a stated protocol requirement:"

**Step 2: Show your reasoning**
"Since [stated fact], this suggests [inference]"

**Step 3: Acknowledge uncertainty**
"But this isn't explicitly confirmed in the protocol"

**Step 4: Recommend verification**
"Verify this interpretation with [appropriate person]"

---

## The Verification Checklist

Before stating any study-specific fact, Claude should ask:

- [ ] Is this explicitly stated in the provided protocol?
- [ ] Can I point to the exact page/section?
- [ ] Is this a reasonable inference from stated facts?
- [ ] Or am I assuming/inferring beyond what's documented?
- [ ] Should I label this as an inference vs. fact?
- [ ] If I'm wrong about this, what could go wrong?
- [ ] Should I encourage verification with the Study Manager or Monitor?

---

## How YOU Can Catch Hallucinations

### Ask Claude These Questions:

**1. "Where does the protocol say that?"**
Claude should be able to cite it. If Claude can't, it was hallucinated.

**2. "Show me the exact text supporting that conclusion"**
If Claude shows text that doesn't actually support the conclusion, hallucination detected.

**3. "Is that stated in the protocol, or is that your inference?"**
Force Claude to be explicit. If Claude hedges, it was uncertain.

**4. "What would happen if I followed your advice and it turned out you were wrong?"**
For critical information, verify before acting.

### When You Spot a Hallucination:

✅ **Do this:**
"I just checked the protocol, and it actually says [X]. Can you re-analyze based on this correction?"

✅ **Claude should:**
Acknowledge the correction, thank you for catching it, and re-analyze correctly.

❌ **Don't do this:**
Just accept the wrong information and move forward.

---

## Study-Specific Information: Always Verify

### High-Risk Areas for Hallucination:

These topics are commonly hallucinated because they sound plausible but can vary wildly by study:

- ⚠️ Visit windows (±days can vary 3-14 days)
- ⚠️ Eligibility ages (might be 21-65, 18+, 40-75, etc.)
- ⚠️ Endpoint definitions (how exactly is something measured?)
- ⚠️ Safety parameters (what labs? what values?)
- ⚠️ Randomization ratios (1:1, 2:1, 1:2:1?)
- ⚠️ Blinding status (which parties are blinded?)
- ⚠️ Concomitant medication restrictions
- ⚠️ Protocol deviations (what counts as one?)
- ⚠️ CRA responsibilities (varies significantly by study)
- ⚠️ Monitoring procedures (on-site vs. central varies)

**For these topics especially: Always get the source citation before acting.**

---

## Source Priority System

When analyzing a CRA's specific study, use this priority:

**Tier 1 - HIGHEST PRIORITY:**
- Current approved protocol
- Current approved ICF
- Current monitoring plan
- Current safety reports

**Tier 2 - HIGH PRIORITY:**
- Study-specific SOPs
- Investigator's Brochure
- Statistical Analysis Plan
- Protocol amendments

**Tier 3 - MEDIUM PRIORITY:**
- Study manuals
- Investigator instructions
- Site coordinator training materials

**Tier 4 - REFERENCE ONLY:**
- Generic clinical research knowledge
- Regulatory standards
- "Typical" study practices
- Industry guidelines

**Never override Tier 1 with Tier 4.**

Example:
❌ "Typically, 14-day washouts are standard..." (Wrong if YOUR protocol says 7 days)
✅ "Your protocol specifies 7 days, which is shorter than typical" (Correct)

---

## Critical Phrases That Indicate Hallucination Risk

Claude should use different language for facts vs. inferences:

**Safe language (for facts from protocol):**
- "The protocol states..."
- "According to [document], Section [X]..."
- "The protocol specifies..."
- "As documented in the [protocol/ICF]..."

**Safe language (for inferences):**
- "This suggests..."
- "This implies..."
- "This inference is based on..."
- "I'm inferring that... based on..."
- "This is my interpretation of..."

**Risky language (hallucination warning signs):**
- ❌ "Typically..." (when discussing study-specific requirements)
- ❌ "Usually..." (when discussing YOUR study)
- ❌ "Likely..." (for study-specific facts)
- ❌ "Probably..." (for requirements that need certainty)
- ❌ "It's common for..." (when discussing YOUR study)
- ❌ "[Name], the [role], probably..." (inventing people)

---

## Template for Safe Statements

Use this structure to avoid hallucination:

**FACT + CITATION:**
```
[Fact from protocol] 
[Source: "Protocol, Section X, page Y" or "You stated that..."]
```

**INFERENCE:**
```
Based on [stated fact], this suggests [inference].
Verify this interpretation with [appropriate person].
```

**ASSUMPTION:**
```
I'm assuming [assumption] to proceed.
If this isn't correct, let me know.
```

**UNKNOWN:**
```
The protocol doesn't specify [X].
This should be clarified with [appropriate person].
```

**Example:**

✅ **Safe:**
"The protocol (Section 3.1, page 5) specifies a 14-day washout before screening. This suggests the investigational product has a longer half-life, requiring more time to clear from the system. Verify this interpretation with the Study Manager. The exact clinical reason should be in the Investigator's Brochure."

❌ **Hallucination-prone:**
"The washout is 14 days because the drug has a long half-life and remains in the system. Patients need this time to clear the drug before screening."

---

## When Claude Isn't Sure: What to Do

**If Claude says: "I'm not certain about this"**

✅ **Good.** This means Claude is being appropriately cautious. Ask Claude to:
1. State what IS certain
2. Identify what ISN'T certain
3. Suggest how to find the answer

**If Claude states something as fact and you're not sure it's right:**

✅ **Verify it.** Ask Claude: "Show me the protocol text that supports this"

✅ **Cross-check.** Look it up in your protocol yourself

✅ **Correct it.** If wrong, tell Claude: "Actually, the protocol says [X]. Re-analyze based on this"

---

## A Note on AI Limitations

Claude is an AI language model trained on large amounts of text. It can:
- ✅ Recognize patterns
- ✅ Make logical inferences
- ✅ Explain complex concepts
- ✅ Organize information
- ✅ Generate questions

Claude cannot:
- ❌ Access documents you haven't provided
- ❌ Remember information from previous (unrelated) conversations
- ❌ Know your specific study documents unless you provide them
- ❌ Distinguish perfectly between fact and hallucination when uncertain
- ❌ Replace human clinical research judgment

**Your responsibility:** Be the verification layer. When Claude's answer matters, verify it.

---

## Summary: The CRA's Anti-Hallucination Checklist

Before acting on Claude's advice about your study:

- [ ] Did Claude cite a protocol section (page/section number)?
- [ ] Does that section actually say what Claude claims?
- [ ] If Claude made an inference, did it label it as such?
- [ ] Did Claude acknowledge what it doesn't know?
- [ ] Does the answer match my understanding of the study?
- [ ] If I'm uncertain, should I verify with the Study Manager/Monitor?
- [ ] Is this a high-risk area (visit windows, endpoints, safety, eligibility)?
- [ ] If Claude is wrong, what's the potential impact?

**When in doubt: Always verify critical information with your Study Manager, Monitor, or the actual protocol document.**

Claude is a thinking tool. You are the clinical research professional with judgment and responsibility.
