# 🎮 DOTASTATS

> Real-time Dota 2 statistics dashboard — hero winrates, player profiles, meta trends and more.

![License](https://img.shields.io/badge/license-MIT-orange) ![Status](https://img.shields.io/badge/status-in%20development-yellow) ![API](https://img.shields.io/badge/API-OpenDota-red)

---

## 🔥 What is this?

**DOTASTATS** is a clean, fast, dark-themed statistics dashboard for Dota 2 built with pure Vanilla JS — no frameworks, no bloat. Just real data from the OpenDota API rendered beautifully.

Plug in any Steam ID and instantly get a full breakdown of a player's performance, their best heroes, recent match history, and how the current meta looks patch by patch. Built as a portfolio project, designed to look and feel like something you'd actually want to use.

---

## ✨ Features

- 🔍 **Player Search** — look up any player by Steam ID, see their rank, MMR estimate, and overall win/loss record
- 🧙 **Hero Stats** — top heroes ranked by winrate and pick rate, with S/A/B/C tier badges
- ⚔️ **Radiant vs Dire** — animated side winrate chart with a smooth left-to-right curtain transition when switching sides
- 🕹️ **Recent Matches** — color-coded win/loss feed with KDA, duration, hero, and MMR delta
- 📊 **Role Distribution** — pick rate breakdown across all 5 roles (Carry, Mid, Offlane, Soft Supp, Hard Supp)
- 🌍 **Meta Snapshot** — avg game length, first blood time, Roshan kills per game, tower damage average
- ⚡ **No API key needed** — powered by the free OpenDota public API

---

## 🛠️ Tech Stack

| Layer | Tech |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 + Custom Properties |
| Logic | Vanilla JS (ES Modules) |
| Data | [OpenDota REST API](https://docs.opendota.com) |
| Dev server | Live Server (VS Code) |

---

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/yourusername/dotastats.git
cd dotastats
```

Then just open `index.html` with **Live Server** in VS Code and you're good to go. No installs, no build step.

---

## 📁 Project Structure

```
dotastats/
├── index.html          # main page
├── style.css           # all styles, CSS variables, animations
└── src/
    ├── main.js         # entry point, page logic, event listeners
    ├── api.js          # all OpenDota API calls
    ├── ui.js           # DOM rendering functions
    └── utils.js        # KDA calc, time formatting, Steam ID conversion
```

---

## 🗺️ Roadmap

- [x] Project structure & design system
- [ ] Player search by Steam ID
- [ ] Hero winrate table with sorting (Win % / Pick %)
- [ ] Radiant / Dire winrate chart with animated curtain transition
- [ ] Recent matches feed
- [ ] Role distribution bar chart
- [ ] Meta snapshot panel
- [ ] Mobile responsive layout

---

## 📡 API Reference

All data comes from the **[OpenDota API](https://docs.opendota.com)** — completely free, no authentication required for standard endpoints. Rate limit is ~50k requests/month on the free tier.

Key endpoints used:
- `GET /players/{accountId}` — player profile
- `GET /players/{accountId}/wl` — win/loss record
- `GET /players/{accountId}/recentMatches` — last 20 matches
- `GET /players/{accountId}/heroes` — hero stats
- `GET /heroes` — full hero list with IDs

---

## ⚠️ Disclaimer

DOTASTATS is an independent fan project and is **not affiliated with Valve Corporation** in any way. Dota 2 is a trademark of Valve Corporation.