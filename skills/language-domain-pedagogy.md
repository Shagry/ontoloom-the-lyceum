---
id: bb758380-904c-4f9c-9724-58a9239939c1
type: skill
title: Language Domain Pedagogy
tags:
  - domain-pedagogy
  - language
  - blocks
  - lyceum-core
references: []
created: '2026-03-03'
updated: '2026-03-03'
---
LANGUAGE-SPECIFIC BLOCKS (use these for language courses):

- listen-and-tap: Audio plays a word. Learner taps the correct written option.
  { "type": "listen-and-tap", "audioText": "Bonjour", "language": "french", "options": ["Bonjour", "Bonsoir", "Merci", "Au revoir"], "correctIndex": 0, "instruction": "Listen and tap what you hear", "translation": "Hello" }

- word-card: Large visual card showing a word with pronunciation (auto-plays audio), translation, and example.
  { "type": "word-card", "word": "Bonjour", "phonetic": "/bɔ̃.ʒuʁ/", "translation": "Hello / Good morning", "emoji": "👋", "example": "Bonjour, comment allez-vous?", "tip": "Used as a formal greeting, any time of day until evening." }

- sentence-builder: User taps words in the correct order to build a sentence.
  { "type": "sentence-builder", "instruction": "Build the sentence: 'I would like a coffee'", "words": ["café", "voudrais", "un", "Je"], "correctOrder": ["Je", "voudrais", "un", "café"], "translation": "I would like a coffee" }

- conversation-fill: A dialogue scene with blanks in the learner's lines.
  { "type": "conversation-fill", "context": "At a café", "lines": [{"speaker": "Waiter", "text": "Bonjour, qu'est-ce que vous désirez?"}, {"speaker": "You", "text": "Je voudrais {{0}}, s'il vous plaît."}], "blanks": [{"options": ["un café", "un chat", "un livre"], "correctIndex": 0}], "explanation": "Un café means 'a coffee' — the correct response when ordering." }

- picture-match: Visual quiz with emoji representations.
  { "type": "picture-match", "question": "Which picture matches 'le chat'?", "options": [{"emoji": "🐱", "label": "Cat"}, {"emoji": "🐕", "label": "Dog"}, {"emoji": "🐦", "label": "Bird"}, {"emoji": "🐟", "label": "Fish"}], "correctIndex": 0, "explanation": "Le chat means 'the cat' in French." }

FIRST-TOUCH SEQUENCE FOR LANGUAGE (Module 1, Blocks 1-3):
  Block 1: listen-and-tap — hear the most common greeting, tap it (e.g., "Bonjour" for French)
  Block 2: word-card — see the greeting with pronunciation, translation, and example
  Block 3: picture-match — match 2-3 simple nouns to images (visual vocabulary)

IMPORTANT: Language lessons should be at least 50% interactive. The learner should HEAR the language spoken from the very first block. Every new vocabulary word must have audio pronunciation.
