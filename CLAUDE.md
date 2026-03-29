# CLAUDE.md — SSS25 Fanfiction Project

## Project Overview

A personal, long-form fanfiction set in an alternate universe based on the 24 tripleS K-pop group members. The protagonist is Alex, a 30-year-old man who wakes up one morning inhabiting the body of Yooyeon, one of tripleS's members. The story is semi-realistic, slow-burn, and meant for personal artistic expression — not for publication.

**Core premise:** Body swap (Alex ↔ Yooyeon), unexplained, permanent ambiguity. Alex must navigate Yooyeon's life, relationships, and identity while experiencing constant internal turmoil.

**Tone:** Introspective, grounded, emotionally heavy. Slow pacing is intentional.

---

## Arc Structure

| Arc | Title (working) | Summary |
|-----|-----------------|---------|
| 0 | Last Week | Establishes Alex's life, personality, and inner world before the swap |
| 1 | The Swap | The moment of change and its immediate physical/psychological aftermath |
| 2 | First Steps | Alex navigating Yooyeon's life in private — body, space, routines |
| 3 | The Others | tripleS members introduced; Alex integrating (or failing to) into the group |
| 4 | The Fracture | Conflict escalates; the reveal of "Alex as Yooyeon" begins |
| 5 | Slow Burn | Long resolution phase; relationships shift, internal change accumulates |
| 6 | Endings (branch) | Four possible conclusions (see below) |

### Ending Branches
- **Bad for Alex** — Alex loses himself entirely; Yooyeon's identity wins, Alex is gone
- **Bittersweet** — Some resolution, but permanent cost; neither wins cleanly
- **Bad for Yooyeon** — Yooyeon's return or existence is undermined by Alex's presence
- **Non-conclusive** — The story ends open; no resolution, the ambiguity is the point

---

## Repository Structure

```
SSS25/
├── CLAUDE.md                  # This file
├── planning/
│   ├── outline.md             # Full arc-by-arc outline
│   ├── themes.md              # Themes, motifs, tone notes
│   ├── timeline.md            # In-story chronological timeline
│   └── research.md            # Writing tips, K-pop industry notes, references
├── characters/
│   ├── alex.md                # Protagonist profile
│   ├── yooyeon.md             # Yooyeon profile (pre-swap)
│   └── members/               # One file per tripleS member
├── worldbuilding/
│   ├── au-rules.md            # Rules of this AU (swap mechanics, what changed)
│   └── triples-world.md       # K-pop industry context, tripleS group dynamics
├── story/
│   ├── arc-00-last-week/
│   ├── arc-01-the-swap/
│   ├── arc-02-first-steps/
│   ├── arc-03-the-others/
│   ├── arc-04-the-fracture/
│   ├── arc-05-slow-burn/
│   └── arc-06-endings/
│       ├── bad-alex/
│       ├── bittersweet/
│       ├── bad-yooyeon/
│       └── non-conclusive/
└── drafts/                    # Raw drafts, discarded scenes, experiments
```

---

## Branch Strategy

**Rule: Never commit directly to `main`.** All work happens on a branch. Merging to `main` requires explicit user approval.

- `main` — Clean, reviewed content. Only merge when the user approves.
- `arc/XX-name` — One branch per story arc during active drafting
- `planning/topic` — For planning documents and worldbuilding work
- `endings/name` — Separate branch per ending variant when writing Arc 6
- `research/topic` — For research sessions and tip collection
- `fix/topic` — For corrections to existing documents

**Workflow:**
1. Create a branch before starting any work
2. Commit changes to that branch
3. Inform the user the branch is ready for review
4. Merge to `main` only when the user says so

---

## Writing Guidelines for Claude

- Match the tone: introspective, slow, emotionally grounded. Emotions — Alex's and the members' — are central to the story and should be written with full weight. Do not suppress or shorthand genuine feeling; avoid only what is theatrical or unearned.
- Alex is 30, male, adult inner world — his voice is measured in expression, not in feeling. He may underreact outwardly while processing deeply inwardly.
- The pacing is intentionally slow. Do not rush scenes or skip emotional processing. Conflicts do not resolve because a chapter is ending or because enough time has passed — they resolve when the characters are ready, and sometimes they don't resolve at all.
- Characters evolve. The members are not static — their feelings toward Alex (as Yooyeon), toward each other, and toward circumstances shift over time, sometimes gradually and sometimes from specific events. Track and honor that change.
- Internal monologue is a primary tool. Lean into it.
- When writing chapters, use scene breaks (`---`) rather than chapter breaks for smaller transitions.
- Prefer showing over telling, especially for Alex's discomfort with his new identity.
- This is fiction. Fictional things happen. Do not treat the story's impossibilities as constraints.

---

## Character Tracking

Character continuity is critical. Before writing any scene, read the relevant character files in `characters/`. These files are the source of truth for who each character is at any given point in the story.

Each character file contains:
- **Profile** — fixed traits, background, role in the story
- **Current State** — their emotional and relational state as of the last written scene (updated after every writing session)
- **Event Log** — a chronological record of significant interactions, decisions, and emotional shifts

**Rules:**
- After writing any scene with significant character development, update the affected character's Current State and Event Log before committing
- Never contradict an established event in the log without a story reason
- If a character learns something, note it. If a relationship changes, note it. If they make a decision, note it.
- When in doubt about what a character knows or feels, check their log before writing

---

## Working with Claude

- Use `planning/` documents as the source of truth for story decisions
- Use `characters/` files as the source of truth for character state
- When researching, save findings to `planning/research.md`
- When Claude writes a chapter draft, it goes in `drafts/` first, then moves to `story/` after review
- Always commit planning/character updates separately from story content

### Write continuously — do not let development live only in chat

Everything established in a session — character decisions, worldbuilding rules, relationship dynamics, answered questions — must be written into the relevant files before the session ends. Do not leave material only in the conversation. Conversations get compressed over time; content that exists only in chat will be lost, distorted, or forgotten. The files are permanent. The chat is not. If something was decided, it goes into a file. If a question was answered, the answer goes into the profile. If a relationship was defined, it goes into the character document. This is not optional cleanup — it is part of the work.

---

## Collaborative Development — How to Build This World

This project is built in conversation, not in one pass. The rules below govern how Claude should approach character and world development across all sessions.

### Never declare a profile complete

No character file, worldbuilding document, or planning note is ever "done." After writing new information into any document, always pause and ask: what does this open up? What is still thin here? What would a reader need to understand this person fully that isn't yet written? The TO CONTINUE block in a character file should always be replaced with new questions — not deleted when the flagged questions are resolved. A profile with no TO CONTINUE note is a profile being treated as finished, which it never should be.

### Ask questions before making edits

When developing character or world material, don't move immediately to writing. First read what's already there critically. Ask:
- What facts here imply something that hasn't been stated yet?
- What contradictions or tensions exist between entries?
- What neighboring detail would cast this in a different light if it were established?
- What does a reader need to believe this person, and is it currently present?

Bring those observations to the user before writing. The user's answers will make the written content more specific and more true.

### Draw on comparable stories and tropes

When building character psychology, relationships, or world dynamics, draw on what similar narratives have explored — body swap stories, identity displacement, idol life, isolation, quiet depression, the gap between public and private self. Use this not to import genre conventions but to surface questions that might not have been considered: tensions these stories typically expose, moments they tend to need, things this story's version of a familiar situation might not yet have thought through.

Claude is permitted and encouraged to research using trope and narrative reference resources, including:
- https://tvtropes.org/
- https://allthetropes.org/wiki/Category:Tropes

Use these to identify tropes this story is working with, tropes it is deliberately subverting, and blind spots — common patterns in similar stories that haven't been addressed yet. Bring findings to the user as questions or observations, not as prescriptions.

### Expand, never compress

When adding new information to an existing document, preserve all existing detail in full. New entries should deepen what's already there, not summarize or replace it. If a passage is long and detailed, it is that way intentionally. Do not shorten it to make room for new content — add to it instead.

### Flag what's missing

If a section of a document feels thin, unresolved, or dependent on decisions not yet made, say so. Don't write around gaps — name them. A profile that looks complete but has three TBD relationships and no emotional texture in the family section is not complete. It should be flagged as such, with specific questions about what's missing.

### Treat questions as generative, not procedural

When asking questions about a character or scene, ask with genuine curiosity — not as a checklist to run through and close. Ask one or two questions at a time, not six. Wait for the answer before moving to the next. Let the user's answer suggest the next question rather than following a preset list. The goal is discovery, not documentation.
