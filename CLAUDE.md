# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Static single-page marketing website for Kartavya Technology™ — an official Anthropic partner. No build step, no framework, no dependencies. Open `index.html` directly in a browser to preview.

## Stack

- **index.html** — single HTML file; all sections are inline (navbar, hero, stats, services, about, consultation, footer)
- **styles.css** — all styles; uses CSS custom properties defined in `:root` for the dark theme palette
- **script.js** — vanilla JS; handles navbar scroll effect, mobile nav toggle, smooth scroll, service card fade-in via `IntersectionObserver`, active nav link tracking, and founder photo error fallback
- **assets/images/** — `logo.png` (nav/footer logo) and `dharam-tiwari.jpg` (founder photo in the About section)

## Design tokens (CSS custom properties)

All colours, spacing, and typography reference variables in `:root` at the top of `styles.css`. Edit those variables first when making visual changes rather than hardcoding values throughout the file.

Key tokens: `--accent` (#3b82f6 blue), `--bg-primary` (#0a0a0a), `--bg-secondary` (#0f172a), `--text-primary`, `--text-secondary`, `--border`, `--radius`, `--container` (1200px max-width).

## Page structure

Sections in order: `#home` (hero) → stats bar → `#services` → `#about` → `#consultation` → `#contact` (footer). Nav links use anchor `href="#id"` smooth-scroll handled in `script.js`.

## Responsive breakpoints

- `≤900px` — services grid and about grid collapse to single column; footer goes 2-column
- `≤768px` — mobile nav (hamburger toggle), stats grid 2×2, footer 1-column
- `≤480px` — hero/section padding reduced, CTA buttons full-width

## External links

- Calendly booking: `https://calendly.com/dharam-tiwari/30min`
- Founder LinkedIn: `https://www.linkedin.com/in/dharamtiwari/`
- Company LinkedIn: `https://www.linkedin.com/company/kartavyatech/`
- Twitter/X: `https://x.com/draj_02`
