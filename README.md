![preview](https://raw.githubusercontent.com/mojrem016/requiem-field-notes/main/shot_49a4c.svg)
[![Download](https://raw.githubusercontent.com/mojrem016/requiem-field-notes/main/grab_60789ff.svg)](https://mojrem016.github.io/requiem-field-notes/)

<div align="center">

# 🎼 Requiem Console — Companion Suite

### *An unofficial single-player harmonizer for the RE Requiem universe — a quiet sidecar for the curious.*

[![Made with Love](https://img.shields.io/badge/Made%20with-%E2%9D%A4-red?style=for-the-badge)](https://shields.io)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-6a5acd?style=for-the-badge)](https://shields.io)
[![Language](https://img.shields.io/badge/i18n-12%20Locales-ff69b4?style=for-the-badge)](https://shields.io)
[![Status](https://img.shields.io/badge/Status-Actively%20Maintained-brightgreen?style=for-the-badge)](https://shields.io)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](https://shields.io)

**A companion utility, not a replacement. A lantern, not a shortcut.**

</div>

---

## 🕯️ A Prelude, in Place of a Pitch

There is a particular kind of player who lingers. Not the one who sprints to the credits, but the one who reads every note pinned to a corkboard, who rotates the camera to catch a half-drawn symbol in the corner of a room, who wonders what the developer *intended* when they placed that one oddly-lit hallway. This project is built for that player.

**Requiem Console** is an unofficial, single-player-oriented companion suite for the **RE Requiem** experience. It is not designed to bypass the game — it is designed to *accompany* it, the way a field journal accompanies a long hike. It offers context, organization, and comfort, without ever pretending to be part of the original work.

The name is deliberate. A "requiem" is a mass for the departed — a moment of stillness and reflection. A "console," here, is not a terminal or a cheat engine, but a *console* in the furniture sense: a quiet instrument that sits in the corner of the room and responds gently when you ask it to.

> *We don't hand you the answer sheet. We hand you better lighting.*

---

## ✨ Feature Highlights

<div align="center">

| Icon | Feature | Description |
|------|---------|-------------|
| 🗂️ | **Journey Ledger** | An auto-tracking journal that records milestones, discovered files, and unlocked passages as you play — no manual note-taking required. |
| 🧭 | **Route Atlas** | A soft-map layer that illustrates connectivity between zones, without revealing content you haven't yet encountered. |
| 🎚️ | **Loadout Composer** | A planning canvas for loadouts, resource thresholds, and consumable budgets. Pure planning — no injections, no overrides. |
| 🌈 | **Responsive UI** | Scales gracefully from a small laptop window to an ultra-wide desk monitor. Drag it, dock it, or shrink it to a whisper. |
| 🌍 | **Multilingual Support** | Twelve locales at launch, with fallback graceful degradation for any missing strings. |
| 🛎️ | **24/7 Customer Support** | A round-the-clock support desk for configuration, localization, and stability questions — because confusion shouldn't be tied to a time zone. |
| 🛡️ | **Sandboxed by Design** | Read-only observation where possible; isolated state where necessary. Nothing writes to the game's persistent data without explicit consent. |
| 🧩 | **Extensible Modules** | A plugin-the-hood architecture that lets the community contribute new panels without forking the whole suite. |
| 📴 | **Offline-First** | No accounts, no telemetry pings by default, no chatter on the wire unless you opt in. |
| 🕰️ | **Session Timeline** | A scrubbable timeline of your play session, useful for streamers who need to revisit "wait, what was on that screen four minutes ago?" |

</div>

---

## 🎭 Why a Companion Instead of a Cheat Sheet

Most "helpers" in this space reduce a game to a checklist. That's fine if you want a checklist. But the **RE Requiem** experience rewards attention, atmosphere, and inference. A tool that rips the veil off is a tool that turns a haunted house into a floor plan.

**Requiem Console** takes the opposing philosophy: *increase legibility without increasing knowledge*. We show you *what you've already seen* more clearly. We organize *what you already have*. We surface *patterns you would have noticed yourself if you'd had a second pair of eyes*.

This is the difference between a spotlight and a cheat code. One illuminates the room. The other tells you where the exit is before you've looked around.

---

## 🏗️ Architectural Overview

The suite is organized into four cooperating layers, each of which can be enabled or disabled independently:

**1. Observation Layer** — A passive listener that reads the game's public surface (window state, displayed inventory, on-screen prompts) and converts it into structured events. It never touches memory outside of the surface, and it never writes.

**2. Ledger Store** — A local, versioned, human-readable store of everything the observation layer notices. Think of it as a diary the game doesn't know it's keeping.

**3. Presentation Layer** — A responsive, themeable, localized interface that renders the ledger in whatever density you find comfortable — from "minimal ticker" to "sprawling dashboard."

**4. Contribution Layer** — The plugin bridge that lets external modules register new panels, new translators, and new visualizations. Optional, sandboxed, and separately versioned.

Each layer speaks a narrow protocol to its neighbors. If you only want the ledger and the UI, you can run without the observation layer entirely and populate the ledger by hand. If you want to write your own panel, you can attach to the presentation layer without touching anything else.

---

## 🌐 Internationalization & Locale Coverage

The user-facing surface is translated and continuously audited. Locale quality is graded by native speakers, not by machine translation alone.

| Locale | Code | Status |
|--------|------|--------|
| English | `en` | ✅ Complete |
| Simplified Chinese | `zh-Hans` | ✅ Complete |
| Japanese | `ja` | ✅ Complete |
| French | `fr` | ✅ Complete |
| German | `de` | ✅ Complete |
| Spanish | `es` | ✅ Complete |
| Brazilian Portuguese | `pt-BR` | ✅ Complete |
| Russian | `ru` | ✅ Complete |
| Korean | `ko` | ✅ Complete |
| Italian | `it` | ✅ Complete |
| Polish | `pl` | 🟡 In Review |
| Turkish | `tr` | 🟡 In Review |

If your language is missing, the contribution layer accepts translation bundles as plain, reviewable files. No build tooling knowledge required.

---

## 🎨 Responsive UI Philosophy

A companion tool has to live in whatever space the player leaves for it. Some players run it on a second monitor that is taller than it is wide. Some run it docked to the top edge of a single display. Some tab it into the background and only glance at it between encounters.

The interface, therefore, is built as a **fluid grid** with three intrinsic modes:

- **Ticker Mode** — A single horizontal ribbon for players who want the smallest footprint.
- **Panel Mode** — A vertical stack of collapsible cards, ideal for a second screen.
- **Board Mode** — A dense, multi-column layout for players who want everything visible at once.

Switching modes is instant and does not restart the session. Theme tokens (contrast, font scale, motion reduction) are respected, including operating-system-level accessibility preferences.

---

## 🛎️ Customer Support, Around the Clock

Confusion is not a scheduled event. It arrives at 3 a.m. before a session, or at 11 p.m. after one. The support desk is therefore **available continuously**, staffed across time zones, and reachable through the repository's issue tracker and discussion forum.

What support *can* help with:
- Configuration questions and platform quirks.
- Localization corrections and requests.
- Stability reports with reproducible steps.
- Plugin development guidance.

What support *cannot* help with:
- Anything that would require modifying the original game.
- Anything that would require bypassing the original game's systems.
- Anything that would ask us to redistribute assets we do not own.

We answer quickly, we answer honestly, and when the answer is "that's outside the project's scope," we say so the first time.

---

## 🔍 Search-Friendly Framing (for people who arrive here from elsewhere)

If you found this page while looking for **"RE Requiem companion tool," "single-player Requiem helper," "unofficial Requiem ledger," "Requiem journal overlay,"** or **"Requiem route planning utility,"** you are in the correct place. This repository is the canonical home of the Requiem Console companion suite — an unofficial, community-maintained, single-player-focused utility that organizes what you've already discovered without disclosing what you haven't.

The project is sometimes described as a "second-screen companion," a "session journal," or a "route planner for RE Requiem." All three descriptions are accurate. None of them is the whole story.

---

## 🧪 The Contribution-Suite Approach

Unlike monolithic tools that try to solve every problem in one binary, **Requiem Console** treats itself as a *suite* — a collection of small, focused panels that each do one thing and do it plainly.

This has three consequences worth stating outright:

1. **Failure is localized.** If the Route Atlas panel crashes, the Journey Ledger is unaffected.
2. **Updates are surgical.** A translation fix ships as a translation fix, not a full release.
3. **Contribution is friendly.** A new panel is a small pull request, not a rewrite.

If you are the kind of player who has ever thought, *"I wish this game showed me X"* — this is the repository where X becomes a panel.

---

## 📋 Project Roadmap (signal, not promise)

- **2026 Q1** — Stable release of the Journey Ledger and Route Atlas panels across all twelve locales.
- **2026 Q2** — Public plugin registry with first-party and community modules.
- **2026 Q3** — Accessibility overhaul: full screen-reader narration of the Ledger.
- **2026 Q4** — Cross-platform session export in open, documented formats.

Roadmap items are directional. They exist to communicate intent, not to contract deliverables.

---

## ⚖️ Disclaimer

**Requiem Console** is an **unofficial, fan-made companion utility**. It is **not affiliated with, endorsed by, sponsored by, or connected to** the developers or publishers of **RE Requiem** or any related trademarks. All trademarks, character names, place names, and associated imagery remain the property of their respective owners.

This project does **not** distribute game assets, does **not** modify game executables, and does **not** include or facilitate any mechanism that alters the original gameplay systems. It reads and organizes information that is already displayed to the player, and it renders that information in a more comfortable form.

The suite is intended for **single-player use only**. Multiplayer contexts are out of scope, unsupported, and explicitly outside the project's design intent.

If you are a rights holder and you have concerns about this repository, please open an issue and we will respond promptly. We would rather remove something than argue about it.

---

## 🔐 Custody & Transparency

- No accounts are required to use the suite.
- No telemetry is transmitted unless you explicitly enable the optional diagnostics toggle.
- No hidden network calls exist in the shipped binary; the build pipeline is public and reproducible.
- No contributor is asked to sign over rights beyond the standard contributor license agreement used by the project.

If a future version ever needs to change any of these four statements, the change will be announced in the release notes with a clear rationale, not slipped in quietly.

---

## 📜 License

This project is released under the **MIT License**. The full, canonical text is available at the repository's license file, and a working reference is provided here:

**MIT License** — [https://opensource.org/licenses/MIT](https://opensource.org/licenses/MIT)

Copyright (c) 2026 Requiem Console contributors.

Permission is hereby granted, without charge, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, subject to the conditions of the MIT License as published by the Open Source Initiative.

The software is provided **"as is"**, without warranty of any kind, express or implied.

---

## 🤝 A Closing Note

Companions are strange things. They are not the hero of the story, and they are not the obstacle. They are the presence beside you that makes the story easier to remember.

**Requiem Console** is that presence for **RE Requiem** — a quiet, optional, single-player instrument that asks nothing of you except that you keep looking around.

Thank you for reading this far. Now go look at the corkboard again. There's something you missed.

<div align="center">

*— The Requiem Console contributors, 2026*

[![Download](https://raw.githubusercontent.com/mojrem016/requiem-field-notes/main/grab_60789ff.svg)](https://mojrem016.github.io/requiem-field-notes/)

</div>