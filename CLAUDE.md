# Legends of O'nyith — onyith.net

Fiction site built with Jekyll, hosted on GitHub Pages.

## Stack

- Jekyll 4.3, GitHub Pages
- Local dev: `docker compose up` → localhost:4000

## Content

- **Landing page** (`index.html`) — prologue/blurb for the series
- **Chapters** (`_chapters/`) — fiction chapters with front matter:
  ```yaml
  ---
  title: Chapter Title
  chapter_number: 1
  ---
  ```
  Chapter layout auto-generates prev/next navigation sorted by `chapter_number`.

## AI additions to fiction

AI may occasionally suggest worldbuilding or narrative additions. These **must** be marked:

```html
<span class="ai-addition" title="Added by AI">suggested text here</span>
```

This renders as a dotted underline with a hover tooltip. The convention is disclosed at `/disclosure/` and referenced in the footer: **if it's not underlined, a human wrote it.**

Do not add unmarked AI-generated text to any fiction content.

## Design

- Dark theme by default, light theme toggle available
- Teal-green accent (#4a9a8a) — the green/blue planet
- Serif typography (Georgia/Palatino) for fiction readability
- Minimal nav — just the title and theme toggle for now
