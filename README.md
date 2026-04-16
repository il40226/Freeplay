# Freeplay Games

A simple unblocked games site that runs on `file://` protocol. No server needed.

## Setup

Unzip and open `index.html` in your browser.

## Adding Games

1. Put the game HTML file in `games/` (e.g. `games/snake.html`)
2. Put a thumbnail in `images/` (e.g. `images/snake.png`)
3. Open `js/main.js` and add to the `GAMES` array:

```js
{ id: "snake", name: "Snake", image: "images/snake.png", file: "games/snake.html" },
```

## File Structure

```
freeplay/
├── index.html       ← Main page
├── settings.html    ← Settings page
├── css/style.css    ← All styles
├── js/
│   ├── settings.js  ← Settings module
│   └── main.js      ← Game list & logic
├── images/          ← Game thumbnails
└── games/           ← Game HTML files
```

## Game Open Modes

- **Iframe** — 90% wide × 87% tall overlay
- **New Tab** — Opens file:// link in new tab
- **Same Tab** — Replaces current tab
- **about:blank** — Game embedded inside an about:blank window

## Other Features

- Search bar to filter games
- Tab disguise (customizable title)
- Panic key (customizable key + redirect URL)
- All settings saved to localStorage
