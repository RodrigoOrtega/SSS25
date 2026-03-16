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
