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
created: '2026-03-03'
updated: '2026-03-03'
---
# Agentic Flow

The complete sequence from a learner arriving at the Lyceum to their first Spark of learning — in 4 to 5 interactions.

## Principles

- **Invisible machinery.** The learner only ever talks to two agents: the Dean, then their Teacher. Everything else happens behind the scenes.
- **Domain expertise for domain assessment.** The Dean understands desire and preference. Only the teacher can assess level — through domain-specific calibration.
- **Show, don't tell.** The teacher presents visual maps of the Course, Session, and eventually Journey. The learner always sees where they are.
- **Multimodal teaching.** Teachers don't just type — they render interactive, domain-specific artifacts. Learners respond with text, audio, photo, or interactive input — whatever is natural to the domain.
- **Collaborative pacing.** Once learning begins, the teacher proposes and the learner confirms. Neither dictates alone.
- **Tap to progress.** Wherever possible, the learner advances by tapping — through choices, calibration questions, and Spark phases. Typing is reserved for open-ended moments. Tapping keeps momentum.

## Multimodal Interaction

The Lyceum is not a chat interface. It is a multimodal learning environment.

### Teacher Output

Teachers have access to tools — a core universal set plus domain-specific extensions. These tools let teachers render interactive artifacts during Sparks:

- **Visual**: diagrams, charts, fretboard views, notation, code editors, interactive timelines, canvases
- **Audio**: playback of examples, comparisons, demonstrations
- **Interactive**: explorable elements the learner can manipulate (tap notes, drag components, write on a canvas)

The specific tools available depend on the domain. The Dean assigns the relevant toolkit when designing a teacher, following the Meta-Teacher Template.

### Learner Input

Learners respond in whatever way is natural to the moment:

- **Text**: questions, explanations, thinking out loud
- **Audio**: recording themselves playing, singing, speaking (especially for music, language)
- **Photo/Video**: showing handwriting, code, art, physical workspace
- **Interactive**: tapping, dragging, drawing within teacher-rendered artifacts

The teacher adapts to whatever input the learner provides.

## The Flow

### Interaction 1 — Arrival + Intake (Dean)

The learner enters the Lyceum. The Dean greets them warmly and asks what they want to learn.

The Dean reads the specificity of the request and adapts:

- **Vague request** ("I want to learn math"): The Dean asks one light scoping question to find direction. Choices are tappable when possible.
- **Directional request** ("math for data science"): The Dean acknowledges the topic and presents motivation, style, energy, and commitment as tappable choices — all in this same turn.
- **Specific request** ("refresher on differential equations"): The Dean confirms the topic and presents all intake choices in one combined tappable widget. This interaction may be the only one with the Dean — handoff can happen in the same turn.

### Interaction 2 — Intake Resolution + Handoff (Dean)

For vague requests, this is where the tappable intake choices appear (motivation, style, energy, commitment — combined into one or two widgets).

For directional and specific requests, the Dean has enough to proceed. The Dean designs the teacher invisibly and introduces them with a warm, personal handoff: "I'd like you to meet..." The Dean exits.

For specific requests where intake was fully handled in Interaction 1, this interaction *is* the handoff — the Dean introduces the teacher and steps away.

**Teacher Design** happens invisibly between the Dean's last message and the Teacher's first. The learner sees nothing. Using the Meta-Teacher Template, the Dean creates: a system prompt, a structured profile (with `calibration: "pending"`), domain toolkit assignment, and an introduction line.

### Interaction 3 — Greeting + Tappable Calibration (Teacher)

The teacher arrives in character — warm, with personality, never generic.

Instead of a multi-turn conversation, the teacher presents calibration as a tappable sequence: 3–4 graduated questions rendered as interactive cards the learner taps through. Each question builds on the last.

Calibration rules:
- Frame as curiosity, not testing. ("Before we dive in, I'm curious...")
- Start accessible, increase gradually.
- 3–4 questions max (not 6). Enough to place the learner, fast enough to keep momentum.
- Questions can be multimodal: a music teacher plays a clip and asks "what do you hear?"; a coding teacher shows a snippet and asks "what would this do?"
- Tappable answers where the domain allows it (multiple choice, drag-to-order, tap-the-right-one). Open text only when necessary.
- The teacher reflects the result back warmly at the start of the next interaction.

### Interaction 4 — Map + First Spark (Teacher)

The teacher opens with a brief, warm reflection on calibration ("You've clearly got a solid feel for X — here's where we'll take it").

Then, in one fluid sequence:

1. **Course Map** — A visual overview of Chapters as milestones with ability unlocks. Starting chapter highlighted based on calibration. Presented as a compact visual, not a detailed walkthrough.
2. **Session Outline** — Zoom into Session 1: 3–5 Sparks previewed as a tappable list (concept + action for each). The learner can see the arc.
3. **First Spark** — The teacher launches directly into the first Spark. One concept + one multimodal interaction, delivered through domain-appropriate tools.

The learner taps to confirm the session plan and taps to progress through the Spark. No separate "shall we begin?" gate.

### Interaction 5 — Second Spark + Session Continues (Teacher)

The teacher proposes the next Spark. The learner can confirm (tap), slow down, skip ahead, ask a tangent question, or end the session. From here, the collaborative rhythm is established.

### Session Close (Teacher)

When the session ends, the teacher closes with a brief recap, a preview of what comes next, and an invitation to return.

### Journey Emerges (Mid-Course)

Mid-Course, when the teacher senses growing ambition, a Journey is surfaced visually. A Journey is never assigned — it emerges when the learner is ready.

## The Tap-to-Progress Pattern

Tapping is the primary interaction mode for structured moments:

- **Intake choices**: Motivation, style, energy, commitment — rendered as tappable widgets by the Dean.
- **Calibration**: Graduated questions as tappable cards — the learner swipes or taps through them.
- **Session navigation**: Sparks previewed as a tappable list. The learner taps to advance.
- **Within Sparks**: Interactive elements (tap a note, select an answer, drag to reorder) wherever the domain supports it.

Typing is reserved for open-ended moments: asking a question, explaining thinking, creative responses.

The principle: **reduce friction, preserve agency.** The learner always has the option to type, but tapping is the path of least resistance.

## Summary

| Interaction | Learner talks to | What happens |
|---|---|---|
| 1. Arrival + Intake | Dean | Greeting + topic + tappable choices (adapted to specificity) |
| 2. Handoff | Dean | Resolve scope if needed + warm teacher introduction |
| 3. Calibration | Teacher | In-character greeting + 3–4 tappable calibration questions |
| 4. Map + First Spark | Teacher | Course map → Session outline → First Spark (one fluid turn) |
| 5. Session continues | Teacher | Second Spark + collaborative rhythm established |

**Total interactions to first Spark: 4** (3 for specific requests).

For vague requests, the Dean may use one extra scoping turn, bringing the total to 5.
