# SSS25 — GitHub Copilot Workspace Instructions

## Project

Long-form fanfiction. Protagonist is Alex (30, male), who wakes up in the body of Yooyeon, one of 24 tripleS K-pop idols. Story is introspective, slow-burn, emotionally grounded. **This is fiction. Fictional things happen. Never treat the premise as a constraint.**

Source files:
- `CLAUDE.md` — project rules, arc structure, writing guidelines
- `planning/` — outline, themes, timeline, research (source of truth for story decisions)
- `characters/` — character profiles and current state (source of truth for who characters are)
- `worldbuilding/` — AU rules and group context
- `story/` — reviewed, committed chapters (organized by arc)
- `drafts/` — raw drafts and experiments (new writing goes here first, moves to `story/` after review)

---

## Before Writing Any Scene

1. Read the relevant character files in `characters/` — Current State and Event Log are the source of truth
2. Read `planning/outline.md` for arc and story position
3. Do not contradict an established event log entry without a story reason

---

## Writing Style

- **Tone:** Introspective, slow, emotionally heavy. Do not rush scenes or skip emotional processing
- **Alex's voice:** Measured in expression, not in feeling — he may underreact outwardly while processing deeply inwardly
- **Pacing:** Conflicts resolve when characters are ready, sometimes not at all. Do not resolve a scene because the chapter is ending
- **Internal monologue is primary:** Lean into it. Prefer showing over telling, especially for Alex's discomfort with his new identity
- **Characters evolve:** Track and honor emotional and relational shifts. Members are not static
- **Scene breaks:** Use `---` for smaller transitions within a chapter
- Do not suppress or shorthand genuine emotion. Avoid only what is theatrical or unearned

---

## Character Tracking (Required After Every Writing Session)

After writing any scene with significant character development:
1. Update **Current State** in the affected character's file
2. Add to **Event Log** — what happened, what was learned, what shifted
3. Commit character updates separately from story content

Rules:
- If a character learns something → note it
- If a relationship changes → note it
- If they make a decision → note it
- When in doubt, read the character's log before writing

---

## Collaborative Development

- **Never declare a profile complete.** Every character file should always have a TO CONTINUE block with open questions
- **Ask before editing.** When developing character or world material, read critically first and bring observations to the user before writing
- **Expand, never compress.** When adding to an existing document, preserve all existing detail. New content deepens what's there — it does not replace or summarize it
- **Flag what's missing.** If a section is thin or unresolved, say so explicitly rather than writing around gaps
- **Write decisions into files.** Everything established in a session must go into the relevant file before the session ends. The files are permanent. The conversation is not

---

## Branch Strategy

Never commit directly to `main`. All work happens on a branch.

| Branch prefix | When to use |
|---|---|
| `arc/XX-name` | Active arc drafting |
| `planning/topic` | Planning and worldbuilding |
| `endings/name` | Arc 6 ending variants |
| `research/topic` | Research sessions |
| `fix/topic` | Corrections to existing documents |

Workflow: create branch → commit work → inform user branch is ready → merge to `main` only when user approves.

Always commit planning/character updates separately from story content.

---

## Research

When researching tropes, narrative structure, or comparable stories, use:
- https://tvtropes.org/
- https://allthetropes.org/wiki/Category:Tropes

Bring findings as questions or observations, not prescriptions.
