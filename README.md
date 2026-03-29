# 🚲 Bike Day Tracker

A lightweight Progressive Web App (PWA) to track which office locations you cycled to each day — so you can easily report your monthly bike distances for reimbursement.

## Features

### Today View
- Opens directly to today's date with one-tap location toggles
- Navigate to previous/next days using the arrow buttons
- "Go to today" shortcut when viewing a past or future date

### Calendar View
- Full month calendar (Mon–Sun) with prev/next month navigation
- Colored dots on days where locations were recorded
- Tap any day to open an edit overlay with the same toggle UI

### Monthly Summary
- Overview card: total days cycled and total km for the month
- Per-location breakdown: day count and km
- Chronological list of each day with colored location badges
- "Copy Summary to Clipboard" button for easy end-of-month reporting

### Location Management
- Add, edit, and delete locations via the ⚙️ settings panel
- Each location has a name, color, and optional distance (km)

## Technical Details

- **Single file** — everything lives in `index.html` (HTML, CSS, JavaScript)
- **Tailwind CSS** — styling via CDN
- **IndexedDB** — all data stored locally on your device, nothing sent to any server
- **PWA** — installable on Android and iOS; works fully offline after first load
  - Inline Web App Manifest (via Blob URL)
  - Inline Service Worker that caches Tailwind & Google Fonts for offline use

## Installation on Mobile

1. Open `index.html` in your mobile browser (Chrome on Android, Safari on iOS)
2. Use the browser's "Add to Home Screen" / "Install App" option
3. The app launches in standalone mode (no browser chrome)

---

## Vibe Coded

This app was **vibe coded** — built entirely through a natural language conversation with an AI assistant, without manually writing a single line of code.

| Tool | Detail |
|---|---|
| **AI Assistant** | GitHub Copilot (in VS Code) |
| **Model** | Claude Opus/Sonnet 4.6 |
| **Verification** | Playwright MCP (automated browser testing during development) |

The full app — including IndexedDB data layer, PWA manifest, service worker, calendar logic, and UI — was designed, implemented, and tested in a single conversation session.
