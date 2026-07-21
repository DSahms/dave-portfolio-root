# Brain & compute strategy (locked 2026-07-14)

**Purpose:** Keep **models / cards / cloud routing** from getting mixed into product identity (NURA ≠ Persona-Lock ≠ Arden).  
**Products:** `PRODUCT_HOMES.md`. **Stack roles:** this file + `STACK_CURSOR_ARDEN_HERMES.md`.

---

## Roles (do not marry)

| Piece | Job | Where it runs |
|-------|-----|----------------|
| **Arden** | Default **product** people use — companion, soul, memory, brain dropdown | Their machine (local app) |
| **Hermes** | Agent / hands — multi-step tools, execution | **Self-hosted in the cloud** (access from anywhere). Not on Dave’s M40 desk by default |
| **Cursor / Composer** | Dave’s builder only | Dave’s workstation. Never part of the consumer story |

Arden is unfinished — finish Arden before treating Hermes-cloud as the main build. Cursor stays a different animal: don’t “integrate Cursor into Arden.”

---

## Local brain thesis (Gemma-first)

**Proven local model:** Gemma-4-E4B-it (QAT UD Q4_K_XL) on KoboldCpp — fast, multimodal with projectors, good enough to **trust**.

**Product philosophy (why this matters):**

- VRAM and cloud compute are expensive.
- People won’t try AI if the entry fee is a $1000+ GPU.
- Ship a path that works on **cheaper cards** and **edge** (Jetson-class devices).
- Build trust by proving **local works** — then escalate when the job is too heavy.

```
  User ask
     │
     ▼
  Local Gemma (Kobold)  ── light / medium work
     │
     │  triggers: complexity, latency budget, token/context pressure,
     │            tool-storm, “need a bigger brain”
     ▼
  Venice (cloud)        ── heavy lift only
```

This is **not** “replace Venice for Brittany tomorrow.” Consumer Arden can still default Venice until local packaging is ready. The **architecture direction** is: local-first for the cheap/edge story; cloud as overflow.

---

## What to optimize (effectiveness, not thinner quants)

Give Gemma everything that makes it *better at its job*:

1. Correct Kobold flags (`--jinja`, `--jinjatools`) — Gemma 4 is format-sensitive  
2. Matching mmproj (vision/audio)  
3. Context headroom on the card (prefer longer context over bigger model on 8–24GB class)  
4. Few sharp MCP tools + short skills (not a Claude-sized tool zoo)  
5. Clear handoff rules to Venice when local shouldn’t carry the load  

Do **not** confuse this with:

- Renaming NURA / Persona-Lock  
- Merging Cursor into the product  
- Parking Hermes on the M40 so Arden fights for VRAM  

---

## Hardware story (customer trust)

| Tier | Idea |
|------|------|
| **Edge / budget** | Cheap NVIDIA / Jetson-class — Gemma-class local brain |
| **Dave / power user** | M40 24GB lab — same architecture, more context/tools |
| **Overflow** | Venice when local shouldn’t lift alone |

Proof → trust → then sell. Not “buy a 4090 or you can’t play.”

---

## Agent rules

1. Talking **models / VRAM / Jetson / Kobold / Venice routing** → this file. Don’t invent product merges.  
2. Talking **Arden features / Brittany ship** → `Arden\ARDEN_NORTH_STAR.md` (Venice may still be consumer default until local path ships).  
3. Talking **Hermes** → agent layer, prefer **off-box / cloud self-host** plan; don’t assume it sits on the M40.  
4. Talking **Cursor** → Dave-only builder. Not a product dependency.  
5. Arden not done → don’t divert the critical path into Hermes cloud build unless Dave names that sprint.
