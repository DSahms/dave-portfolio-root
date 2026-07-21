# Claude → Memory Export (Portfolio Standard)

**~4 minutes per project.** Run in each Claude project. Save the output yourself to the matching folder on your machine.

---

## The prompt (one prompt — copy every time)

Change only **`[PROJECT NAME]`** and **`[PROJECT]`** (same word, uppercase in filename).

```
Export everything you know about [PROJECT NAME] from this Claude project's instructions and conversation history. Output ONE markdown file only. No preamble.

Filename for the export: [PROJECT]_CLAUDE_MEMORY_EXPORT.md

Include: product identity, architecture, naming (current + dead names), decisions, contradictions, open threads, founder context if relevant, and anything you know that has never been written into a project file.

Do not reference local disk paths, folders, or drives. You may not have filesystem access — export from Claude memory only.

Mark each item: FACT / RECOLLECTION / OPEN

Format:
# [PROJECT] — Claude Memory Export
## Executive Summary
## Product Identity
## Architecture
## Decisions
## Contradictions & Stale Names
## Open Threads
## Only in Claude (not saved to a file yet)

Be exhaustive. Output only the markdown.
```

---

## Where Dave saves each export (for you — not for Claude)

| Done | Project | Save to |
|------|---------|---------|
| ✅ | NURA | `NURA Platform\NURA_CLAUDE_MEMORY_EXPORT.md` |
| ✅ | The Ledger Series | `The Ledger Series\The Ledger Series_CLAUDE_MEMORY_EXPORT.md` |
| ✅ | PersonaLock Desktop | `PersonaLock\PERSONALOCK_DESKTOP_CLAUDE_MEMORY_EXPORT.md` |
| ✅ | PersonaLock Mobile | `PersonaLock\PERSONALOCK_MOBILE_CLAUDE_MEMORY_EXPORT.md` |
| ✅ | StoryKeeper | `StoryKeeper\storykeeper_CLAUDE_MEMORY_EXPORT.md` |
| ⬜ | Panoptes Lens | `Panoptes Lens\PANOPTES_CLAUDE_MEMORY_EXPORT.md` |
| ⬜ | Daily Bread | `Daily bread\DAILY_BREAD_CLAUDE_MEMORY_EXPORT.md` |

**Priority:** Ledger → PersonaLock → StoryKeeper

---

## After drop-in (Cursor)

*"Read `[filename]` — Claude-origin context; verify against disk before acting."*
