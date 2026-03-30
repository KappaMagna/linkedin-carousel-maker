# Coffee-Break Carousel Maker

> A zero-dependency, single-file LinkedIn carousel creator — built entirely through a vibe coding session with Claude Code.

**No install. No build step. No server. Open the HTML file and start creating.**

---

## What is this?

The **Coffee-Break Carousel Maker** is a browser-based tool for creating multi-slide LinkedIn carousel posts. It was built as the companion app for the [Coffee-Break Guides](https://contento60.gumroad.com/) series by [Contento Consulting](https://contento.consulting) — and as a live demonstration of vibe coding: building real software through conversation with AI, without writing a single line of code manually.

The app ships pre-loaded with content for *"Prompt al Potere"* (Coffee-Break Guide N°2), but every element is fully customizable.

---

## Features

### Content
- **9 editable slides** — cover, hook, techniques, teaser, CTA
- **Click-to-edit** — click directly on any text in the slide preview to modify it inline
- **Import from text or PDF** — paste your content or upload a `.txt` / `.pdf` file and let the app auto-distribute it across slides

### Design
- **3 color themes** — Teal / Dark / Cream, fully customizable via color pickers
- **Font picker** — 7 title fonts + 5 body fonts, loaded on demand from Google Fonts
- **Global font size** — scale all text up or down (70%–140%)
- **Per-slide font size** — independent `A−` / `A+` controls per slide
- **Italic toggle** — per-slide italic for the title
- **Background selector** — choose the color variant per slide

### Format & Export
- **Format toggle** — 1:1 (1080×1080px) or 4:5 (1080×1350px)
- **PDF export** — exports all 9 slides as a print-ready PDF via browser print dialog (LinkedIn-ready)
- **Image upload** — replace the default logo and cover background with your own images

### Brand
- Logo and hero image embedded as base64 — works fully offline
- Topbar logo updates instantly when you upload a new logo

---

## How to use

1. **Download** `carousel_prompt_al_potere_v3.html`
2. **Open** it in any modern browser (Chrome, Safari, Firefox)
3. **Customize** content, fonts, and colors in the left panel — the preview updates live
4. **Export** as PDF via the export button

That's it. No installation, no account, no internet required (except Google Fonts and PDF import, which use CDN).

---

## Import your own content

In the left panel, find **"Importa contenuto"**:

- **Upload a `.txt` or `.pdf` file** — text is extracted and auto-split into slides
- **Paste text** directly — one paragraph per slide (separated by blank lines), first line = title, rest = body
- Click **"Genera slide →"** — content is distributed across slides 1–7; slides 8 (teaser) and 9 (CTA) are preserved

---

## Tech stack

| Layer | Choice | Why |
|-------|--------|-----|
| Architecture | Single-file HTML/CSS/JS | Zero dependencies, works offline, trivial to share |
| Fonts | Google Fonts CDN | Loaded on demand per selection |
| PDF import | PDF.js 3.11 (cdnjs CDN) | Text extraction without a backend |
| PDF export | Browser `window.print()` + `@media print` CSS | No server, no library |
| Images | Base64-embedded PNG | Fully self-contained |

No npm. No bundler. No framework. No build step.

---

## Origin story

This app was built in a single Claude Code session through natural-language conversation — no manual coding. Every feature, from the animated slide transitions to the inline editing and PDF export, was described in words and implemented by Claude.

It is itself the subject of a LinkedIn carousel post about vibe coding.

> *"La chiarezza è il codice."*
> You don't need to know how to program. You need to know exactly what you want.

---

## About

Made with ☕ by **Kerstin Petrick** and **Claude Code**
[Contento Consulting](https://contento.consulting) · Human-AI Synergy Coaching · Italy

Coffee-Break Guides: [contento60.gumroad.com](https://contento60.gumroad.com)

---

## License

MIT — use it, fork it, adapt it for your own carousel series.
