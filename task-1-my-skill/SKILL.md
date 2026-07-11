[flashcard-maker-SKILL.md](https://github.com/user-attachments/files/29924787/flashcard-maker-SKILL.md)
---
name: flashcard-maker
description: Generates study flashcards (Question-Answer format) for any topic the user names. Use this skill whenever the user asks to "make flashcards," "create flashcards," "quiz me on," or wants to revise/study a topic using flashcards — even if they don't give notes, just a topic name. Also trigger if the user says things like "help me memorize X" or "test my knowledge of X."
---

# Flashcard Maker

A skill for turning any topic name into a ready-to-use set of study flashcards, without needing the user to supply notes.

## When to use this skill

Trigger this skill whenever the user:
- Says "make flashcards on/about/for [topic]"
- Says "quiz me on [topic]"
- Asks to revise, memorize, or study a topic and flashcards would help
- Gives just a topic name and asks for a study aid

Do NOT wait for the user to paste notes — this skill works from a topic name alone. If the user does paste notes/text instead, use that content as the source instead of generating from general knowledge.

## Instructions

1. **Identify the topic** from the user's request (e.g., "make flashcards on Newton's Laws" → topic = "Newton's Laws").

2. **Determine the number of flashcards**:
   - If the user specifies a number, use it.
   - Otherwise, default to **10 flashcards**.

3. **Generate the flashcards** using your own knowledge of the topic (or the user's pasted notes, if provided instead of a topic name). Follow these rules:
   - Cover the most important concepts, definitions, and facts for that topic — don't just pick random trivia.
   - Order the cards from **easier/foundational** concepts to **harder/more detailed** ones.
   - Each card must have exactly one clear **Question** and one concise **Answer** (1–2 sentences max for the answer — flashcards should be quick to review, not mini-essays).
   - Avoid yes/no questions; prefer questions that require recalling a fact, definition, or concept.
   - Do not repeat the same concept across multiple cards.

4. **Output format** — always use this exact structure:

```
📚 Flashcards: [Topic Name]

1. Q: [Question]
   A: [Answer]

2. Q: [Question]
   A: [Answer]

...

N. Q: [Question]
   A: [Answer]
```

5. **After presenting the cards**, add a short one-line note offering to:
   - Generate more flashcards on the same topic, or
   - Make flashcards on a related sub-topic, or
   - Quiz the user interactively (ask questions one at a time and check their answers).

## Example

**User input:** "make flashcards on photosynthesis"

**Output:**
```
📚 Flashcards: Photosynthesis

1. Q: What is photosynthesis?
   A: The process by which plants convert light energy into chemical energy (glucose) using sunlight, water, and carbon dioxide.

2. Q: What are the two main stages of photosynthesis?
   A: The light-dependent reactions and the light-independent reactions (Calvin cycle).

3. Q: Where in the plant cell does photosynthesis occur?
   A: In the chloroplasts.

...
```

## Notes

- Keep answers short and memorable — the goal is fast recall, not detailed explanation.
- If the topic is very broad (e.g., "World War 2"), it's fine to focus on the most commonly tested/important facts rather than trying to cover everything.
- If the user gives a vague or extremely niche topic, do your best with available knowledge and note if some details might be worth double-checking.
