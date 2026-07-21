# Product homes — do not merge

**Locked:** 2026-07-14  
**Why:** “PersonaLock Wellness” naming kept collapsing into NURA. They are **two products**, two Play Store homes.

---

## The line

| | **Persona-Lock** | **NURA / NURA Connect** |
|---|---|---|
| **Audience** | Everyday consumer | Industry / facilities / corporate programs |
| **Play Store home** | Consumer listing | Corporate / enterprise-style listing (facility download) |
| **Brand family** | Anything **Persona** / **Personal Lock** / **Persona-Lock Wellness** | **NURA** and **NURA Connect** only |
| **Disk home** | `D:\dev\PersonaLock\` | `D:\dev\NURA Platform\` · Connect app: `NURA Platform\nura-connect\` |
| **GitHub home** | `DSahms/persona-lock` | `DSahms/nura-platform` |
| **What it is** | Standalone companion + Desktop Edition (cave wall, consumer soul) | Continuum-of-care platform + companion that travels with the person in care |

**Rule for agents:** Never treat Persona-Lock (or Wellness) as “the old name for NURA Connect.” NURA did **not** eat Persona-Lock. Shared code history is fine; shared **identity** is not.

---

## Legacy naming (dead brands vs live brands)

| Old / on-disk string | Belongs to | Notes |
|---|---|---|
| `PersonaLock\` folder | **Persona-Lock** | Folder spelling ≠ product spelling |
| `personalock_wellness` | **LEGACY path** | Old nest under PersonaLock; **canonical NURA Connect is** `NURA Platform\nura-connect\` |
| “Personal Lock Wellness” / “PersonaLock Wellness” | **Persona-Lock** | Consumer product family — **not** NURA |
| NURA Connect | **NURA** | Industry companion; disk `NURA Platform\nura-connect\`; GitHub `nura-platform` |
| `Persona-lock-Wellness` (old GitHub repo) | **ARCHIVE** | Legacy dump; do not develop there |

---

## Play Store (target)

1. **Consumer** — Persona-Lock (and Persona-Lock Wellness face if used): everyday download.  
2. **Industry** — NURA Connect under the NURA platform line: facility / corporate download track.

Same company (AI Integration and Consulting LLC). Same engine brand available (**Rémanence**) where it earns its keep. **Two store homes. Two product IDs. Two repos.**

---

## Code lineage (honest)

Flutter work under `PersonaLock\personalock_wellness\` was partly re-skinned toward NURA Connect for facility demos. That was unfinished product-splitting — **not** permission to erase Persona-Lock.

Correct end-state:

- **Persona-Lock mobile / Desktop** = consumer app (Persona branding, consumer Play Store) under `PersonaLock\`
- **NURA Connect** = industry app at `NURA Platform\nura-connect\` (facility signals, corporate listing)

Flutter work formerly under `PersonaLock\personalock_wellness\` **moved** to `NURA Platform\nura-connect\` (see `MOVED.md` at the old path). They may share ancestry. They must **diverge** as products (package name, icon, store listing, copy).

---

## Agent checklist

1. Working on recovery **facility / tablet / Maryville / island / corporate?** → NURA only (`NURA Platform\`, `nura-platform`).  
2. Working on **consumer companion / cave wall / Desktop Edition / Wellness / $10/mo line?** → Persona-Lock only (`PersonaLock\`, `persona-lock`).  
3. If unsure — **ask**. Do not “helpfully” rename Persona → NURA or NURA → Persona.
