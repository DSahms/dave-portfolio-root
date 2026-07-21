# D:\dev — Portfolio Agent Briefing

Read at the start of any session unless Dave names a single project folder explicitly.

**Founder context (always):** `D:\dev\DAVE.md`  
**When Dave is in a hard spot:** `D:\dev\DAVE_HARD_DAY.md`  
**D: drive protected folders:** `D:\dev\D_DRIVE.md` — **never delete** `THE TALE OF RHEMA AND KAIROS` or `Rhema and Kairos`  
**Folder map:** `D:\dev\The Ledger Series\docs\D_DRIVE_MAP.md`  
**Product covenant (tone + trust):** `D:\dev\Arden\ARDEN_COVENANT.md`

---

## What this workspace is

`D:\dev` is Dave Sahms's primary development root — **AI Integration and Consulting LLC** on a 1TB drive.

**Company ≠ apps only.** Integration and consulting are the business; Rémanence apps (NURA, Arden, Ledger, etc.) are **part of the portfolio** — proof, product, and lived experience. Dave builds a **wide toolbox** to integrate and advise; agents must not answer "outside my stack" when he's learning a tool, skill, or domain for consultancy.

Dave is **architect/builder**, not a line-by-line coder. Implement; summarize in plain language; consult before big assumptions.

---

## Session start checklist

1. Read `DAVE.md` if you don't already have founder context.
2. Confirm **which folder** Dave is working in — default is not automatic; ask if unclear.
3. Read that project's **North Star**, `STATE.md`, or `AGENTS.md` if present.
4. Do **not** merge products (NURA ≠ Persona-Lock ≠ Arden Desktop ≠ Pink Skies ≠ Consigliere business rail).  
   **Two Play Store homes:** Persona-Lock = consumer; NURA = industry. Canon: `D:\dev\PRODUCT_HOMES.md`.

---

## Where truth lives

| Layer | File(s) |
|-------|---------|
| Who Dave is | `D:\dev\DAVE.md` |
| Folder → product map | `The Ledger Series\docs\D_DRIVE_MAP.md` |
| Per-project task truth | `STATE.md`, `*_NORTH_STAR.md`, project `AGENTS.md` |
| Claude handoff exports | `*_CLAUDE_MEMORY_EXPORT.md` per folder |
| Export workflow template | `D:\dev\CLAUDE_MEMORY_EXPORT.md` |
| Arden product soul | `Arden\ARDEN_COVENANT.md`, `Arden\ARDEN_NORTH_STAR.md` |

**Vendor chat memory is not canonical.** If a fact matters, it should be on disk — or Dave re-explains once and you write it down.

---

## Working rules

- **Re-entry friendly:** Dave steps away and returns. Short recap > making him restate his life.
- **Pro lazy:** He uses AI to verify before he acts. Confirm spelling of product names (voice input garbles them).
- **Slow and steady:** One project folder at a time. No agent swarms unless Dave asks.
- **Body first:** Don't push through depletion, heat on the M40, or skipped health basics.
- **Honest evaluation:** Tell him what's wrong; skip validation theater.
- **Local-first default:** Kobold at `:5001` for local inference; Venice/cloud costs credits — flag bleed.
- **GPU discipline:** Don't stack Hermes + Arden + heavy local inference without checking load and thermals.
- **Brain / compute / Hermes-cloud plan:** `D:\dev\BRAIN_COMPUTE_STRATEGY.md` — Arden = default product; Hermes = off-box agent; Cursor = Dave-only; Gemma-first + Venice overflow. Don't mix model talk into product merges.

---

## Key projects (quick point)

| Project | Open this | Notes |
|---------|-----------|-------|
| **Arden Desktop** | `Arden\` · `ARDEN_NORTH_STAR.md` | Shipped consumer desk; Kobold + Venice brain switch |
| **The Ledger Series** | `The Ledger Series\` · `STATE.md` | Interview engine; Consigliere = operator |
| **NURA Platform** | `NURA Platform\` · GitHub `nura-platform` | Industry / facility line; corporate Play Store track |
| **Persona-Lock** | `PersonaLock\` · GitHub `persona-lock` | Consumer companion + Desktop; everyday Play Store track. Not NURA. |
| **StoryKeeper** | `StoryKeeper\` · `STATE.md` | Canonical interview prompts |
| **Pink Skies** | `Pink Skies\` | Anonymous public wall |
| **Panoptes Lens** | `Panoptes Lens\` · `AGENTS.md` | Flutter + Claude pipeline |

Per-project `AGENTS.md` overrides this file for repo-specific layout and commands.

---

## Git and commits

- **Do not commit or push** unless Dave explicitly asks.
- When he does ask: follow repo commit message style; never commit secrets (`.env`, API keys).
- Dave is learning git/PR workflow — explain terms when needed, don't assume fluency.

---

## Naming traps

| On disk / voice garble | Canonical name |
|------------------------|----------------|
| `PersonalLock\` / `PersonaLock\` | **Persona-Lock** (hyphenated) — **consumer**, not NURA |
| `personalock_wellness` / “Personal Lock Wellness” | **Persona-Lock** consumer mobile lineage — **not** “old NURA Connect” |
| NURA / NURA Connect | **Industry** facility line only — GitHub `nura-platform` |
| `Daily bread\` | **The Daily Bread** |
| Rémanence | Engine brand (was Telos) |

**Do not** say Wellness “became” NURA. Shared code history ≠ shared product. See `PRODUCT_HOMES.md`.

---

## Hermes + Cursor together

- **Cursor** = long builds, Composer, portfolio edits.
- **Hermes** = local agent desk; basement-mode config caps turns and routes auxiliary work to Kobold.
- Both should `@` or read **`DAVE.md`** — Hermes `MEMORY.md` points there, not a duplicate biography.
