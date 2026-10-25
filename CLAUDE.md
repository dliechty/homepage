# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Static personal homepage for David Liechty. Single-page site with no build step, no dependencies, and no tests.

## Architecture

- **`index.html`** — The entire site: HTML, CSS (inlined in `<style>`), inline SVG icons/favicon, and a small inline `<script>` (live service status, scroll reveal, snake easter egg).
- Deployed via **GitHub Pages** directly from the `main` branch.
- Dark-only "home lab terminal" theme built on **CSS custom properties** (`--color-*`); amber accent, green/red for status.
- Typography from Google Fonts (JetBrains Mono for headings/terminal bits, Inter for body text).
- Service cards read live status from Uptime Kuma badge endpoints (`status.qwertyshoe.com/api/badge/<id>/status`; the badges allow cross-origin reads, the heartbeat JSON API doesn't). Each card's `data-monitor` is the monitor ID on the public `/status/home` page.
- Motion respects `prefers-reduced-motion`.

## Development

Open `index.html` in a browser. No build or serve commands needed.

## Deployment

Push to `main` — GitHub Pages serves the site automatically.
