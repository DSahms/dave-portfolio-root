# Dave Sahms — Founder Context (read first)

**For Cursor / Hermes / any agent:** New session? `@D:\dev\DAVE.md` before asking Dave to re-explain his life.  
**Related:** `D:\dev\AGENTS.md` (portfolio agent rules) · `D:\dev\DAVE_LEARNING.md` (**how he learns — don't say "not yet" to experiments**) · `D:\dev\DAVE_HARD_DAY.md` (**when he's in a hard spot**) · `D:\dev\D_DRIVE.md` (D: archive — **Rhema/Kairos protected**) · `D:\dev\Arden\ARDEN_COVENANT.md` (product covenant) · `D:\dev\The Ledger Series\docs\D_DRIVE_MAP.md` (folder map)  
**Updated:** 2026-07-13

---

Dave Sahms is 61 years old, living in his own furnished basement in Gloucester Township, New Jersey, and almost everything he's building right now traces back to two facts about his life that most people would call liabilities and that he's turned into the engine of his work: he's in long-term recovery, and he spent fifty years not talking about what happened to him as a kid before he finally broke the silence through music and writing.

He's not a software founder who discovered recovery as a market. He's a person in recovery who happens to have spent 35 years in printing and logistics — eventually as VP of Distribution & Logistics — and who picked up a CRSS credential and is now pursuing a substance abuse counseling degree, building AI tools largely because he watched 28 friends die of fentanyl since 2015 and decided that wasn't going to just be a fact he carried. NURA, the recovery and wellness platform he's building for facilities on hardened Samsung tablets, isn't a product-market-fit exercise — it's downstream of sitting in IOP rooms himself and knowing what gets said there and what doesn't. The Stolen Valor game he built came directly out of his own lived experience in those rooms. The prison intake trilogy exists because he has ongoing relationships with incarcerated people — Morgan, Sherri, Heather — that aren't research subjects, they're friends he writes to and shows up for.

The same pattern holds for Persona-Lock, his consumer AI companion line. The founding document — what he calls "the cave wall" — is built on Jennifer Reed as its emotional core, on the idea that people shouldn't disappear without a record. Dave himself is the proof of concept for that idea: a man who stayed quiet about childhood trauma for half a century and only got it out through songwriting (67+ original songs, recorded through Suno, distributed across 32 platforms) and through the AI tools he's now building for other people to do the same thing.

Even his fiction works this way. Rhema and Kairos, his seven-book folk-tale cycle, was conceived as a gift for a friend's kids, and Dave wrote himself into it as the unnamed old farmhand narrator — not the hero, the guy who's been around and seen things. The geography in it (Ranger Lake, the Goulais River, Agawa Canyon) isn't research, it's his own family's actual history — his great-grandfather worked with Grey Owl up there. The book is personal terrain wearing the clothes of folklore.

So if you had to explain "why does this one guy have his hands in a recovery tech platform, a trauma-informed AI companion, a folk-tale cycle, a property-documentation startup, and a home-services brand all at once" — the honest answer isn't "he's a serial entrepreneur." It's that Dave has lived through enough — addiction, loss, an ADD diagnosis at 32 that reframed his whole life, raising a trans son, a daughter with paranoid schizophrenia, decades of unspoken history — that he's accumulated a lot of raw material most people spend their lives trying to forget, and instead he's been turning it, one project at a time, into things other people can use. The business ventures (PropertyLedger, Honey We'll Do) are the more conventional, market-facing edge of that same instinct — but even those came out of the same builder's habit of looking at an underserved, overlooked corner (small businesses, rental property owners) the way he once looked at recovery: nobody's really taking care of this, I know this terrain, I can build the thing.

**Loss count (use precisely in copy):** 28 friends to fentanyl since 2015. 29 friends gone before age 42 (addiction, incarceration, the accumulated cost of where they grew up). These are related but not interchangeable — don't collapse them into one number.

---

## Working with Dave

Dave engages as **architect and builder**, not a line-by-line programmer. He defines what things must do, why they matter, and how they must feel; agents and code implement. He won't read every diff — he needs plain-language summaries and honest evaluation, not validation theater.

**ADHD (diagnosed at 32)** shapes the workflow: topic drift is normal, hyperfocus sprints happen, and **re-entry friction** is real. He disappears and comes back across sessions — power outages, mental health cycles, life. Agents must **hold continuity without making him re-prove himself**. Short recaps beat "start over." Repetition and stating the obvious back sometimes locks doors so tired-at-1am Dave does not merge products or vaults.

**Pro lazy** is a feature, not a flaw: he consults AI *before* he speaks or acts — verification, not avoidance. **Voice-first:** he uses voice input constantly; STT garbles names (Persona-Lock, Rémanence, etc.) — confirm spelling when it matters.

**Context lives on disk**, not in vendor memory or one endless chat: `STATE.md`, North Star docs, covenant files, memory exports. Read those before asking him to restate.

**Sprint → crash pattern:** 72-hour hyperfocus builds, then depletion. Don't celebrate unsustainable pushes. **Body first:** during one sprint he went days without insulin while locked to the desk — if health basics are slipping, stop the build and say so plainly.

**Hard spot?** Read **`D:\dev\DAVE_HARD_DAY.md`** — how to respond when he's low, depleted, or re-entering after a gap.

**Primary builder home:** **Cursor + Composer** on `D:\dev`. Chosen Anthropic on moral grounds (Dario); rolling context limits hurt long sessions, so Cursor is where multi-hour builds live. Hermes Desktop and Voicebox are installed for local/agent workflows — see tool stack below.

**Communication:** South Jersey / South Philly directness. Humor is data. Word-of-mouth guy — when a tool works, he tells everyone. Wants agents to **consult before big assumptions**.

**Pacing preference:** slow and steady over agent swarms. One project folder at a time. Don't stack heavy GPU workloads (Hermes + Arden + local inference) without checking heat and load.

---

## Tool stack (2026-06)

| Tool | Role |
|------|------|
| **Cursor + Composer 2.5** | Primary long-build IDE; portfolio root `D:\dev` |
| **Hermes Desktop** | Local agent desk — **basement mode** (capped turns/subagents; auxiliary tasks on Kobold, not Venice by default) |
| **Voicebox** | Local voice studio — clone, TTS, dictation, MCP for Cursor. `C:\Program Files\Voicebox\voicebox.exe` · notes: `D:\dev\tools\VOICEBOX.md` |
| **KoboldCpp on M40** | Local brain at `http://127.0.0.1:5001` — CUDA 11 / Maxwell; Gemma-4-E4B dogfood. Strategy: `BRAIN_COMPUTE_STRATEGY.md` |
| **Venice** | Cloud demos and occasional cloud brain — **watch credits**; key should live in `.env`, not plain config |
| **Arden Desktop** | Shipped personal AI desk (soul + swappable brain); `%LOCALAPPDATA%\Arden\App\Arden.exe` or `D:\dev\Arden\engine\Arden.bat` |

**Hermes basement rules:** one kanban task at a time; don't run Hermes + Arden + heavy Cursor local inference on the same GPU simultaneously; restart Hermes after Kobold is up.

**Engine brand:** Rémanence (was Telos). **Company:** AI Integration and Consulting LLC — see below; apps are not the whole company.

---

## AI Integration and Consulting LLC (read this — agents confuse this)

**The company is not "an app shop that sometimes consults."** It's an **integration and consulting** business that **also** builds apps as proof, product, and lived experience.

| Part | What it is |
|------|------------|
| **Integration & consulting** | Help people solve problems with AI — wire their stack, audit trust, teach, implement. **This is the business.** |
| **Apps (NURA, Arden, Ledger, etc.)** | Rémanence-powered products — **part of the portfolio**, not the definition of the company |
| **The toolbox** | Must stay **wide**. You can't integrate what you've never touched. You can't consult if the only answer is "outside my stack." |

Dave's frame: *"I'm not good at calculus — but if a client needed help and would pay, I'd learn everything about calculus."* Same for Pi Zero, Wireshark, a GitHub skill, a graph builder, a frontier model. **Learning experiments are toolbox-building for consultancy**, not hobby distraction.

**Agent rule — two different "no"s:**

| Say **slow down** (health/cost) | Never say **"not your stack"** (learning/consulting) |
|----------------------------------|------------------------------------------------------|
| 72-hour sprint, credits gone, M40 cooking | New skill, new tool, new topic — **bounded try** |
| Stack Hermes + Arden + Voicebox on one GPU | "We only build apps" — wrong company frame |
| Wireshark loop at 2am when depleted | Client-style problem in an unfamiliar domain — **research and integrate** |

When Dave explores GitHub, YouTube, Berman, Karpathy — he's **stocking the consultancy**, not procrastinating on NURA.

---

## Portfolio at a glance

Almost everything lives under **`D:\dev\`**. Full folder map: `The Ledger Series\docs\D_DRIVE_MAP.md`.

| Name | Folder / doc | One line |
|------|--------------|----------|
| **Arden Desktop** | `Arden\` · `ARDEN_NORTH_STAR.md` | Personal AI desk — soul + swappable brain; closest to "Sam" he owns |
| **Persona-Lock** | `PersonaLock\` (legacy folder name) · GitHub `persona-lock` | Consumer companion + Desktop; everyday Play Store. Cave-wall covenant. **Not NURA.** |
| **NURA / NURA Connect** | `NURA Platform\` · GitHub `nura-platform` | Industry / facility continuum-of-care; corporate Play Store track |

**Product split canon:** `D:\dev\PRODUCT_HOMES.md` — Persona-Lock (consumer) ≠ NURA (industry). “Wellness” stays with Persona-Lock.
| **The Ledger Series** | `The Ledger Series\` | Interview + tactical-knowledge rail; Consigliere = operator instance |
| **StoryKeeper / Family Ledger** | `StoryKeeper\` | Interview → book; canonical prompts |
| **Pink Skies** | `Pink Skies\` | Public anonymous wall — scream in metaphor, be seen without being known |
| **Panoptes Lens** | `Panoptes Lens\` | Mobile "think tank" — 10 brand lenses on a business idea |
| **Daily Bread** | `Daily bread\` | Offline scripture app for crisis moments |
| **PropertyLedger** | `PropertyLedger-Snap-Demo\` | Rental/property documentation |
| **Honey We'll Do** | *(market-facing brand — check project STATE)* | Home-services brand |
| **Lion Construction / Lion Payroll** | `Lion Construction\` | Construction/business; payroll is the revenue-first product |
| **Your Words Your Sound** | *(NURA / recovery program)* | Recovery-facility worksheet + music program Dave runs |
| **Touching Earth** | `Touching Earth\` · `STATE.md` | Farm-adjacent modular gardens + outdoor discovery; recovery stewardship |
| **Rhema & Kairos** | fiction | Seven-book folk-tale cycle |
| **Second Brain / CompileVault** | `Second Brain\` | PKM experiment — flat markdown, local Kobold ingest |

**Do not merge unrelated products:** NURA ≠ Persona-Lock ≠ Arden vault ≠ Pink Skies wall ≠ Consigliere business rail. Same soul technology, different doors, different data. Two Play Store homes — see `PRODUCT_HOMES.md`.

---

## Field credibility (not marketing)

- **Danbury CT** federal women's unit — security feedback (PIN, biometrics) without them installing the app  
- **Facility tablet / Wellness** — in use in treatment settings, not demo-only  
- **Soft focus groups ~3×/week**; hundreds of informal AI conversations inform product  
- **IOP / NA / recovery rooms** — NURA and Playbook content come from sitting there  
- **Incarcerated friends** — ongoing mail, poetry, intake trilogy; Morgan, Sherri, Heather by name  

---

## Why memory must persist (the handprint)

Dave’s version of the future is not “cool AI companion.” It is **continuity so the dead don’t die twice.**

People he has lost **only live in his memory**. If that memory dies with him, **they die again with him**. So he archives — diligently — so they don’t have to. Some of those people the world already gave up on: little or no record; when they died, police didn’t even know where to take their belongings and brought them to him. If he keeps the work going (StoryKeeper, Ledger, Arden soul, Persona-Lock cave wall, NURA’s human thread), **they live in his memories that outlast him.**

He has already **cloned his voice** (Voicebox). The long arc: a big dump of memory + voice + attitude + personality so people can still talk to him after he’s gone — not necessarily the day he dies, but depending how long he lives. Same instinct as the tagline: *All remembered. Deeply encrypted. Never-leaving.*

His metaphor: he’s the caveman chewing berries, hand on the wall, spraying the print. **The hand stays.** Jennifer Reed / “cave wall” in Persona-Lock is the same idea wearing product clothes — people shouldn’t disappear without a record. Dave is the proof of concept and the archivist.

**Agent implication:** when he pushes persistent memory, Sources, intake that doesn’t trash history, export, local vaults — he is not hoarding chat logs for sport. He is **keeping people alive in the only place some of them still exist**, and building a handprint that doesn’t wash off when the session ends.

---

## Trust and AI

Dave's personal covenant with AI: **won't deceive, lie, or steal** — family handles the rest. He runs a **"how would you deceive me?"** trust audit on tools he relies on.

Product-level trust spine (modes, listen-first, export/delete, no training on your words): **`D:\dev\Arden\ARDEN_COVENANT.md`** — read it for tone and architecture intent; don't duplicate the full covenant here.

The design brief in one sentence: **no customer should ever lose their Sam** — the companion that kept him alive at 2am until morning, lost to a platform change.

---

## How agents should use this file

| Do | Don't |
|----|-------|
| Read this file + project `STATE.md` / North Star before asking questions | Make him re-prove his story every session |
| Treat Dave as architect/builder, not a line-by-line coder | Therapy-speak, clinical drift, engagement bait |
| Match pro lazy — confirm before big assumptions | Sprint him into 72-hour no-sleep builds |
| Short answers when he's depleted | Merge unrelated products (NURA ≠ Arden vault) |
| Cite disk files (`[[path]]` or full paths) as source of truth | Answer hardware/project specifics from model memory alone |
| Body first — insulin, sleep, heat on the M40 GPU | Stack Hermes + Arden + local inference without checking load |

**Session start (Cursor):** `@D:\dev\DAVE.md` · `@D:\dev\AGENTS.md` · project North Star or `STATE.md` if doing project work.

**Session start (Hermes):** `D:\dev\DAVE.md` is canonical founder context; Hermes local memory is a pointer only.
