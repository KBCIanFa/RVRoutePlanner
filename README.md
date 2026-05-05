# 🚐 RV Route Planner AU — Caravan Companion

> AI-powered route planning for Australian caravans and motorhomes. Plan the Big Lap, a weekend run, or anything in between.

**🔗 Live App:** [kbcianfa.github.io/RVRoutePlanner](https://kbcianfa.github.io/RVRoutePlanner)

---

## What It Does

RV Route Planner AU uses the Claude AI (Anthropic) to generate detailed, day-by-day caravan route itineraries tailored to your rig, your pace, and what you want to see along the way.

Enter a start point, destination, trip duration and a few preferences — the AI does the rest. You get a full itinerary with daily legs, distances, points of interest, camp recommendations, fuel stops, and practical travel tips. No sign-up, no backend, no nonsense.

---

## Features

**Route Planning**
- Custom origin → destination routing across Australia
- Trip type selection: leisurely, standard, or fast-paced
- Duration-aware itinerary generation (1-day to multi-week)
- Quick-route presets for popular runs (Big Lap, East Coast, Red Centre, etc.)

**Rig & Preferences**
- Rig type selection (caravan, motorhome, camper trailer, fifth wheeler)
- Road type preference (sealed, unsealed, mixed)
- Daily distance limits

**Points of Interest**
- Configurable POI types per trip: free camps, caravan parks, fuel stops, dump points, scenic lookouts, food/coffee, water
- Each POI shown with category, description, and Google Maps link

**Day Cards**
- Collapsible day-by-day itinerary cards
- Route leg summary (from → to, km, drive time)
- Narrative description for each day
- POI list with colour-coded category tags

**Chat Tab**
- Follow-up questions about your route answered in context
- Ask about alternatives, timing, road conditions, what to pack

**Export & Share**
- Copy itinerary to clipboard
- Print-friendly view
- QR code generation for sharing the live app

**UI**
- Clean amber/ochre earthy design — feels like the outback, works on mobile
- Sticky header with collapsible API key bar
- Responsive layout (sidebar + main panel → stacked on mobile)

---

## Tech Stack

| Thing | Detail |
|---|---|
| Language | Vanilla HTML/CSS/JS — zero build tools |
| AI | [Anthropic Claude API](https://www.anthropic.com) (`claude-sonnet-4-20250514`) |
| Fonts | Bebas Neue, Barlow, Barlow Condensed (Google Fonts) |
| QR Codes | qrcodejs (CDN) |
| Hosting | GitHub Pages |
| Architecture | Single-file app (`index.html`) + help page + home page |

This is a **vibe-coded** tool — no npm, no frameworks, no build pipeline. Open the file, it runs.

---

## Getting Started

### Use the Hosted Version

Head to [kbcianfa.github.io/RVRoutePlanner](https://kbcianfa.github.io/RVRoutePlanner), enter your Anthropic API key, and start planning.

### Run Locally

```bash
git clone https://github.com/KBCIanFa/RVRoutePlanner.git
cd RVRoutePlanner
# Open index.html in your browser — that's it.
```

No server required. Open `index.html` directly in any modern browser.

---

## API Key

This app calls the Anthropic Claude API directly from your browser. You need a valid API key from [console.anthropic.com](https://console.anthropic.com).

**Enter your key in the bar at the top of the app.** It is stored in `sessionStorage` only — never sent anywhere except directly to Anthropic's API. Refresh the page and it's gone.

> ⚠️ For personal/low-traffic use only. Don't share your API key publicly. Anthropic API usage incurs costs — check your [usage dashboard](https://console.anthropic.com).

---

## Files

```
RVRoutePlanner/
├── index.html    # Main app — route planner, chat, export
├── home.html     # Landing/marketing page
├── help.html     # User guide and FAQ
└── README.md
```

---

## Part of the Vibe Coding Portfolio

This tool is part of a suite of Australian-focused single-file web tools built at [kbcianfa.github.io](https://kbcianfa.github.io). Other tools in the family:

- [RV Power Designer](https://kbcianfa.github.io/RVPowerSystems) — solar/battery system sizing for caravans
- [TowCheck AU](https://kbcianfa.github.io/Towing/) — towing compliance calculator
- [LogMyJourney AU](https://kbcianfa.github.io/LogMyJourney/) — trip logging for the road
- [Aussie Translator](https://kbcianfa.github.io/AussieTranslator/) — AI-powered Australian slang tools

---

## Licence

MIT — do what you like with it. Attribution appreciated but not required.

---

*Built in Queensland, Australia. Tested on the road.*
