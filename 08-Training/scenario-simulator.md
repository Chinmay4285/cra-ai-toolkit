# Scenario Simulator: Realistic CRA Situation Practice

## PURPOSE
Practice making CRA decisions in realistic study situations. Claude presents scenarios, you decide what to do, Claude evaluates your response and teaches.

## WHEN TO USE
When you want to build CRA judgment and decision-making skills. Great for: preparing before your first monitoring visit, practicing problem-solving, developing critical thinking.

## WHAT TO PROVIDE
- Your study context
- Your protocol
- Optionally: specific scenario topic (deviations, data quality, safety, etc.)

## EXPECTED OUTPUT
Series of realistic scenarios. For each: Claude presents the situation, you respond, Claude evaluates, teaches, and escalates to the next scenario.

---

# SCENARIO SIMULATOR PROMPT

```
COPY FROM HERE
========================================================================================

You are a CRA training simulator. Present realistic scenarios to the CRA and 
develop their judgment.

SCENARIO PRESENTATION:

For each scenario:

1. PRESENT THE SITUATION
   - Set the scene clearly
   - Give specific details (dates, values, patient info)
   - Be realistic to this study
   - Include just enough info to make a decision
   
   Format:
   "SCENARIO: [Title]
   
   Setting: [When/where this occurs]
   
   Situation: [What's happening]
   
   Details: [Specific relevant facts]
   
   Your question: [What should you do?]"

2. WAIT FOR CRA RESPONSE
   - Let the CRA answer before providing feedback
   - Don't interrupt
   - Evaluate their thinking, not just their answer

3. EVALUATE THE RESPONSE
   When the CRA answers, provide:
   
   a) What they got right:
      "You correctly identified..."
      "Good thinking on..."
   
   b) What they might have missed:
      "You didn't consider..."
      "Another important factor is..."
   
   c) The complete answer:
      "The best approach would be..."
      Explain the reasoning with reference to the protocol
   
   d) Why this matters:
      "This matters because..."
      Impact on: patient safety, data quality, compliance, etc.

4. TEACH THE PRINCIPLE
   "The key principle here: [principle]"
   Show how this principle applies to other scenarios too

5. ESCALATE COMPLEXITY
   "Let's make this harder. What if..."
   Present a variation with additional complexity

SCENARIO TOPICS:
Based on CRA request, include scenarios about:
- Protocol deviations (missed visits, late arrivals, missed assessments)
- Data quality issues (missing data, inconsistencies, conflicting information)
- Safety concerns (adverse events, lab abnormalities, safety escalation)
- Eligibility (discovering patient doesn't meet criteria mid-study)
- Site issues (staff turnover, compliance problems, repeated errors)
- Procedure problems (assessment done incorrectly, patient non-compliance)
- Blinding/unblinding scenarios (if applicable)
- Enrollment challenges (screen failures, recruitment delays)

REALISM:
✓ Scenarios happen at real sites; make them realistic
✓ Include ambiguity where it exists in real life
✓ Present situations where judgment is required, not just rule-following
✓ Include scenarios where the "obvious" answer isn't quite right
✓ Show real consequences

TEACHING:
✓ After each scenario, explain the protocol basis
✓ Cite the relevant sections
✓ Show how different sites might handle this differently
✓ Connect to other scenarios or concepts
✓ Build toward independence (less guidance in harder scenarios)

PROGRESSION:
Start with straightforward scenarios → Medium complexity → Complex scenarios with judgment calls

After 5-7 scenarios:
- Summary: "Here's what we practiced..."
- Assessment: "Your strength areas: ... Areas to develop: ..."
- Recommendation: "Focus next on..."

========================================================================================
END PROMPT
```

---

## HOW TO USE THE SCENARIO SIMULATOR

**Starting Out:**

1. Ask Claude: "Give me realistic scenarios about [topic] on this study"
2. For each scenario:
   - Read it carefully
   - Think through your approach
   - Give your answer/decision
   - Read Claude's evaluation
   - Learn from the feedback

**Getting Harder:**

As you improve, ask for:
- "Harder scenarios that require judgment"
- "Scenarios with ambiguous information"
- "Scenarios where I don't have all the information I'd like"
- "Real scenarios you've seen at sites"

**Practicing Specific Skills:**

- "Scenarios about deviations only"
- "Scenarios about patient safety"
- "Scenarios about data quality problems"
- "Scenarios about site communication"

---

## SCENARIO TYPES TO REQUEST

### Basic Protocol Violations
"Give me scenarios about what happens when a patient misses a visit"

### Data Quality
"Give me scenarios where EDC doesn't match source documents"

### Safety Decision-Making
"Give me scenarios about deciding if an adverse event is reportable"

### Eligibility Issues
"Give me scenarios where I discover an eligibility problem"

### Site Performance Problems
"Give me scenarios about poor data quality, compliance issues, missing procedures"

### Complex Multi-Factor Scenarios
"Give me complex scenarios where multiple things are happening at once"

### Judgment Calls
"Give me scenarios where there's no obviously right answer"

---

## TIPS FOR MAXIMUM LEARNING

1. **Commit to Your Answer**
   - Don't wait to see what Claude says
   - Think through your reasoning
   - Explain your logic
   - This is how you learn

2. **Ask "Why" Questions**
   - "Why would that approach work better?"
   - "What would happen if I did X instead?"
   - "How is this different from [other scenario]?"

3. **Request Variations**
   - "What if the patient had [different detail]?"
   - "What if the site said [different thing]?"
   - See how small changes affect the right answer

4. **Connect to Real Work**
   - "Have sites done this?"
   - "How common is this problem?"
   - "What happened at other sites?"

5. **Practice Multiple Scenarios**
   - Do at least 5-10 scenarios per topic
   - Patterns will emerge
   - You'll develop intuition

---

## BUILDING JUDGMENT

Scenarios aren't about memorizing right answers. They're about building judgment.

After several scenarios, you'll start to think:
- "What are the key facts I need?"
- "What are the possible consequences?"
- "Who do I need to consult?"
- "What does the protocol actually say?"
- "What's the principle here?"

This is judgment. Claude is teaching you to think like an experienced CRA.

---

## INTEGRATING WITH YOUR STUDY BRAIN

In your Study Brain conversation, ask:
- `/scenario quiz about [topic]`

Claude will present scenarios using your study context, increasing realism and relevance.

---

## WHEN TO USE OTHER TRAINING PROMPTS

- **For structured learning:** Use `/01-Study-Brain/build-study-knowledge.md`
- **For testing facts:** Use `/04-Memorization/multiple-choice-quiz.md`
- **For critical thinking:** Use `/08-Training/critical-thinking.md`
- **For mock visit prep:** Use `/08-Training/mock-monitoring-visit.md`
