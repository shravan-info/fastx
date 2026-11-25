# Fastx Search

Fastx is a lightweight, responsive search hub built with plain HTML, CSS and JavaScript. It has no build step, no framework dependency and no API key requirement.

## Features

- Responsive search homepage and search results layout.
- Search suggestions through DuckDuckGo's autocomplete endpoint.
- Knowledge results from Wikipedia and quick answers from DuckDuckGo Instant Answer when available.
- Full web, image, video, news, map and book searches through DuckDuckGo, Bing or Google.
- Light/dark theme, recent searches stored locally in the browser, keyboard shortcut (Ctrl/⌘ + K) and a basic offline app shell.
- Privacy information and no analytics or advertising trackers added by Fastx.

## Run locally

Open `index.html` in a browser, or run a local static server from this directory:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Open the repository's **Settings → Pages**.
2. Choose **Deploy from a branch**.
3. Select `main` and `/ (root)`, then save.
4. Open the Pages URL shown by GitHub after deployment.

All files use relative paths, so the site can be hosted at a project URL such as `https://shravan-info.github.io/fastx/`.

## Search scope and data sources

Fastx's built-in knowledge panel searches Wikipedia and can show DuckDuckGo Instant Answer summaries. These endpoints do not provide a complete index of the public web. For broad web search and category-specific results, Fastx opens the selected search provider in a new tab. This keeps the project static and avoids paid search API keys or a server-side proxy.

Search suggestions and instant answers depend on third-party services being reachable. Recent searches stay in this browser's local storage and can be cleared from the homepage.
