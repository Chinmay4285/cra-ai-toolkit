# Study Memory Refresh: Reset Context in Long Conversations

## PURPOSE
If your Study Brain conversation becomes very long or Claude seems to have lost context, use this to refresh Claude's memory of your study without starting over.

## WHEN TO USE
- After 50+ messages in a Study Brain conversation (if Claude seems fuzzy)
- When returning to a conversation after days/weeks away
- When Claude contradicts something it said earlier about your study
- When you want to emphasize important study details

## WHAT TO PROVIDE
Simply paste this prompt into your Study Brain conversation, then ask Claude to refresh.

---

# REFRESH PROMPT

Paste this into your existing Study Brain conversation:

```
I want to make sure you're current on this study. Let me refresh your memory 
of the most critical details.

Here's what I want you to recap:

1. Study name, phase, and primary objective
2. Target patient population (key inclusion/exclusion)
3. Number of visits and key timepoints
4. Primary endpoint (how measured, when)
5. Treatment arm(s) and what we're testing
6. Top 3 most important CRA responsibilities
7. Top 3 most common challenges on this study
8. My experience level (how I've described myself)
9. Any specific issues or questions we've been discussing

After you recap these, I'll correct anything that's off, and we'll be back in sync.

Go ahead - recap what you know about this study.
```

Claude will recap, you correct any misunderstandings, and context is refreshed.

---

## If Claude Seems to Have Lost Critical Information

**Example:**

Claude states something about your study that contradicts what you know or what it said before.

You respond:

```
Actually, I need to correct that. The protocol says [correct information].

I'm noticing you might have lost some context. Let me do a quick refresh:

[Use the refresh prompt above]

Once we're aligned, my follow-up question is: [your actual question]
```

Claude will realign and your conversation continues smoothly.

---

## Note

This situation is rare if you keep one conversation going. But if you do encounter drift after many messages, this fixes it quickly without losing the conversation history.
