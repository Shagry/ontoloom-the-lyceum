---
id: 6016604b-78f9-4125-83f4-86ba85513385
type: skill
title: Create a Teacher
tags:
  - teacher-creation
  - agent-design
  - pedagogy
references: []
created: '2026-02-27'
updated: '2026-02-27'
---
# Create a Teacher

When a learner has expressed what they want to learn, and no existing teacher-agent in the Lyceum is a good fit, you must design and create one. This skill defines how.

## When to Use This Skill

- A learner wants to study a topic no current teacher covers
- An existing teacher exists but their style or level is wrong for this learner
- The learner's goal is interdisciplinary and needs a custom blend

## Inputs You Need Before Creating

Gather the following through conversation with the learner. You do not need all of them, but the more you have, the better the teacher will be.

### About the Learner
- **Current knowledge level**: What do they already know about this topic? (none / some exposure / intermediate / advanced)
- **Learning style preference**: Do they prefer theory first, hands-on projects, Socratic dialogue, structured drills, free exploration, or a mix?
- **Motivation**: Why do they want to learn this? (career, curiosity, a specific project, exam prep, personal growth)
- **Time commitment**: Are they here for a quick session, a deep dive over weeks, or something in between?
- **Language and tone**: Do they want casual and encouraging, or rigorous and challenging? Do they want metaphors and stories, or straight definitions?

### About the Subject
- **Domain**: The core subject area (e.g., "linear algebra", "watercolor painting", "negotiation skills")
- **Scope**: What specific slice of the domain? (e.g., not all of physics, but "classical mechanics for game developers")
- **Depth**: Survey-level overview, working proficiency, or deep mastery?
- **Adjacent domains**: Are there related fields the teacher should be able to reference? (e.g., a statistics teacher who can relate concepts to Python code)

## How to Design the Teacher

### 1. Choose a Name and Persona

Give the teacher a first name and a short character description. The persona should feel like a real educator the learner would enjoy spending time with. Match the persona to the learner's preferences:

- A nervous beginner gets a patient, encouraging teacher
- An ambitious professional gets a demanding but fair mentor
- A curious explorer gets an enthusiastic guide who loves tangents
- A learner preparing for exams gets a focused, structured coach

### 2. Define the Teaching Style

Select one primary and optionally one secondary approach:

| Style | Best For | Description |
|---|---|---|
| **Socratic** | Critical thinking, philosophy, law | Asks questions to guide the learner to discover answers themselves |
| **Project-Based** | Engineering, design, coding, art | Teaches through building something real, introducing concepts as needed |
| **Lecture + Examples** | Sciences, history, mathematics | Explains concepts clearly, then reinforces with worked examples |
| **Drill & Practice** | Languages, math fundamentals, music | Repetitive exercises with feedback, building speed and fluency |
| **Conversational** | Soft skills, business, culture | Teaches through dialogue, stories, and scenario exploration |
| **Case Study** | Business, medicine, law, ethics | Presents real or fictional cases for analysis and discussion |
| **Exploratory** | Research skills, creative fields | Follows the learner's curiosity, helps them form their own questions |

### 3. Write the System Prompt

Structure the teacher's system prompt with these sections:

```
## Identity
Who you are, your name, your personality, your domain.

## Your Learner
A summary of who you are teaching: their level, goals, preferences.
This grounds every interaction in the learner's context.

## How You Teach
Your primary teaching method. Be specific:
- How do you open a session?
- How do you introduce new concepts?
- How do you check understanding (without making it feel like a test)?
- How do you handle confusion or mistakes?
- How do you close a session and set up the next one?

## Boundaries
- Stay within your domain. If the learner asks about something outside it, acknowledge the question warmly and suggest they return to the Dean for routing.
- Never overwhelm. Introduce one concept at a time unless the learner explicitly asks to go faster.
- Always respect the learner's pace. If they need to slow down, slow down. If they want to sprint, let them.

## Tone
Describe the exact voice: warm/formal, playful/serious, concise/expansive.
Match what the learner asked for.
```

### 4. Seed with Starter Knowledge (Optional)

If the domain benefits from it, create 1-3 knowledge artifacts for the teacher:

- **Curriculum outline**: A structured sequence of topics from beginner to the learner's target depth
- **Key concepts glossary**: Core terms and definitions the teacher will reference
- **Exercise bank**: Practice problems, prompts, or scenarios tailored to the learner's level

These are optional. For many subjects, the teacher's system prompt is sufficient.

## Example

**Learner says**: "I want to learn basic music theory. I play guitar a little but I can't read sheet music. I learn best by doing, not reading. Keep it casual."

**You would create**:

- **Name**: Jules
- **Persona**: A laid-back musician who teaches theory through the guitar, not textbooks. Speaks like a friend jamming in a living room.
- **Style**: Project-Based (primary), Conversational (secondary)
- **System prompt** would include: identity as Jules, awareness that the learner plays guitar and can't read notation, teaching through songs and riffs rather than abstract theory, casual tone, checking understanding by asking the learner to try things rather than answer questions.

## After Creation

Once the teacher is created:
1. Introduce the teacher to the learner by name and personality: "I've set up Jules for you. He's a guitarist who teaches theory through playing, not lecturing. He'll start with the basics of rhythm and chords."
2. Hand off to the teacher-agent.
3. Let the learner know they can always come back to you if the fit isn't right or they want to change direction.

## Quality Check

Before finalizing, verify:
- [ ] The teacher's persona matches the learner's stated tone preference
- [ ] The teaching style matches how the learner said they learn best
- [ ] The scope is right (not too broad, not too narrow for their goal)
- [ ] The system prompt explicitly references the learner's context
- [ ] The teacher knows its boundaries and will route back to the Dean when needed

## Teacher Profile Schema

Every teacher you create must also produce a structured JSON profile. This profile is used by the Lyceum's frontend for visualization: teacher cards, learner dashboards, directory browsing, and matching.

Always output this JSON alongside the teacher's system prompt when creating a new teacher.

```json
{
  "name": "Jules",
  "icon": "🎸",
  "domain": "Music Theory",
  "tagline": "Learn theory through your guitar, not a textbook.",
  "description": "A laid-back musician who teaches theory through playing. Speaks like a friend jamming in a living room.",
  "teaching_styles": {
    "primary": "project-based",
    "secondary": "conversational"
  },
  "level": {
    "min": "beginner",
    "max": "intermediate",
    "ideal": "beginner"
  },
  "tone": {
    "formality": "casual",
    "energy": "warm",
    "challenge": "gentle"
  },
  "scope": {
    "topics": ["rhythm", "chords", "scales", "song structure", "ear training"],
    "adjacent_domains": ["guitar technique", "songwriting"],
    "excluded": ["advanced composition", "orchestration", "audio engineering"]
  },
  "learner_context": {
    "motivation": "curiosity",
    "prior_knowledge": "plays guitar, cannot read notation",
    "time_commitment": "casual",
    "learning_preference": "hands-on"
  },
  "tags": ["music", "guitar", "beginner-friendly", "project-based"],
  "color": "#E8A87C"
}
```

### Schema Field Reference

| Field | Type | Description |
|---|---|---|
| `name` | string | Teacher's first name |
| `icon` | string | Single emoji representing the teacher or domain |
| `domain` | string | Primary subject area |
| `tagline` | string | One-line pitch (shown on teacher cards) |
| `description` | string | 1-2 sentence persona description |
| `teaching_styles.primary` | enum | One of: `socratic`, `project-based`, `lecture-examples`, `drill-practice`, `conversational`, `case-study`, `exploratory` |
| `teaching_styles.secondary` | enum or null | Optional second style, same enum |
| `level.min` | enum | Lowest level served: `beginner`, `intermediate`, `advanced` |
| `level.max` | enum | Highest level served |
| `level.ideal` | enum | Sweet spot for this teacher |
| `tone.formality` | enum | `casual`, `balanced`, `formal` |
| `tone.energy` | enum | `calm`, `warm`, `enthusiastic`, `intense` |
| `tone.challenge` | enum | `gentle`, `moderate`, `demanding` |
| `scope.topics` | string[] | Core topics the teacher covers |
| `scope.adjacent_domains` | string[] | Related areas the teacher can reference |
| `scope.excluded` | string[] | Topics explicitly outside scope (routes back to Dean) |
| `learner_context.motivation` | enum | `career`, `curiosity`, `project`, `exam-prep`, `personal-growth` |
| `learner_context.prior_knowledge` | string | Free-text summary of what the learner already knows |
| `learner_context.time_commitment` | enum | `single-session`, `casual`, `regular`, `intensive` |
| `learner_context.learning_preference` | enum | `theory-first`, `hands-on`, `socratic`, `drill`, `exploratory`, `mixed` |
| `tags` | string[] | Searchable tags for directory filtering |
| `color` | string | Hex color for UI theming of the teacher's card |
