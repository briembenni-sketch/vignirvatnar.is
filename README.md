# vignirvatnar.is

Landing page for **Vignir Vatnar ehf** — an Icelandic online chess academy run by GM Vignir Vatnar Stefánsson (Iceland's #1 chess player, 2× Icelandic Champion).

## Stack

- Single-file HTML/CSS/JS (`index.html`)
- Google Fonts: Cormorant Garamond, Inter, JetBrains Mono
- Plausible Analytics (privacy-friendly)
- Deployed via Vercel (auto-deploy on push to `main`)

## Design

"Luxury chess club" aesthetic — dark, warm, gold accents.

- **Colors:** `#0b0a08` (bg), `#f3ead8` (ink), `#c9a961` (gold), `#e8c878` (gold-bright)
- **Fonts:** Cormorant Garamond (display), Inter (body), JetBrains Mono (labels)
- Subtle grain texture overlay, radial gold glows
- Animated chessboard, morphing chess piece, fade-up scroll reveals
- Fully responsive with mobile hamburger menu

## Features

### Sections
- Hero with portrait placeholder, morphing chess piece animation, CTA
- "Featured in" bar (Lichess, FIDE, RÚV, etc.)
- Achievements bar (500+, 2×, 2400, #1)
- About section with GM credentials
- Courses section with tactical chess board (highlighted squares)
- Testimonials (3-card grid with decorative quotes)
- "What you'll learn" — 6 category cards (Openings, Tactics, Strategy, Endgames, Calculation, Mental game)
- Pricing section with monthly/yearly toggle, savings calculator, direct repeat.is checkout links
- Team section
- FAQ accordion (6 questions, a11y-compliant)
- Final CTA section
- Newsletter signup (frontend-only, ready for ConvertKit/Mailerlite)

### Conversion Optimization
- Sticky bottom-bar CTA on mobile (shows after scrolling past hero)
- Direct checkout links to repeat.is (monthly + yearly)
- Pricing toggle with "Vinsælast" badge switching
- Social proof badge (646+ Instagram followers)
- Plausible event tracking on all CTA clicks

### SEO
- JSON-LD structured data (Person, Organization, Product, FAQPage)
- Open Graph and Twitter Card meta tags with og:image
- Canonical URL + hreflang (is, x-default)
- sitemap.xml and robots.txt
- SVG chess king favicon

### Accessibility (WCAG 2.1 AA)
- Skip-to-content link
- Gold focus rings on all interactive elements (`:focus-visible`)
- `prefers-reduced-motion` support
- ARIA labels on icon buttons, hamburger, nav landmarks
- FAQ buttons with `aria-expanded` state
- Proper heading hierarchy and landmark regions

### Performance
- Hero image preload with `fetchpriority="high"`
- Image placeholders ready for lazy-loading
- All CSS/JS inline (no external requests beyond fonts + analytics)
- Single-file architecture — no build step

### Analytics
- Plausible Analytics (`data-domain="vignirvatnar.is"`)
- CTA click tracking via `plausible()` calls
- Newsletter signup tracking

## URL Paths (Wix integration)

All navigation links point to existing Wix-hosted pages:

| Path | Page |
|------|------|
| `/blog` | Blog |
| `/velja-áskrift` | Choose subscription |
| `/stórmeistarapakkinn` | GM package |
| `/hópkennsla` | Group lessons |
| `/þjónusta-fyrir-fyrirtæki` | Corporate services |
| `/kaupa-núna` | Buy now |
| `/skilmálar` | Terms |
| `/personuverndarstefna` | Privacy policy |

## TODOs for Founder

- [ ] **Add real photos** to `/public/images/` (replace placeholder chess piece icons):
  - `vignir-hero.webp` — Hero portrait (WebP, ~200KB, quality 85)
  - `vignir-about.webp` — About section portrait
  - `vignir-team.webp` — Team section photo
  - `benedikt-briem.webp` — Benedikt's team photo
  - `oliver-johansson.webp` — Oliver testimonial avatar
  - `og-image.jpg` — Open Graph image (1200×630px)
- [ ] **Set up Plausible Analytics account** for vignirvatnar.is domain
- [ ] **Connect newsletter** to ConvertKit or Mailerlite
- [ ] **Add real student testimonials** (replace placeholder quotes)
- [ ] Implement English translation (i18n)

## Development

Open `index.html` in a browser. No build step required.

## Changelog

### 2026-04-28 — Premium polish + conversion optimization

- Added hero section with portrait placeholder and morphing chess piece animation
- Added "Featured in" bar (Lichess, Skáksamband Íslands, FIDE, Visir.is, Morgunblaðið, RÚV)
- Added achievements bar (500+, 2×, 2400, #1)
- Added tactical chess board with highlighted squares and game caption
- Added "What you'll learn" 6-card grid section
- Added pricing section with monthly/yearly toggle, savings calculator
- Added direct repeat.is checkout URLs for both plans
- Added team section (Vignir + Benedikt)
- Added FAQ accordion (6 questions, proper a11y)
- Added sticky mobile CTA bar (shows after scrolling past hero)
- Added newsletter signup form (frontend-only)
- Added social proof badge (Instagram followers)
- Added Plausible Analytics with CTA click tracking
- Added skip-to-content link for accessibility
- Added JSON-LD for Product and FAQPage
- Added hreflang tags, og:image meta tags
- Added sitemap.xml and robots.txt
- Added hero image preload
- Updated all CTA links to "Prófa frítt í 30 daga" with direct checkout URLs

### 2026-04-28 — Initial build

- Created landing page with luxury chess club aesthetic
- Hero section with animated chessboard and floating king CTA
- About section with GM credentials
- Offerings grid (3 cards)
- Testimonials section (placeholder)
- Final CTA section
- Added SEO meta tags, JSON-LD structured data, SVG favicon
- Added `prefers-reduced-motion` support
- Added visible focus rings for keyboard navigation
- Added IS/EN language toggle stub
- Added `vercel.json` with security headers
- Added `.gitignore`