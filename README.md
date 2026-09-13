# WorldAI-WAI-
# WAI — World AI Browser

A browser-style web app with real tab management, navigation, bookmarks, history, and a built-in AI assistant — all running from a single HTML file.

## What it is

WAI is a functional browser shell you open in your own browser. It gives you tabs, an address bar, search, bookmarks, and history like a normal browser, plus an AI sidebar ("Ask WAI") you can chat with while you browse.

It is **not** a native browser engine — it runs inside your existing browser (Chrome, Safari, Edge, etc.) as a self-contained web page. Any site it "loads" is displayed inside an iframe, which means it inherits the security rules every browser-in-a-browser runs into (see **Known limitation** below).

## Features

- **Tabs** — open, switch, close, pin, and reopen closed tabs
- **Private tabs** — don't get saved to history
- **Address bar** with a live status indicator (green = should load, orange = will be blocked, teal = will run as a search)
- **Search engine picker** — DuckDuckGo, Wikipedia, Google, or Bing, saved as your default
- **Bookmarks bar** and **history**, both persisted across sessions
- **Settings panel** — light/dark theme, reduce-motion, default search engine, homepage
- **Zoom controls** per tab
- **Real favicons** for tabs, bookmarks, history, and quick links
- **New tab page** — world clock strip plus a curated directory of real sites organized into Reference, News & Ideas, Tools & Archives, and Explore
- **Ask WAI** — an AI assistant sidebar, powered by Claude, for chatting or thinking through whatever you're browsing

## Getting started

1. Download `wai-browser.html`
2. Open it in any modern browser — double-click it, or drag it into a browser window
3. Start typing in the address bar to search or navigate

No installation, server, or build step required.

## Keyboard shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl/Cmd + T` | New tab |
| `Ctrl/Cmd + Shift + N` | New private tab |
| `Ctrl/Cmd + Shift + T` | Reopen last closed tab |
| `Ctrl/Cmd + W` | Close current tab |
| `Ctrl/Cmd + L` | Focus the address bar |

## Known limitation

Some sites — Google, YouTube, Facebook, Instagram, Twitter/X, Amazon, Netflix, LinkedIn, TikTok, Apple, Yahoo, Bing, Snapchat, Pinterest, WhatsApp, Microsoft — set a security header that blocks any outside page, including WAI, from displaying them in a frame. This is a policy the site itself controls, not something WAI can override. When you hit one, WAI shows a fallback card with a real "open in a new tab" button instead of a blank page.

## Data & privacy

Bookmarks, history, and settings are saved locally to the browser's own storage for this app — nothing is sent anywhere except the pages you actually navigate to, and messages you send to the Ask WAI assistant.

## License

WAI — World AI Browser
Copyright (c) 2026 Abhi. All rights reserved.

This software and its source code may not be copied, modified, redistributed, or used to create derivative works without prior written permission from the copyright holder. See `LICENSE.txt` for full terms.
