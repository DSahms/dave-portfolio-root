# Stack positioning: Cursor, Arden, and Hermes

**For:** Context when comparing Hermes Desktop to what Dave already has  
**Date:** June 2026 · **Updated direction:** 2026-07-14 → see `D:\dev\BRAIN_COMPUTE_STRATEGY.md`

---

## Locked direction (July 2026)

| Role | Default |
|------|---------|
| **Arden** | The product people use (finish building this first) |
| **Hermes** | Agent layer — plan is **self-host in the cloud** (access anywhere, not stealing M40 from Arden) |
| **Cursor** | Dave’s builder only — never married into the consumer product |
| **Local brain** | Gemma-4-E4B on Kobold — prove cheap/edge; escalate heavy work to **Venice** |

Do not conflate model/card talk with NURA / Persona-Lock / Arden product work. Full canon: `BRAIN_COMPUTE_STRATEGY.md`.

---

## Context for this conversation

I'm not looking for a generic "what can AI do for me" answer. I already have a **stack with defined roles**. Hermes Desktop only earns a place if it does something **none of these already do**.

---

## What Cursor Pro + Composer 2.5 handles (the coding agent)

This is my **engineering partner** — it lives in the repo, not on my desktop as a chat buddy.

### Composer covers

- **Building and fixing software** — multi-file edits, refactors, debugging from real logs and stack traces
- **Running the ship loop** — build Arden, run acceptance tests, diagnose Venice/Kobold failures, repackage portable zips, fix CI-style issues **without me as the test harness**
- **Project memory in code** — knows `D:\dev\Arden\engine\`, Daily Bread, packaging scripts, env vars, PyInstaller, etc.
- **Autonomous iteration** — find bug → patch → rebuild → verify in one session
- **Documentation and specs** — project overviews, ship checklists, architecture notes tied to *my* codebase
- **Cross-project work** — Arden Desktop, Daily Bread, Second Brain, release paths, all in one workspace

### Composer is not

- My daily personal companion
- A privacy-first local chat window for non-technical use
- A product I hand to Brittany with an installer and desktop shortcut
- Voice-first or "sit on the couch and talk to the forest"

**Analogy:** Composer is the **shop floor** — welders, diagnostics, assembly line. Not the front porch.

---

## What Arden Desktop is and what it handles (the personal workstation)

**Arden** is a **shipped consumer product** — a forest-green Windows app, not a dev tool.

**Tagline:** *Keep the soul. Change the brain.*  
**Line:** Powered by Rémanence.

### What Arden does today (June 2026, real build)

| Capability | Detail |
|------------|--------|
| **Personal companion chat** | Named assistant (default Arden, user-renamable), warm consumer personality, streaming replies |
| **Swappable brains** | Same soul/memories; switch **Kobold** (local :5001), **Venice** (Llama 3.3 70B), **Groq** (backup) from a dropdown — no reinstall |
| **Local memory** | SQLite + hash embeddings; exchanges recalled into context; data under `%LOCALAPPDATA%\Arden\` |
| **Session persistence** | Sidebar with multiple named chats, survives restarts |
| **Onboarding + Settings** | First-run wizard, API keys, companion name, user name |
| **Consumer packaging** | Portable zip, `Install-Arden.ps1`, desktop shortcut, Brittany-ready path |
| **Automated QA** | `acceptance-test`, `diagnose-test`, `smoke-test` — headless verification without me clicking |
| **Optional research tab** | Open Notebook integration (Dave edition; not bundled in consumer portable) |
| **Voice hooks** | Mic + "Speak replies" (consumer defaults off; TTS optional) |

### What makes Arden different from a generic desktop AI

1. **Soul/brain split** — personality + memory stay; inference engine swaps per message.
2. **Built for a non-Dave user** — Brittany can unzip, install, paste a Venice key, never touch a terminal.
3. **Rémanence product identity** — forest sanctuary UI, sessions, "never leaves the forest" positioning.
4. **Tied to my product family** — separate from NURA Connect (facility), Daily Bread (scripture app), PersonaLock (deprecated).

### What Arden explicitly is not

- A coding agent (no repo access, no multi-file refactors)
- A slash-command agent OS (no `/task`, `/delegate`, agent marketplace)
- A cloud-only ChatGPT wrapper
- NotebookLM (no bundled podcast-from-sources in v1 consumer)

**Analogy:** Arden is the **front porch** — one window, one companion, your machine, your memories.

---

## How the two relate (so we don't double-count)

```
┌─────────────────────────────────────────────────────────────┐
│  CURSOR / COMPOSER     →  builds, fixes, ships Arden        │
│  ARDEN DESKTOP         →  what Dave/Brittany actually run   │
│  HERMES DESKTOP        →  ??? only if it fills a real gap   │
└─────────────────────────────────────────────────────────────┘
```

Composer **made** Arden work (Venice crash, UI lock, portable install, diagnose harness). Arden **is** the product. Hermes doesn't replace either unless it does something **outside** that boundary.

---

## What I need from you (revised question for the AI)

Given that I already have:

1. **Cursor Composer** for coding, debugging, and shipping
2. **Arden Desktop** for personal companion chat, local memory, swappable Venice/Kobold/Groq brains, and consumer install

**What does Hermes Desktop do that neither of those covers?**

Be specific. Don't repeat:

- "Personal AI you talk to" → **Arden**
- "Help you build software" → **Composer**
- "Remember context across sessions" → **Arden memory vault**
- "Use local models" → **Arden + Kobold**
- "Use cloud APIs" → **Arden + Venice/Groq**
- "Research / documents" → **Arden Notebooks tab (Open Notebook)** on Dave's build

I'm open to Hermes if it's genuinely the **execution/agent layer** (file ops, multi-step tasks, tool use, orchestration) — the "hands" in my stack — but not if it's just a third chat window with a different logo.

---

## One-liner for the argument

> Composer builds the car. Arden is the car I drive. Hermes needs to be the garage robot that does something I can't already do from the driver's seat or the factory — or it's redundant.

---

## What's likely left for Hermes (honest niche)

From the Second Brain / stack docs, Hermes was scoped as:

- **Execution / "hands"** — terminal tasks, file ops, agent-to-agent, slash-command power user stuff
- **Intent layer on top** — natural language instead of memorizing `/commands`
- **Not** the knowledge compiler (that's Second Brain / vault)
- **Not** the personal companion product (that's Arden)
- **Not** the IDE (that's Cursor)

So the honest remaining niche for Hermes Desktop is something like: **do tasks on my machine across apps and files, orchestrate agents, run workflows** — not **chat with me nicely**.

If the answer is still "Hermes is your generic personal AI," the reply is: *That's Arden. I already shipped it. Next answer.*
