# ReefbytesMV Website

## Overview
Static HTML/CSS website for ReefbytesMV — a Maldives-based software engineering and web development company (www.reefbytesmv.com).

## Project Structure
- `index.html` — Main homepage (redesigned, modern dark UI)
- `careers.html` — Careers page (has its own embedded `<style>` block)
- `styles.css` — Global stylesheet (full dark premium redesign)
- `sitemap.xml` — XML sitemap for search engines
- `robots.txt` — Search engine crawl rules
- `assets/` — Logo and hero background images (NOT tracked by git — must be regenerated on rollback)

## Design System (styles.css)
- **Theme**: Dark premium — `#09090B` background, glass-morphism cards
- **Fonts**: Inter (UI) + JetBrains Mono (labels/accents) via Google Fonts
- **Accent colors**: Electric blue `#2563EB`, Violet `#7C3AED`, Cyan `#06B6D4`
- **Components**: Pill buttons (.btn, .btn-ghost, .btn-sm), section labels, gradient text, tag pills, stats strip, portfolio overlay cards

## Page Sections (index.html)
1. Fixed dark glass navbar with "Get a Quote" CTA button
2. Full-height hero with badge, large gradient text, two CTAs, scroll indicator
3. Stats strip (8+ years, 150+ projects, 40+ team, 98% satisfaction)
4. About section (two-column with trust badges)
5. Services grid (6 cards — custom software, mobile, web, cloud, security, AI)
6. Portfolio grid (3 image cards with tag overlays)
7. Contact section (info panel + Formspree-connected form)
8. Footer (4-column dark footer)

## SEO
- Meta description, keywords, canonical URL all using `https://www.reefbytesmv.com`
- Open Graph + Twitter Card tags
- JSON-LD ProfessionalService schema with Malé/Maldives address
- Sitemap and robots.txt configured

## Assets (regenerate on rollback)
- `assets/hero-bg.png` — Dark coding-themed 16:9 hero background
- `assets/logo-icon-nobg.png` — Hexagonal blue-purple logo, transparent background

## Known Notes
- `careers.html` has its own embedded `<style>` block — CSS changes must be applied there separately
- Contact form uses Formspree endpoint: `https://formspree.io/f/xblvgzzl`
- Hours listed as Sun–Thu 9AM–6PM MVT (Maldives timezone, not PST)

## Running the Project
```
python3 -m http.server 5000
```

## Deployment
Configured as a static site. Public directory: `.` (root)
