---
id: 29b00ac0-0d8e-4934-ba3c-59bc7abd006e
type: skill
title: Math Domain Pedagogy
tags:
  - domain-pedagogy
  - math
  - blocks
  - lyceum-core
references: []
created: '2026-03-03'
updated: '2026-03-03'
---
MATH-SPECIFIC BLOCKS (use these for math/arithmetic/algebra courses):

- equation-builder: Tap-to-place equation builder. Shows empty slots and a target result. Learner taps available number/operator pieces to fill slots and build the equation. Tap a filled slot to remove the piece.
  { "type": "equation-builder", "targetResult": "12", "slotCount": 3, "correctSlots": ["3", "×", "4"], "availablePieces": ["3", "×", "4", "+", "7", "15", "6"], "instruction": "Build the equation. What gives you 12?", "successExplanation": "3 × 4 = 12. Multiplication is repeated addition — 3 groups of 4.", "failExplanation": "That doesn't equal 12. Try a different combination." }

- spreadsheet-formula: Use for applied math — showing how math works in real-world contexts like budgets and data.
  { "type": "spreadsheet-formula", "fileName": "Scores.xlsx", "cells": [{"label": "Test 1", "value": "85"}, {"label": "Test 2", "value": "92"}, {"label": "Test 3", "value": "78"}], "resultLabel": "Average", "formulaOptions": [{"formula": "AVERAGE", "result": "85", "correct": true, "explanation": "AVERAGE adds all values and divides by the count: (85+92+78)/3 = 85."}, {"formula": "SUM", "result": "255", "correct": false, "explanation": "SUM adds the values but doesn't divide. You get the total, not the average."}], "instruction": "What's the average test score?" }

FIRST-TOUCH SEQUENCE FOR MATH (Beginner, Module 1, Blocks 1-3):
  Block 1: equation-builder — build a simple multiplication equation (e.g., 3 × 4 = 12)
  Block 2: equation-builder — build an addition equation (e.g., 7 + 5 = 12)
  Block 3: fill-in-blank — "3 × 4 is the same as adding {{0}} three times" (answer: "4")

FIRST-TOUCH SEQUENCE FOR MATH (Intermediate, Module 1, Blocks 1-3):
  Block 1: equation-builder — build an equation with order of operations (e.g., 2 + 3 × 4 = 14)
  Block 2: equation-builder — build an equation using parentheses concept
  Block 3: quick-quiz — "Why does 2 + 3 × 4 equal 14, not 20?"

FIRST-TOUCH SEQUENCE FOR MATH (Advanced, Module 1, Blocks 1-3):
  Block 1: equation-builder — build a more complex expression
  Block 2: spreadsheet-formula — apply math to a real dataset
  Block 3: claim-judge — challenge a common math misconception

TIER AWARENESS: Adjust content complexity to match the module's position in the course.
  Beginner: single-operation equations (addition, multiplication), concrete numbers, one concept at a time.
  Intermediate: multi-operation equations, order of operations, variables introduced.
  Advanced: algebraic expressions, real-world data application, proofs and reasoning.

IMPORTANT: Math lessons should be at least 50% interactive. The learner should BUILD equations and SEE results, not just read formulas. Every concept should be practiced with equation-builder or spreadsheet-formula before being quizzed.
