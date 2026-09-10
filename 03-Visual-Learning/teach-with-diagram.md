# Teach with Diagram: Visual Learning Approach

## PURPOSE
Get a visual representation of a clinical research concept, process, or requirement. Diagrams make complex relationships and sequences memorable.

## WHEN TO USE
When you learn better visually or when a concept involves steps, decisions, or relationships. Perfect for: visit workflows, study design, decision trees, timelines, relationships between requirements.

## WHAT TO PROVIDE
- Your study context
- Your protocol (relevant sections)
- What you want visualized

## EXPECTED OUTPUT
A clear diagram (ASCII, flowchart, or Mermaid format) that shows the concept visually, followed by a detailed explanation.

---

# TEACH WITH DIAGRAM PROMPT

```
COPY FROM HERE
========================================================================================

You are an expert at creating visuals that explain complex clinical research concepts.

TASK: Create a diagram that explains [concept/process/requirement] in the context of 
this study. Then explain the diagram.

DIAGRAM SELECTION:
Choose the BEST diagram type for what's being explained:
- Flowchart: For processes with decisions and steps
- Timeline: For sequences of events with timing
- Decision Tree: For criteria and decision logic
- Table/Matrix: For comparisons and relationships
- Concept Map: For how ideas relate
- Process Flow: For what happens when and why
- Swim Lane: For activities by role/timepoint

DIAGRAM REQUIREMENTS:
✓ Clear, easy to understand at a glance
✓ Labeled with study-specific terminology
✓ Shows the flow or relationship being explained
✓ Color/format distinguishes different elements if possible (ASCII or Mermaid)
✓ Includes critical decision points or timing information
✓ Is study-specific, not generic

EXPLANATION AFTER THE DIAGRAM:
1. "This diagram shows..." (overview)
2. "Key elements:" (label what's important)
3. "The flow/process/relationship:" (walk through step by step)
4. "Critical decision points:" (where judgment is required)
5. "CRA implications:" (what the CRA should watch for)
6. "Common misunderstandings:" (what people get wrong)

SOURCE GROUNDING:
- Base the diagram on the specific protocol details provided
- Cite protocol sections for important facts
- If explaining a process, reference where in the protocol it's described

DO NOT:
✗ Create overly complex diagrams
✗ Use generic flowchart shapes; use content-specific formatting
✗ Forget the "CRA implications" section
✗ Leave any part of the diagram unexplained

========================================================================================
END PROMPT
```

---

## WHAT CLAUDE CAN DIAGRAM

**Study Design:**
- "Diagram the study design [show arms, randomization, duration]"

**Patient Journey:**
- "Diagram what happens to a patient from screening through follow-up"

**Visit Workflows:**
- "Diagram what procedures happen at the baseline visit and in what order"

**Decision Points:**
- "Diagram how to determine if a patient meets inclusion criteria"

**Timelines:**
- "Diagram the study timeline showing all visits and assessments"

**Relationships:**
- "Diagram how the eligibility criteria, inclusion population, and endpoints relate"

**Safety Processes:**
- "Diagram the safety monitoring process from adverse event report to documentation"

**Data Flow:**
- "Diagram how study data flows from site to EDC to database"

---

## TIPS FOR BEST RESULTS

1. **Describe what you want to see**
   - Better: "I need to understand the patient flow during the screening phase"
   - Simpler: "Show me screening as a flowchart"

2. **Ask for specific format if you have a preference**
   - "I learn better with timelines—show the entire study as a timeline"
   - "Use a decision tree to show eligibility logic"

3. **Request explanation after**
   - "After showing the diagram, walk me through it step by step"
   - "Explain what could go wrong at each step"

4. **Ask CRA-specific follow-up**
   - "What should I watch for in this process?"
   - "What's the most common mistake at this step?"

---

## INTEGRATING WITH STUDY BRAIN

In your Study Brain conversation, ask:
- `/diagram of [concept]`

Claude will create a visual explanation while maintaining your study context.

---

## When to Use Other Prompts Instead

- **If you want a written explanation:** Use `teach-me.md`
- **If you want a story:** Use `explain-like-a-story.md`
- **If you want to memorize facts:** Use `/04-Memorization/flashcards.md`
- **If you want to test yourself:** Use `/04-Memorization/scenario-quiz.md`
