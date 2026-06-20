# Ask My Build Log

A FAQ chatbot about my dev portfolio — projects, tech stack, education, internships. Matched live with TF-IDF + cosine similarity, not a fixed if/else lookup.

## Features
- 12 intents, each with several example phrasings (handles paraphrasing, not just exact matches)
- Preprocessing: lowercasing, punctuation stripping, tokenizing, stopword removal
- TF-IDF vectors built per example phrase; new questions matched by cosine similarity against all of them
- Shows the matched intent + confidence score under each reply (transparency into how the match was made)
- Falls back gracefully when nothing scores above threshold
- Single HTML file — no install, no build step, no API key, no backend

## Run it
Open `index.html` in any browser.

## Before you publish
The FAQ content (`INTENTS` array near the top of the script) is written generically from my own background — double check it still matches reality, and update the contact answer with a real link before sharing.

## Stack
HTML, CSS, vanilla JS. TF-IDF + cosine similarity implemented from scratch — no NLP library needed for a corpus this size.

---
CodeAlpha AI Internship — Task 2: Chatbot for FAQs
