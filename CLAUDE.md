# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static single-page website for "Völser Radl-Börse" - a bicycle exchange event organized by Pfadfinder*innengruppe Völs (Austrian Scouts) in Tyrol. The site is in German.

**Live URL**: https://radlboerse.voels.org (hosted via GitHub Pages)

## Tech Stack

- **HTML5** with semantic elements (`<main>`, `<section>`, `<aside>`)
- **Bootstrap 5.3.x** (css/bootstrap.min.css, js/bootstrap.bundle.min.js)
- **Custom PPOE Theme** (css/ppoe-theme.css) following PPOE brand guidelines
- No build process - edit files directly and commit

## Development

Open `index.html` in a browser. No server required for basic development. For local server:

```bash
python3 -m http.server 8000
```

## Architecture

### CSS Structure

1. `css/fonts.css` - Font face declarations (Kumbh Sans, Gloria Hallelujah)
2. `css/bootstrap.min.css` - Bootstrap 5 core
3. `css/ppoe-theme.css` - All custom styles with CSS custom properties

### PPOE Brand Colors (defined in :root)

- `--ppoe-red: #9D2632` (primary)
- `--ppoe-gray: #4D4F5A` (secondary/text)
- Stage colors: `--ppoe-biber`, `--ppoe-wiwoe`, `--ppoe-gusp`, `--ppoe-caex`, `--ppoe-raro`

Reference: https://ppoe.at/service/ressourcen/design/

### Typography

- Body: `var(--font-body)` = Kumbh Sans
- Accent/Slogans: `var(--font-accent)` = Gloria Hallelujah

### Key CSS Classes

- `.ppoe-navbar` - Red navbar styling
- `.featurette` / `.featurette-heading` - Main content sections
- `.slogan` - Rotated accent text in Gloria Hallelujah
- `.content-card` / `.content-card--primary` - Card boxes
- `.alert-ppoe-danger` / `.alert-ppoe-success` - Alert boxes with icons
- `.ablauf-list` - Definition list for process steps
- `.steps-list` - Numbered step cards
- `.btn-ppoe-download` - Green download buttons
- `.map-link` - Links to maps with pin icon

### Icons

Custom PPOE-styled SVG icons in `img/ppoe-icons/`:
- download.svg, info.svg, map-pin.svg, success.svg, warning.svg

## Annual Updates

Each year before the event, update:

1. **Dates** in index.html:
   - Hero section h2 (event date)
   - JSON-LD structured data (startDate, endDate with timezone)
   - Meta description
   - Spenden section (donation deadline)
   - Footer copyright year

2. **Phone number** if changed (Kontakt section)
