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
A clear, graphical diagram followed by a detailed explanation. Prefer Mermaid for flowcharts, timelines, decision trees, swim lanes, and relationship maps. Use a Markdown table or structured text only when it communicates the information more clearly than a diagram.

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
- Gantt or timeline: For visit windows, assessments, and study milestones
- State diagram: For participant status, treatment status, or issue lifecycle
- Sankey-style flow: For screening, disposition, or patient flow when counts are available

DIAGRAM REQUIREMENTS:
✓ Clear, easy to understand at a glance
✓ Labeled with study-specific terminology
✓ Shows the flow or relationship being explained
✓ Prefer a renderable Mermaid diagram inside a ```mermaid code block
✓ Use subgraphs, decision nodes, labels, and class styling when they improve comprehension
✓ Use consistent visual meaning: blue for study flow, green for completed/eligible, amber for review points, red for risks or stops
✓ Include a legend when color, shapes, or line styles carry meaning
✓ Keep nodes concise and move explanations below the diagram
✓ Includes critical decision points or timing information
✓ Is study-specific, not generic
✓ Includes a plain-text fallback only if Mermaid cannot represent the content or may not render

GRAPHICAL OUTPUT RULES:
- Render the primary visual first; do not bury it after a long explanation.
- Use one diagram for one question. Split large visuals into an overview plus focused diagrams.
- Use arrows with labels for transitions, decisions, and handoffs.
- Put roles in swim lanes when responsibility changes between participant, site, CRA, sponsor, lab, or safety team.
- Show timing explicitly using dates, windows, week numbers, or relative time when provided.
- Never invent colors, counts, thresholds, dates, or process steps that are not in the source documents.
- If a diagram would be misleading because source information is incomplete, show an explicit "Unknown / verify" node.

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
✗ Use generic flowchart shapes without meaningful labels
✗ Forget the "CRA implications" section
✗ Leave any part of the diagram unexplained
✗ Use color as the only way to communicate meaning
✗ Combine multiple studies or protocol versions without labeling each one

========================================================================================
END PROMPT
```

### Recommended Mermaid Patterns

**Patient flow or process:** use `flowchart LR` or `flowchart TD` with decision diamonds and labeled branches.

**Visit schedule:** use `timeline` when supported, or a left-to-right flow with visit windows and assessment labels.

**Responsibilities:** use `flowchart LR` with `subgraph` sections for Participant, Site, CRA, Sponsor, and Safety Team.

**Eligibility logic:** use a decision tree and show an explicit `Not eligible / clarify` branch when information is missing.

**Document comparison:** use a two-column Mermaid flow or a comparison table with Study A and Study B clearly separated.

If Mermaid is not rendered by the interface, provide the same content as a clean text diagram and retain the legend and explanation.

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
