# Teach Me: Clear Concept Explanation

## PURPOSE
Get a clear, study-specific explanation of any clinical research concept, procedure, or requirement. This prompt transforms complex ideas into understandable explanations with practical CRA implications.

## WHEN TO USE
When you encounter a concept you don't fully understand and need it explained clearly with examples from your study.

## WHAT TO PROVIDE
- Your study context (from study-context-template.md)
- Your protocol (or relevant section)
- The specific concept, procedure, or requirement you don't understand

## EXPECTED OUTPUT
Clear explanation covering: what it is, why it matters, how it applies to your study, practical CRA implications, and how it connects to other requirements.

---

# TEACH ME PROMPT

```
COPY FROM HERE
========================================================================================

You are an expert clinical research educator explaining a concept to a CRA learning 
their study.

GOAL: Explain this concept clearly and completely, with specific application to 
the study materials provided.

STRUCTURE YOUR EXPLANATION:

1. SIMPLE DEFINITION
   What is this in the most basic terms? (2-3 sentences)

2. STUDY-SPECIFIC APPLICATION
   How does this apply in this specific study? 
   (Reference the protocol section)

3. WHY IT MATTERS
   Why is this requirement/procedure important for:
   - Patient safety
   - Study data quality
   - Regulatory compliance
   - Study success

4. PRACTICAL CRA IMPLICATIONS
   What does the CRA actually need to DO differently because of this?
   What should the CRA watch for?

5. CONNECTED CONCEPTS
   How does this relate to other study requirements?
   What else should the CRA understand about this topic?

6. COMMON MISUNDERSTANDINGS
   What do CRAs often get wrong about this?
   What should the CRA be careful NOT to assume?

7. QUESTIONS TO VERIFY
   What should the CRA ask the Study Manager or Monitor if unsure?

8. WOULD YOU LIKE TO KNOW MORE ABOUT...
   (Offer 2-3 related topics)

SOURCE GROUNDING:
- Every claim about the study should cite the protocol section
- Distinguish between stated facts and reasonable inferences
- If information isn't in the protocol, say so

TONE:
- Professional but conversational
- Respectful that the CRA has professional judgment
- Curious about the CRA's perspective

AFTER YOUR EXPLANATION:
Ask: "Does this make sense? What follow-up questions do you have?"

========================================================================================
END PROMPT
```

---

## USAGE EXAMPLES

**Example 1:**
"I don't understand the inclusion criteria. It says 'documented diagnosis.' What does documented mean?"

*Claude uses this prompt to explain what 'documented diagnosis' means in the study context, why it matters, how the CRA verifies it, and what mistakes to avoid.*

**Example 2:**
"Explain source data verification to me in the context of this study."

*Claude explains what SDV is, why this study requires it, what the CRA specifically must verify at each visit, how it affects timeline, and common problems.*

**Example 3:**
"Why do we have a washout period? I understand we're clearing the drug but why does that matter for this specific study?"

*Claude explains washout, why this study has one, the specific clinical reason for the timing, how it affects the visit schedule, and what happens if someone doesn't complete it.*

---

## Tips

1. **Be specific about what confuses you**
   - Not: "Explain endpoints"
   - But: "Explain the primary endpoint and why it's measured at week 12 instead of week 8"

2. **Ask follow-ups to deepen understanding**
   - After Claude's explanation: "What if a patient missed this assessment—how would that affect the endpoint?"
   - "How does this requirement connect to [other requirement]?"

3. **Request examples**
   - "Give me a specific example from a site"
   - "What's the most common mistake on this?"

4. **Compare to other studies**
   - "Is this typical or unusual?" (Claude can compare without your protocol being 'usual')

---

## When to Use Other Prompts Instead

- **If you want a visual:** Use `/Visual-Learning/teach-with-diagram.md`
- **If you want a story:** Use `/Understand/explain-like-a-story.md`
- **If you want to memorize:** Use `/Memorization/flashcards.md`
- **If you want comprehensive study understanding:** Use `/Study-Brain/study-expert.md`
