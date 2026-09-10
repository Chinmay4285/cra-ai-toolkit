# Quizlet Generator: Create Flashcards for Study Facts

## PURPOSE
Automatically generate flashcards for study facts, terminology, procedures, eligibility criteria, and any study-specific information. These cards can be imported into Quizlet for offline study.

## WHEN TO USE
When you need to memorize study facts quickly. Great for: learning eligibility criteria, visit procedures, endpoints, terminology, safety information, key numbers.

## WHAT TO PROVIDE
- Your study context
- Your study protocol
- Specify what topic you want flashcards for

## EXPECTED OUTPUT
Flashcard pairs in Quizlet-compatible format (Term | Definition). Usually 15-30 cards per topic.

---

# QUIZLET GENERATOR PROMPT

```
COPY FROM HERE
========================================================================================

You are an expert at creating study-specific flashcards for CRA learning.

TASK: Generate flashcards for [topic] from the provided study protocol.

FLASHCARD GENERATION RULES:

1. CREATE MULTIPLE DIFFICULTY LEVELS
   
   LEVEL 1 - MEMORIZATION (Basic facts)
   - Simple definitions
   - Key terms
   - Important numbers
   - Acronyms
   
   LEVEL 2 - UNDERSTANDING (Concepts)
   - Why something is required
   - Relationships between concepts
   - "What if" scenarios
   - Application in study context
   
   LEVEL 3 - APPLICATION (Practical use)
   - Site scenarios
   - CRA decision-making
   - Problem-solving
   - Connecting multiple concepts

2. QUIZLET FORMAT (MUST USE THIS FORMAT)
   
   Front | Back
   ---|---
   What is a primary endpoint? | The main measurement used to determine if the study drug works
   [More cards...]

3. CONTENT REQUIREMENTS
   - Every card must be study-specific (not generic)
   - Every card should cite the protocol if possible
   - Cards should connect to each other
   - Balance breadth and depth
   - Include commonly confused concepts

4. QUALITY CHECKS
   ✓ Front side is clear, specific question or prompt
   ✓ Back side is complete but concise answer
   ✓ Every card is study-relevant
   ✓ No duplicate concepts
   ✓ Cards are scannable (not too long)

5. ORGANIZATION
   Group cards by difficulty:
   
   ## LEVEL 1: MEMORIZATION
   [Basic facts cards]
   
   ## LEVEL 2: UNDERSTANDING
   [Concept cards]
   
   ## LEVEL 3: APPLICATION
   [Scenario/decision cards]

6. COMPLETE LIST
   Finish with a summary:
   - Total cards generated
   - What to study first (Level 1)
   - What to tackle next (Levels 2-3)
   - Study strategy recommendation

HOW TO IMPORT TO QUIZLET:
1. Copy the cards from "LEVEL 1: MEMORIZATION" through "LEVEL 3: APPLICATION"
2. Go to quizlet.com
3. Create new study set
4. Paste into "Import" option
5. Select "Front | Back" format
6. Done—study immediately

========================================================================================
END PROMPT
```

---

## EXAMPLE TOPICS TO CREATE FLASHCARDS FOR

**Eligibility:**
- "Create flashcards for the inclusion criteria"
- "Create flashcards for the exclusion criteria"
- "Create flashcards for tricky eligibility scenarios"

**Visit Procedures:**
- "Create flashcards for the baseline visit"
- "Create flashcards for all study procedures"

**Endpoints:**
- "Create flashcards for the primary and secondary endpoints"

**Safety:**
- "Create flashcards for adverse event reporting and safety requirements"

**Terminology:**
- "Create flashcards for key study terms and acronyms"

**Numbers & Dates:**
- "Create flashcards for critical study numbers (windows, doses, timing, etc.)"

**Concepts:**
- "Create flashcards for understanding randomization and blinding"

---

## HOW TO MAXIMIZE FLASHCARD VALUE

1. **Study Level 1 first**
   - Get basic facts solid (30 minutes)
   - Use spaced repetition
   - Target 100% accuracy

2. **Move to Levels 2-3**
   - Deeper understanding
   - Problem-solving practice
   - Apply concepts

3. **Review before monitoring visits**
   - Quick 10-minute review
   - Level 1 only (just facts)

4. **Generate multiple flashcard sets**
   - One for each major topic
   - One for procedures
   - One for quick facts reference

5. **Use spaced repetition**
   - Quizlet has built-in spaced repetition
   - Study daily for retention
   - Review a week before important events

---

## INTEGRATING WITH YOUR STUDY BRAIN

In your Study Brain conversation, ask:
- `/flashcards for [topic]`

Claude will generate cards while maintaining your study context. Then copy-paste into Quizlet.

---

## STUDY STRATEGY RECOMMENDATION

**Week 1:**
- Generate flashcards for eligibility and procedures
- Study 30 min/day
- Target each card 3-5 times

**Week 2:**
- Generate flashcards for endpoints, safety, terminology
- Review Week 1 cards at maintenance level
- Study 30 min/day

**Week 3:**
- Generate flashcards for complex scenarios
- Study all previous cards at maintenance level
- Do final review before first monitoring visit

**Ongoing:**
- Quick 10-minute daily review
- Focus on weak areas (Quizlet identifies these)
- Add new cards as you encounter new information

---

## WHEN TO USE OTHER PROMPTS

- **For interactive quizzing:** Use `/04-Memorization/multiple-choice-quiz.md` or `scenario-quiz.md`
- **For adaptive testing:** Use `/08-Training/personal-cra-tutor.md`
- **For detailed explanations:** Use `/02-Understand/teach-me.md`
- **For visual learning:** Use `/03-Visual-Learning/teach-with-diagram.md`
