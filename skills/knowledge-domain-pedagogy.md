---
id: 28ec060a-7035-44ea-bb21-00f662939302
type: skill
title: Knowledge Domain Pedagogy
tags:
  - domain-pedagogy
  - knowledge
  - blocks
  - lyceum-core
references: []
created: '2026-03-03'
updated: '2026-03-03'
---
KNOWLEDGE-SPECIFIC BLOCKS (use these for business/history/science/philosophy courses):

- claim-judge: Present a provocative statement. Learner agrees or disagrees. Then reveal the nuanced truth. Gets the learner THINKING from block 1.
  { "type": "claim-judge", "claim": "The Stoics believed you should suppress all emotions", "options": ["Agree", "Disagree"], "correctIndex": 1, "explanation": "Common misconception. Stoicism is about recognizing which emotions serve you, not eliminating them.", "instruction": "What do you think?" }

- concept-diagram: Interactive concept map. Center node is visible, outer nodes appear one by one as the learner taps. Learner discovers the framework instead of passively seeing it all at once.
  { "type": "concept-diagram", "title": "Porter's Five Forces", "centerLabel": "Competition", "nodes": [{"label": "New Entrants", "description": "Threat of new competitors entering the market."}, {"label": "Suppliers", "description": "Bargaining power of suppliers who provide inputs."}, {"label": "Buyers", "description": "Bargaining power of customers."}, {"label": "Substitutes", "description": "Threat of alternative products or services."}, {"label": "Rivalry", "description": "Intensity of competition among existing firms."}], "tip": "Use this framework to analyze any industry's competitive landscape." }

- timeline-picker: Visual timeline of events. User taps the correct one.
  { "type": "timeline-picker", "question": "When was the first iPhone released?", "events": [{"year": "2005", "label": "YouTube launches"}, {"year": "2007", "label": "iPhone is released"}, {"year": "2008", "label": "Global financial crisis"}, {"year": "2010", "label": "Instagram launches"}], "correctIndex": 1, "explanation": "Steve Jobs announced the iPhone on January 9, 2007, revolutionizing the smartphone industry." }

FIRST-TOUCH SEQUENCE FOR KNOWLEDGE DOMAINS (Module 1, Blocks 1-3):
  Block 1: claim-judge — provocative statement that challenges a common misconception about the topic
  Block 2: concept-diagram — the central framework of the domain, revealed interactively
  Block 3: quick-quiz — test the insight from the claim-judge (did they internalize the correct answer?)

IMPORTANT: Knowledge lessons should make abstract ideas TANGIBLE. Use claim-judge to provoke thought before teaching. Use concept-diagrams to make frameworks interactive. Even for "knowledge" domains, the learner should be DOING (judging claims, exploring diagrams, sorting timelines) not just READING.
