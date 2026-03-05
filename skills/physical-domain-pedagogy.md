---
id: fcacc77e-a9bc-4863-877b-3f4614fbbf19
type: skill
title: Physical Domain Pedagogy
tags:
  - domain-pedagogy
  - physical
  - blocks
  - lyceum-core
references: []
created: '2026-03-03'
updated: '2026-03-03'
---
PHYSICAL SKILL BLOCKS (use these for cooking/drawing/yoga/etc. courses):

- recipe-step: A step-by-step recipe card. Shows one cooking step at a time with a large emoji, instruction text, timer badge, and pro tip. "Done — Next Step →" advances through the sequence. Use for any sequential hands-on process.
  { "type": "recipe-step", "recipeName": "Marinara Sauce", "steps": [{"action": "Heat olive oil", "instruction": "Set your pan on medium heat. Add 2 tablespoons of olive oil and wait for it to shimmer.", "emoji": "🫒", "timer": "30 sec", "tip": "The oil should shimmer but not smoke — that means it's too hot."}, {"action": "Sauté garlic", "instruction": "Add 3 minced garlic cloves. Stir constantly to prevent burning.", "emoji": "🧄", "timer": "1 min", "tip": "Garlic burns fast. The moment it's golden, move to the next step."}, {"action": "Add tomatoes", "instruction": "Pour in one can of crushed San Marzano tomatoes. Stir to combine.", "emoji": "🍅", "tip": "San Marzano tomatoes have less acidity and more sweetness than regular canned tomatoes."}, {"action": "Season and simmer", "instruction": "Add salt, pepper, and fresh basil. Let it simmer on low heat.", "emoji": "🌿", "timer": "15 min", "tip": "Don't stir too often. Let the sauce reduce and concentrate its flavors."}], "instruction": "Follow each step to make a classic marinara sauce.", "successMessage": "4 steps. 4 ingredients. You just cooked a restaurant-quality marinara." }

- ingredient-explorer: Visual grid of ingredients or tools. Tap each to learn its role.
  { "type": "ingredient-explorer", "items": [{"emoji": "🫒", "name": "Olive Oil", "role": "The base of every Italian dish"}, {"emoji": "🧄", "name": "Garlic", "role": "Builds the flavor foundation"}], "instruction": "Tap each ingredient to learn its role" }

- step-illustration: Visual card showing a technique step with detailed breakdown.
  { "type": "step-illustration", "title": "The Pinch Grip", "stepNumber": 1, "description": "Hold the knife between your thumb and index finger, gripping the blade just above the handle.", "emoji": "🔪", "details": ["Thumb on one side of the blade", "Index finger curled on the other side", "Remaining fingers wrap the handle", "This gives maximum control"], "tip": "The pinch grip feels weird at first but gives you much more precision than a hammer grip." }

- tool-identifier: Visual grid of tools. User taps the correct one.
  { "type": "tool-identifier", "question": "Which tool is used for zesting citrus?", "tools": [{"emoji": "🔪", "name": "Chef's Knife"}, {"emoji": "🫕", "name": "Microplane"}, {"emoji": "🥄", "name": "Ladle"}, {"emoji": "🍴", "name": "Tongs"}, {"emoji": "🥣", "name": "Whisk"}, {"emoji": "🫙", "name": "Peeler"}], "correctIndex": 1, "explanation": "A microplane grater is the best tool for zesting — it removes just the flavorful outer layer without the bitter pith." }

FIRST-TOUCH SEQUENCE FOR COOKING (Module 1, Blocks 1-3):
  Block 1: recipe-step — walk through 3-4 steps of a simple, iconic recipe for the cuisine
  Block 2: ingredient-explorer — show 4-5 key ingredients, learner taps to discover each
  Block 3: quick-quiz — "Which ingredient does [specific role]?" referencing what they just explored

FIRST-TOUCH SEQUENCE FOR DRAWING/ART (Module 1, Blocks 1-3):
  Block 1: step-illustration — show how to hold a pencil correctly (the physical foundation)
  Block 2: tool-identifier — identify basic drawing tools
  Block 3: quick-quiz — "Which grip gives you the most control for detail work?"

TIER AWARENESS: Adjust content complexity to match the module's position in the course.
  Beginner: simple recipes (3-4 steps), basic techniques, foundational ingredients.
  Intermediate: compound techniques, timing multiple components, flavor balancing.
  Advanced: advanced plating, recipe modification, improvisation from pantry ingredients.

IMPORTANT: Physical skill lessons should be at least 40% visual/interactive. The learner should feel like they're IN the kitchen / studio / gym, not reading about it. Use recipe-step for any sequential cooking process — it makes the learner walk through each step instead of reading a wall of text.
