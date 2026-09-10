# Multiple-Choice Quiz: Interactive Study Testing

## PURPOSE
Test your knowledge with study-specific multiple-choice questions at various difficulty levels. Get immediate feedback and explanations.

## WHEN TO USE
When you want to test your knowledge before monitoring visits or assess understanding of specific topics.

## WHAT TO PROVIDE
- Your study context
- Your protocol
- Specific topic to be quizzed on (or "overall study")
- Desired difficulty level (basic, intermediate, advanced)

## EXPECTED OUTPUT
Series of multiple-choice questions with feedback after each answer.

---

# MULTIPLE-CHOICE QUIZ PROMPT

```
COPY FROM HERE
========================================================================================

You are creating a study-specific multiple-choice quiz to test CRA knowledge.

QUIZ GENERATION:

1. QUESTION DESIGN
   - Questions test understanding, not just memorization
   - Include some straightforward recall questions
   - Include applied reasoning questions
   - Include scenario-based questions
   - One clear correct answer; distractors are plausible wrong answers

2. DIFFICULTY LEVELS
   
   BASIC (Memorization):
   - Direct facts from protocol
   - Define terms
   - Identify basic requirements
   
   INTERMEDIATE (Understanding):
   - Explain reasons for requirements
   - Connect related concepts
   - Apply protocol to situations
   
   ADVANCED (Judgment):
   - Complex scenarios with multiple factors
   - Situations with ambiguity
   - Risk assessment and decision-making

3. QUIZ FORMAT

   For each question:
   
   QUESTION [#]: [Question stem - state what you're asking]
   
   A) [Distractor - plausible but wrong]
   B) [Distractor - plausible but wrong]
   C) [Correct answer with clear basis in protocol]
   D) [Distractor - plausible but wrong]

4. ANSWERING PROCESS
   
   CRA picks answer → You provide feedback:
   
   "Your answer: [Their answer]
   ✓ CORRECT (if right) or ✗ INCORRECT (if wrong)
   
   Explanation: [Why this answer is correct/incorrect]
   
   Protocol basis: [Where in protocol this is stated]
   
   Key concept: [The principle being tested]
   
   Related concept: [How this connects to other requirements]"

5. QUIZ PROGRESSION
   
   Generate 10-15 questions:
   - First 3-4: Basic difficulty (warm-up)
   - Middle 5-7: Intermediate difficulty (main assessment)
   - Last 3-4: Advanced difficulty (challenge questions)
   
   Progressively increase difficulty.

6. SCORING
   - Calculate percentage correct
   - Identify weak areas
   - Recommend follow-up study if score < 80%
   - Congratulate strong performance

========================================================================================
END PROMPT
```

---

## HOW TO USE THE QUIZ

**Before First Monitoring Visit:**
- Take a basic quiz on procedures
- Take intermediate quiz on eligibility and endpoints
- Target 100% before visiting

**Weekly Practice:**
- Pick a different topic each week
- Intermediate difficulty
- Target consistent 90%+

**Before Important Events:**
- Advanced quiz the day before monitoring
- Refresher quiz on critical facts

**Identifying Weak Areas:**
- Take comprehensive quiz on whole study
- Note which topics have low scores
- Use study prompts to review weak areas
- Re-quiz on weak topics weekly until strong

---

## QUIZ TYPES TO REQUEST

**Topic-Specific:**
- "Quiz me on eligibility criteria only"
- "Quiz me on visit procedures"
- "Quiz me on safety and adverse events"
- "Quiz me on endpoints and assessments"

**Difficulty-Based:**
- "Basic quiz - just facts"
- "Intermediate quiz - understanding"
- "Advanced quiz - judgment and scenarios"

**Format-Based:**
- "Quick 5-question quiz"
- "Comprehensive 20-question quiz"
- "Rapid-fire quiz with quick answers"

**Performance-Based:**
- "After I answer wrong, give me an easier version first"
- "Make it progressively harder as I get answers right"
- "Focus on my weak areas based on previous quizzes"

---

## SCORING GUIDE

**100%** → Excellent. You're ready.
**90-99%** → Very good. A few gaps to address.
**80-89%** → Good but needs review. Focus on wrong topics.
**70-79%** → Needs significant review. Use study prompts for weak areas.
**<70%** → More study needed. Use "teach-me" prompts before more quizzing.

---

## QUIZ STRATEGY

**Week 1:**
- Basic quizzes on major topics (eligibility, procedures, endpoints)
- Target 90%+

**Week 2:**
- Intermediate quizzes
- Mix of topics
- Adaptive difficulty

**Week 3:**
- Advanced/scenario quizzes
- Test judgment, not just facts

**Before Monitoring:**
- Quick 5-question refresh on critical facts
- Confidence booster

**Ongoing:**
- Monthly comprehensive quiz
- Weekly focused quizzes on weak areas
- Adapt based on performance

---

## INTEGRATING WITH YOUR STUDY BRAIN

In your Study Brain conversation, ask:
- `/quiz me on [topic]`
- `/quiz me - intermediate difficulty`
- `/quick 5-question quiz`

Claude will generate questions using your study context.

---

## WHEN TO USE OTHER PROMPTS

- **For flashcards:** Use `/04-Memorization/quizlet-generator.md`
- **For scenario practice:** Use `/08-Training/scenario-simulator.md`
- **For adaptive tutoring:** Use `/08-Training/personal-cra-tutor.md`
- **For explanation:** Use `/02-Understand/teach-me.md`
