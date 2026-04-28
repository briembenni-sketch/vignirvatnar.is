# vignirvatnar.is

Landing page for **Vignir Vatnar ehf** — an Icelandic online chess academy run by GM Vignir Vatnar Stef&#225;nsson (Iceland's #1 chess player, 2&#215; Icelandic Champion).

## Stack

- Single-file HTML/CSS/JS (`index.html`)
- Google Fonts: Cormorant Garamond, Inter, JetBrains Mono
- Deployed via Vercel (auto-deploy on push to `main`)

## Design

"Luxury chess club" aesthetic — dark, warm, gold accents.

- **Colors:** `#0b0a08` (bg), `#f3ead8` (ink), `#c9a961` (gold), `#e8c878` (gold-bright)
- **Fonts:** Cormorant Garamond (display), Inter (body), JetBrains Mono (labels)
- Subtle grain texture overlay, radial gold glows
- Animated chessboard, floating king on CTA, fade-up scroll reveals
- Fully responsive with mobile hamburger menu

## Features

### SEO
- Open Graph and Twitter Card meta tags
- JSON-LD structured data (Person, Organization, Course)
- Canonical URL
- SVG chess king favicon
- Semantic HTML with proper heading hierarchy

### Accessibility (WCAG 2.1 AA)
- Gold focus rings on all interactive elements (`:focus-visible`)
- `prefers-reduced-motion` support — disables all animations
- ARIA labels on icon buttons, hamburger menu, nav landmarks
- `aria-expanded` state on mobile menu toggle
- Proper `role` attributes and landmark regions
- `aria-hidden` on decorative elements

### i18n
- Language toggle stub (IS/EN) in navigation
- Currently both options show Icelandic content
- `<!-- TODO: implement EN translation -->`

## URL Paths (Wix integration)

All navigation links point to existing Wix-hosted pages:

| Path | Page |
|------|------|
| `/blog` | Blog |
| `/velja-&#225;skrift` | Choose subscription |
| `/st&#243;rmeistarapakkinn` | GM package |
| `/h&#243;pkennsla` | Group lessons |
| `/&#254;j&#243;nusta-fyrir-fyrirt&#230;ki` | Corporate services |
| `/kaupa-n&#250;na` | Buy now |
| `/skilm&#225;lar` | Terms |
| `/personuverndarstefna` | Privacy policy |

## Known TODOs

- [ ] Implement English translation (i18n)
- [ ] Replace placeholder photo with GM Vignir professional photo
- [ ] Add actual student testimonials (currently placeholder)
- [ ] Add `og:image` once hero image is available
- [ ] Connect Vercel deployment
- [ ] Set up Plausible Analytics

## Development

Open `index.html` in a browser. No build step required.

## Changelog

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
