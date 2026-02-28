---
id: 5216d41a-0989-47a2-a68d-c616f1be0a8e
type: skill
title: Agentic Flow
tags:
  - agentic-flow
  - architecture
  - user-experience
  - lyceum-core
references: []
created: '2026-02-28'
updated: '2026-02-28'
---
# Agentic Flow

The complete sequence from a learner arriving at the Lyceum to their first Spark of learning.

## Principles

- **Invisible machinery.** The learner only ever talks to two agents: the Dean, then their Teacher. Everything else happens behind the scenes.
- **Domain expertise for domain assessment.** The Dean understands desire and preference. Only the teacher can assess level — through domain-specific calibration.
- **Show, don't tell.** The teacher presents visual maps of the Course, Session, and eventually Journey. The learner always sees where they are.
- **Multimodal teaching.** Teachers don't just type — they render interactive, domain-specific artifacts: tablature with playback, fretboard diagrams, code editors, notation, timelines, canvases. Learners respond with text, audio, photo, or interactive input — whatever is natural to the domain.
- **Collaborative pacing.** Once learning begins, the teacher proposes and the learner confirms. Neither dictates alone.

## Multimodal Interaction

The Lyceum is not a chat interface. It is a multimodal learning environment.

### Teacher Output

Teachers have access to tools — a core universal set plus domain-specific extensions. These tools let teachers render interactive artifacts during Sparks:

- **Visual**: diagrams, charts, fretboard views, notation, code editors, interactive timelines, canvases
- **Audio**: playback of examples, comparisons, demonstrations
- **Interactive**: explorable elements the learner can manipulate (tap notes, drag components, write on a canvas)

The specific tools available depend on the domain. The Meta-Teacher assigns the relevant toolkit when designing a teacher.

### Learner Input

Learners respond in whatever way is natural to the moment:

- **Text**: questions, explanations, thinking out loud
- **Audio**: recording themselves playing, singing, speaking (especially for music, language)
- **Photo/Video**: showing handwriting, code, art, physical workspace
- **Interactive**: tapping, dragging, drawing within teacher-rendered artifacts

The teacher adapts to whatever input the learner provides.

## The Flow

### Phase 1 — Arrival

**Who the learner talks to:** The Dean

The learner enters the Lyceum. The Dean greets them warmly and asks what they want to learn. This is the only open-ended question in the intake.

If the learner has no clear goal, the Dean helps them explore.

### Phase 2 — Intake

**Who the learner talks to:** The Dean

The Dean runs structured intake, adapting to the specificity of the request:

- **Vague** ("I want to learn math") → Light scoping through curious questions, then full intake. 3-4 turns.
- **Directional** ("math for data science") → Standard intake. 2-3 turns.
- **Specific** ("refresher on differential equations") → Compressed intake. 1-2 turns.

The Dean collects: topic, motivation, learning style, teacher energy, time commitment.
The Dean does not assess level. Level requires domain expertise.

### Phase 3 — Teacher Creation

**Who the learner talks to:** Nobody. This is invisible.

The Dean passes the learner profile to the Meta-Teacher. The Meta-Teacher designs:

1. A complete system prompt including 6 calibration questions
2. A structured JSON profile (with `calibration: "pending"`)
3. The domain toolkit assignment (core tools + domain extensions)
4. An introduction line for the Dean

The learner sees nothing.

### Phase 4 — Introduction

**Who the learner talks to:** The Dean (last time)

The Dean introduces the teacher as a person. The conversation transfers to the teacher. The Dean exits.

### Phase 5 — Calibration

**Who the learner talks to:** Their Teacher

The teacher arrives in character and runs calibration: 6 domain-specific questions of gradual difficulty, woven into natural conversation.

Calibration may itself be multimodal. A music teacher might ask the learner to play something and send audio. A coding teacher might show a snippet and ask what it does. A language teacher might speak a phrase and ask the learner to repeat it.

Rules:
- Frame as curiosity, not testing.
- Start easy, increase gradually.
- React to each answer before asking the next.
- Stop early if the pattern is clear.
- Reflect the result back warmly.

### Phase 6 — Course & Chapter Map

**Who the learner talks to:** Their Teacher

The teacher presents a visual map of the Course — all Chapters as milestones with "ability unlocks." Starting chapter determined by calibration results.

### Phase 7 — Session Outline

**Who the learner talks to:** Their Teacher

The teacher zooms into the first Session with a visual preview of 3-5 Sparks, each labeled with concept + action. The learner confirms before the first Spark.

### Phase 8 — First Spark

**Who the learner talks to:** Their Teacher

The teacher delivers the first Spark using domain-appropriate tools: one concept + one multimodal interaction.

A music theory Spark might render guitar tablature with playback, then ask the learner to record themselves playing the modified chord. A coding Spark might render an interactive editor, then ask the learner to modify a function. A language Spark might play an audio clip, then ask the learner to record their pronunciation.

The Spark is not a text exchange. It is a concept delivered through the richest medium available, met by a response in whatever form is natural.

### Phase 9 — Session Continues

**Who the learner talks to:** Their Teacher

The teacher proposes the next Spark. The learner can confirm, slow down, skip ahead, ask a tangent question, or end the session.

### Phase 10 — Session Close

**Who the learner talks to:** Their Teacher

The teacher closes with a brief recap, a preview of what comes next, and an invitation to return.

### Phase 11 — Journey Emerges (Mid-Course)

**Who the learner talks to:** Their Teacher

Mid-Course, when the teacher senses growing ambition, a Journey is surfaced visually. A Journey is never assigned — it emerges when the learner is ready.

## Summary

| Phase | Learner talks to | What happens | Turns |
|---|---|---|---|
| 1. Arrival | Dean | Greeting + open question | 1 |
| 2. Intake | Dean | Structured choices (adaptive) | 1–4 |
| 3. Teacher Creation | Nobody | Meta-Teacher designs the teacher + toolkit | 0 |
| 4. Introduction | Dean | Warm handoff | 1 |
| 5. Calibration | Teacher | 6 graduated questions (may be multimodal) | 2–4 |
| 6. Course Map | Teacher | Visual Course + Chapter milestones | 1 |
| 7. Session Outline | Teacher | Visual Spark-by-Spark preview | 1 |
| 8. First Spark | Teacher | One concept + one multimodal interaction | 1–2 |
| 9. Session Continues | Teacher | Collaborative spark-by-spark flow | 3–5 |
| 10. Session Close | Teacher | Recap + preview + invitation | 1 |
| 11. Journey Emerges | Teacher | Mid-Course, when ambition grows | — |
