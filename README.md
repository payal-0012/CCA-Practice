# CCA-Practice

Self-study tools for the **Claude Certified Architect – Foundations (CCA-F)** exam. Three browser-based pages cover a bank of 175 practice questions. There's nothing to install, and each page is a single self-contained HTML file.

## Live links

| Tool | What it's for | Link |
|---|---|---|
| Practice exam | Timed 60-question mock test | https://payal-0012.github.io/CCA-Practice/ |
| Study coach | Learn all 175 questions with instant feedback | https://payal-0012.github.io/CCA-Practice/ccaf-study-coach.html |
| Flashcards & 20 rules | Memorize the key ideas quickly | https://payal-0012.github.io/CCA-Practice/ccaf-flashcards.html |

## The tools

### 1. Practice exam (`index.html`)
- 60 questions drawn at random from the 175 on every attempt
- 60-minute timer that auto-submits when time runs out
- Scored out of **1000 marks** (16.67 per question), with a percentage
- A question palette to jump around, plus flags for questions to revisit
- After submitting: a full answer key for every question, showing your answer, the correct answer, and whether you got it right, wrong, or skipped it
- **Retest** draws a fresh random set of 60
- Past attempt scores are saved in your browser

### 2. Study coach (`ccaf-study-coach.html`)
- Shows the correct answer immediately after each choice
- Missed questions come back a few cards later in the same session
- A question counts as **learned** after two correct answers in separate sessions
- Modes: Smart session (weakest first), Fix my mistakes, Marathon, sets of 25, and Quick read (all 175 with answers and keyword search)
- Option order is shuffled so you learn the idea, not the letter
- A colour-coded progress map of all 175 questions

### 3. Flashcards & 20 rules (`ccaf-flashcards.html`)
- **20 rules:** the core principles behind most of the questions, each linked to the questions it answers
- **Flashcards:** a short scenario on the front; on the back, the key idea, the exact exam answer, and the rule it belongs to
- **Speed round:** 10 scenarios, matching each to the right key idea
- The 20 exact duplicate questions are skipped by default, leaving 155 cards to learn
- Filter by topic: multi-agent research, tool design & MCP, extraction & Batch API, conversation & context, support agent, Claude Code & SDK, code review & CI

## Suggested study plan

1. Read the **20 rules** first to get the big picture.
2. Work through **Flashcards** until most cards are marked known.
3. Use the **Study coach** to practise with the full question wording.
4. Take the **Practice exam** under timed conditions, and retest until you score consistently.
5. For a final review, use **Quick read** in the study coach and the **Speed round**.

## How the questions work

All 175 questions are stored inside each HTML file as a JavaScript list called `BANK`. Each entry holds the question text, its options, and the correct answer letter. No server or database is used. The exam shuffles the full bank on each attempt and takes the first 60.

## Notes

- **Progress is stored in your browser** (localStorage), per device and per browser. Clearing browser data resets it.
- **Question 140** has only three options (A–C) in the source material.
- **Questions 51, 58 and 67** are identical, but the source gives 67 a different answer key (D) from 51 and 58 (C).
- The answer keys come from third-party practice material and may contain errors. Understanding *why* an answer is right matters more than memorizing the letter.

## Disclaimer

The questions come from third-party practice material and are kept here for personal study only. This project isn't affiliated with or endorsed by Anthropic.
