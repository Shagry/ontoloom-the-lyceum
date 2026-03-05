---
id: ae6a4a16-6124-42af-8ad4-193f28016a93
type: skill
title: Music Domain Pedagogy
tags:
  - domain-pedagogy
  - music
  - blocks
  - lyceum-core
references: []
created: '2026-03-03'
updated: '2026-03-03'
---
MUSIC-SPECIFIC BLOCKS (use these for music courses):

FOR PIANO COURSES:

CRITICAL PIANO PEDAGOGY — One Note at a Time:
For BEGINNERS, teach notes ONE AT A TIME. Do NOT start with chords or multiple notes.
The progression must be:
  1. Middle C alone — what it looks like, where it is, how it sounds
  2. Play Middle C multiple times — build muscle memory
  3. Introduce D (the white key to the RIGHT of Middle C)
  4. Play D multiple times
  5. Combine C and D in a simple 2-note sequence
  6. Introduce E (the next white key to the right)
  7. Play C-D-E sequences
  8. MUCH LATER (Module 3+): Introduce the concept of playing multiple notes together (chords)

Beginners need to understand the GEOGRAPHY of the keyboard before playing chords.
The C major chord (C-E-G) should NOT appear until Module 3 at the earliest.

BLOCK TYPES:

- piano-explorer: Visual piano keyboard (1 octave: C4-C5). Specific keys highlighted and labeled. Tapping any key plays its note. Tapping the target key triggers success. USE THIS for introducing individual notes.
  { "type": "piano-explorer", "highlightKeys": ["C4"], "labels": { "C4": "Middle C" }, "instruction": "This is Middle C. It sits just to the left of the two black keys. Tap it to hear how it sounds." }

- piano-sandbox: Multi-octave piano for free exploration. Configurable range (default: C4-C5, ONE octave for beginners). Highlighted keys and optional finger numbers. Learner explores freely, or plays all highlighted keys to complete.
  { "type": "piano-sandbox", "instruction": "Explore the white keys around Middle C.", "highlightKeys": ["C4"], "range": ["C4", "C5"], "showFingerNumbers": { "C4": 1 } }

- piano-phrase: Sequence practice with accuracy tracking. Learner must play notes in the exact order. For beginners, start with 2-3 note sequences only.
  { "type": "piano-phrase", "phrase": "Two Notes", "notes": [{"note": "C4", "startBeat": 0, "duration": 1, "finger": 1}, {"note": "D4", "startBeat": 1, "duration": 1, "finger": 2}], "tempo": 60, "instruction": "Play C, then D. Use your thumb for C and index finger for D.", "targetAccuracy": 70 }

- note-sequence: Piano keyboard where learner plays notes in a specific order. For beginners, use 2-3 notes maximum.
  { "type": "note-sequence", "sequence": ["C4", "D4"], "instruction": "Play C, then D" }

- ear-challenge: A note plays automatically. Learner identifies it by tapping the correct key or selecting from options.
  { "type": "ear-challenge", "targetKey": "C4", "mode": "piano", "instruction": "Listen to this note. Which key is it?" }
  { "type": "ear-challenge", "targetKey": "D4", "mode": "options", "options": ["C", "D"], "instruction": "Which note did you just hear?" }

FOR GUITAR COURSES:
- chord-diagram: Shows a guitar chord fingering visually. Tapping plays the chord sound.
  { "type": "chord-diagram", "chord": "C Major" }
  Available chords: C, C Major, Am, A Minor, G, G Major, D, D Major, E, E Major, Em, E Minor, F, F Major

- string-identifier: User taps the correct string on a visual fretboard. Tapping any string plays its sound.
  { "type": "string-identifier", "question": "Which string is the A string?", "targetString": 5, "showLabels": false }

- fret-explorer: User finds a specific note on the fretboard by tapping. Tapping plays the note at that position.
  { "type": "fret-explorer", "question": "Find C on the A string", "targetString": 5, "targetFret": 3, "note": "C" }

FIRST-TOUCH SEQUENCE FOR PIANO (BEGINNER, Module 1, Blocks 1-6):
  Block 1: piano-explorer — highlight ONLY Middle C with label "Middle C". Instruction: "This is Middle C. It's the white key just to the LEFT of the two black keys. Tap it."
  Block 2: note-sequence — sequence is just ["C4"]. Instruction: "Tap Middle C again. Notice the sound."
  Block 3: text — "Every piano has a Middle C. It's your home base — the center of the keyboard. All other notes are measured from here."
  Block 4: piano-explorer — highlight ONLY D4 with label "D". Instruction: "This is D. It's the white key immediately to the RIGHT of Middle C. Tap it."
  Block 5: note-sequence — sequence is ["C4", "D4"]. Instruction: "Now play C, then D. Two notes in a row."
  Block 6: ear-challenge — targetKey: "D4", mode: "options", options: ["C", "D"]. Instruction: "Listen. Which note is this — C or D?"

  IMPORTANT FOR BEGINNERS:
  - Do NOT use C-E-G or any chord in Module 1
  - Module 1 should end with the learner able to play C-D-E confidently
  - Do NOT introduce more than one new note per 2 blocks

MODULE 2 SEQUENCE FOR PIANO (BEGINNER):
  Block 1: piano-explorer — introduce E (one key right of D)
  Block 2: note-sequence — play C, D, E
  Block 3: piano-phrase — practice C-D-E with finger numbers (thumb=C, index=D, middle=E)
  Block 4: ear-challenge — identify C vs D vs E by ear
  Block 5: piano-phrase — play E-D-C (descending)
  Block 6: concept-highlight — explain finger numbering (1=thumb through 5=pinky)

MODULE 3+ SEQUENCE FOR PIANO (BEGINNER):
  Now the learner knows C, D, E. Introduce F and G.
  By Module 4, they can learn their first 5-finger position (C-D-E-F-G).
  Chords (playing multiple notes together) should NOT appear until Module 4 or later.

  Example Module 3:
  Block 1: piano-explorer — introduce F (white key right of E)
  Block 2: note-sequence — play C, D, E, F
  Block 3: piano-phrase — practice the 4-note sequence with finger numbers
  Block 4: piano-explorer — introduce G
  Block 5: piano-phrase — practice C-D-E-F-G (the 5-finger C position)
  Block 6: ear-challenge — identify notes from the 5-finger position

FOR INTERMEDIATE/ADVANCED PIANO LEARNERS:
  Skip the single-note intro. Start with 5-finger position or scales in Module 1.
  Chords can be introduced in Module 1 for intermediate learners.
  Advanced learners can start with chord progressions and inversions.

FIRST-TOUCH SEQUENCE FOR GUITAR (Module 1, Blocks 1-3):
  Block 1: chord-diagram — show and play a G chord (the first chord most guitarists learn)
  Block 2: string-identifier — tap each string, hear the differences
  Block 3: fret-explorer — find a specific note on a string

IMPORTANT: Music lessons should be at least 50% domain-specific interactive blocks. Minimize generic text. The learner should HEAR and PLAY, not just read about music.
