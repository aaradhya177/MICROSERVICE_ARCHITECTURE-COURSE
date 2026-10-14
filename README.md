# Distributed Systems Fieldbook

A zero-build, browser-local microservices engineering course in Go. It contains 30 modules, 90 lessons, interactive architecture exercises, quizzes, projects, a glossary, search, theme switching, bookmarks, and progress tracking.

## Run locally

```powershell
cd distributed-systems-fieldbook
python -m http.server 8080 --directory dist
```

Open `http://localhost:8080`. No install or build step is required.

## Architecture

- `dist/index.html` â€” semantic application shell and metadata
- `dist/styles.css` â€” responsive design system and light/dark themes
- `dist/content.js` â€” curriculum, examples, glossary, projects, sources
- `dist/app.js` â€” router, renderers, search, quizzes, lab, local persistence
- `docs/` â€” design, curriculum, validation, and source notes

Progress uses `localStorage`; it is intentionally not presented as account-synchronized. Code execution is a labeled static learning environment: examples are copyable and include local commands.

## Supported browsers

Current Chrome, Edge, Firefox, and Safari. The app uses no runtime framework or third-party script; the only external request is the optional web font.

