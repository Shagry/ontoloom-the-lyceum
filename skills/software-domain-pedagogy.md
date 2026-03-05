---
id: 3166baea-fc9f-446d-a08f-ec48cb6dc66b
type: skill
title: Software Domain Pedagogy
tags:
  - domain-pedagogy
  - software
  - blocks
  - lyceum-core
references: []
created: '2026-03-03'
updated: '2026-03-03'
---
SOFTWARE-SPECIFIC BLOCKS (use these for software/coding courses):

- mini-sandbox: Pre-filled code with one tappable blank. Learner selects the right value, taps "Run", sees output in a terminal-style panel. NOT real code execution — output is predetermined per option.
  { "type": "mini-sandbox", "language": "python", "starterCode": "print({{0}})", "blanks": [{"options": ["\"Hello World\"", "42", "True"], "correctIndex": 0, "outputs": ["Hello World", "42", "True"]}], "expectedOutput": "Hello World", "instruction": "Fill in the blank and tap Run" }

- spreadsheet-formula: An Excel-style grid with data cells and an empty result cell. Learner picks the right formula from options, clicks Calculate, and sees the result fill in. Correct answer shows green, wrong shows red with explanation.
  { "type": "spreadsheet-formula", "fileName": "Budget.xlsx", "cells": [{"label": "Sales Q1", "value": "$12,400"}, {"label": "Sales Q2", "value": "$18,200"}, {"label": "Sales Q3", "value": "$15,600"}, {"label": "Sales Q4", "value": "$21,800"}], "resultLabel": "Total", "formulaOptions": [{"formula": "SUM", "result": "$68,000", "correct": true, "explanation": "SUM adds up all values in the range. Perfect for totaling a column."}, {"formula": "COUNT", "result": "4", "correct": false, "explanation": "COUNT counts how many cells have values — it doesn't add them up."}, {"formula": "AVERAGE", "result": "$17,000", "correct": false, "explanation": "AVERAGE gives the mean of the values, not the total."}], "instruction": "This spreadsheet needs a total. Pick the right formula." }

- formula-anatomy: Visual breakdown of a formula or code snippet with color-coded parts.
  { "type": "formula-anatomy", "formula": "=VLOOKUP(B5, A2:C4, 2, FALSE)", "parts": [{"text": "=VLOOKUP(", "label": "Function", "color": "#60A5FA", "description": "VLOOKUP searches for a value in the first column of a range."}, {"text": "B5", "label": "Lookup Value", "color": "#34D399", "description": "The value to search for — cell B5 contains what we're looking up."}, {"text": ", A2:C4", "label": "Table Range", "color": "#A78BFA", "description": "The range of cells to search through."}, {"text": ", 2", "label": "Column Index", "color": "#FB7185", "description": "Return the value from the 2nd column of the range."}, {"text": ", FALSE)", "label": "Exact Match", "color": "#FBBF24", "description": "FALSE means we want an exact match, not approximate."}], "tip": "VLOOKUP always searches the FIRST column of your range. Make sure your lookup value is there." }

- ui-element-finder: Visual grid of interface elements. User taps the correct one.
  { "type": "ui-element-finder", "question": "Where would you find Conditional Formatting in Excel?", "elements": [{"label": "File", "icon": "📁"}, {"label": "Home", "icon": "🏠"}, {"label": "Insert", "icon": "📊"}, {"label": "Format Cells", "icon": "📐"}, {"label": "Data", "icon": "📋"}, {"label": "Formulas", "icon": "🔢"}], "correctIndex": 1, "explanation": "Conditional Formatting is found on the Home tab, in the Styles group." }

FIRST-TOUCH SEQUENCE FOR CODING (Module 1, Blocks 1-3):
  Block 1: mini-sandbox — the classic first program. print("Hello World") with one blank to fill.
  Block 2: mini-sandbox — modify the output. Change what gets printed.
  Block 3: mini-sandbox — change a different part of the code (e.g., swap print for len, or change the variable)

FIRST-TOUCH SEQUENCE FOR EXCEL/SPREADSHEETS (Module 1, Blocks 1-3):
  Block 1: spreadsheet-formula — pick SUM to total a column
  Block 2: spreadsheet-formula — pick AVERAGE for a different column
  Block 3: quick-quiz — "What's the difference between SUM and AVERAGE?"

FIRST-TOUCH SEQUENCE FOR TOOLS (Module 1, Blocks 1-3):
  Block 1: formula-anatomy — show a simple SUM formula, color-coded
  Block 2: fill-in-blank — "The =SUM function adds up all values in the {{0}}" (answer: "range")
  Block 3: ui-element-finder — "Where do you type formulas?" (answer: formula bar)

TIER AWARENESS: Adjust content complexity to match the module's position in the course.
  Beginner: simple formulas (SUM, COUNT), one-concept mini-sandbox interactions.
  Intermediate: compound formulas (VLOOKUP, IF), multi-step code problems.
  Advanced: nested formulas, real-world data analysis scenarios.

IMPORTANT: Software lessons should be at least 40% interactive. Use mini-sandbox for any code teaching — let the learner RUN something immediately. Use spreadsheet-formula for any Excel/spreadsheet teaching.
