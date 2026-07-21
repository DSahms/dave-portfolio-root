# D: Drive Recovery Inventory
**Date:** 2026-07-21  
**Source of structure:** Windows File Recovery (filenames + folders)  
**Source of content:** Cursor local history + GitHub clones (where available)

## Outside `dev` — status

| Path | Files | Intact | Zeroed | Status | Notes |
|---|---:|---:|---:|---|---|
| Air BNB Ledger | 28 | 20 | 8 | MOSTLY INTACT | Cursor history restored key docs |
| Beta Apps | 466 | 95 | 371 | MOSTLY ZEROED | APK builds/backups mostly lost |
| DCS benchmark | 19 | 19 | 0 | ALL INTACT | Cursor history |
| Documents | 4 | 2 | 2 | MIXED | |
| Lessons | 119 | 0 | 119 | ALL ZEROED | Manuscript + docs — local only |
| Misc | 57 | 26 | 31 | MIXED | |
| Miscellaneous | 1 | 0 | 1 | ZEROED | LLM eval report docx |
| Morgan_Voice | 10 | 0 | 10 | ALL ZEROED | Morgan Freeman TTS mp3s |
| NURA system test | 154 | 67 | 85 | MIXED | Cursor build remnants |
| Rhema and Kairos | 5 | 5 | 0 | ALL INTACT | Small restored set |
| suno text files | 444 | 0 | 444 | ALL ZEROED | Lyrics — re-export from Suno |
| Suno Waves | 229 | 0 | 229 | ALL ZEROED | ~8.2 GB WAV masters — re-download from Suno |
| Takeout | 1 | 1 | 0 | INTACT | |
| Test two | 4 | 2 | 2 | MIXED | |
| THE TALE OF RHEMA AND KAIROS | 71 | 0 | 71 | ALL ZEROED | Use GitHub `rhema-and-kairos` + re-download WAVs |
| Root loose files (screenshots, stack md, etc.) | 8 | 0 | 8 | ALL ZEROED | |

## Inside `dev`

| | Count |
|---|---:|
| Files present | 7130 |
| Intact content | 4761 |
| Zeroed shells | 2369 |
| Intact MB | ~32 MB of real content (plus GitHub clones in `_github_restore`) |

## Recoverable elsewhere (not lost)

- **GitHub clones:** `D:\dev\_github_restore\` — arden, persona-lock, the-ledger-series, storykeeper, property-ledger, pink-skies, refactor-room, rhema-and-kairos, nura-platform, dcs-evaluation, personal-knowledge-corpus
- **F: NURA Codex workspace** — untouched
- **Suno / 32 distribution platforms** — song audio + lyrics can be re-exported
- **Cursor history** — 505 files already restored with content

## Highest-priority local-only losses (outside GitHub)

1. `D:\Suno Waves\` — full WAV masters (~8 GB) — re-download from Suno
2. `D:\suno text files\` — 444 lyric .txt exports — re-export from Suno
3. `D:\THE TALE OF RHEMA AND KAIROS\` — local DOCX/PDF/WAV not on GitHub — check GitHub first, then rebuild
4. `D:\Lessons\` — manuscript + revision docs
5. `D:\Morgan_Voice\` — 10 custom TTS clips
6. `D:\Miscellaneous\LLM_Eval_Suite_Phase1_Report.docx`
7. Founder docs still zeroed: `DAVE_HARD_DAY.md`, `DAVE_LEARNING.md`, `D_DRIVE.md` — rebuild from chat transcripts next

