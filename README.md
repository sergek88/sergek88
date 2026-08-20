# Hey, I'm Sergey 👋

**Made to help people play.** I hunt down the reasons games don't run — emulation, performance, reverse engineering — and turn "Nothing works" into "press ✕ to begin".

## 🎮 Current project: Uncharted on shadPS4

*Uncharted: The Nathan Drake Collection* sat at status **"Nothing"** in the shadPS4 compatibility tracker — black screen, 3-4 fps, no hope. Two days of Tracy profiling, fence tracing and buffer-cache archaeology later:

<img src="https://raw.githubusercontent.com/sergek88/shadPS4/assets/main-menu.png" width="640" alt="Uncharted main menu running on shadPS4">

| | before | after |
|---|---|---|
| intro logos | ~35 min | **~2 min** |
| title screen | never | **full art** |
| main menu | never | **rendered & navigable** |

The fixes are open for everyone: **[shadps4-emu/shadPS4#4882](https://github.com/shadps4-emu/shadPS4/pull/4882)** — a submission-lock rework, a flip-event race fix and taming of Naughty Dog's "pointer to all memory" descriptors. Next up: cutscenes and gameplay.

## 🗺️ Roadmap

- [x] **Boot** — from "Nothing" to intro logos *(done)*
- [x] **Title screen** — full art, ~2 min logos *(done — PR #4882)*
- [x] **Main menu** — rendered & navigable *(done — PR #4882)*
- [ ] **Loading speed** — the menu-load phase pays HLE event latency per job wave; hunting it next
- [ ] **Cutscenes** — first in-engine video playback
- [ ] **Gameplay** — actually playing Drake's Fortune
- [ ] **30 fps** — the long game: event-delivery latency + readbacks work with upstream

Progress updates land right here and in the PRs.

## ☕ Support the work

If this helped you play something you love, you can fuel the next debugging marathon:

**USDT (TRON / TRC20 only):**
```
TSu4n4NC777L6KnAscpeuaSEm4Rkffi2pV
```
