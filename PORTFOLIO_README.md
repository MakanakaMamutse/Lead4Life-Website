# Lead4Life — Full Website Build

**Live site:** [www.lead4life.co.za](https://www.lead4life.co.za)

A complete, production-grade website built from scratch for **Lead4Life**, a South African experiential leadership development organisation with 23+ years of impact and 180,000+ lives reached across schools, corporates, communities, and beyond.

---

## Project Overview

| | |
|---|---|
| **Type** | Multi-page static website |
| **Timeline** | December 2025 – May 2026 (4+ months) |
| **Status** | Live & in active continuous refinement |
| **Commits** | 222+ |
| **Pages** | 26 |
| **CSS source files** | 54 |
| **JavaScript modules** | 30 |
| **Image assets** | 146 |
| **Logo assets** | 60 client & partner logos |
| **Total assets** | 214 files |

---

## Scale & Structure

### Pages (26 total)

**Core**
- Homepage, About, Overview, Programmes, Clients & Partners, Gallery, Testimonials, FAQs, Contact, Resources, Careers, Business Opportunities, 404

**Market Segments (8)**
- Schools, Tertiary Students, Corporates, Entrepreneurs & SMEs, NPOs & Faith-Based Organisations, Individuals, Young Adults, Communities

**LifeClub Sub-brand (5)**
- Landing page, Gallery, Testimonials, Clients, Resources

**Legal (3)**
- Privacy Policy, Terms & Conditions, Cookie Policy

---

### CSS Architecture

54 source CSS files organised into a modular system:

```
css/
├── global.css                  — design tokens, resets, typography
├── sections/                   — one file per page section (navbar, hero, footer, etc.)
├── components/                 — reusable UI components (modals, sliders, etc.)
├── pages/                      — page-specific overrides
└── build/                      — 25 per-page bundles (generated, not hand-written)
```

A custom Node.js build script (`build-css.js`) scans each HTML page, collects its CSS dependencies, and generates a single import bundle per page — keeping source files editable without a full rebuild every time.

---

### JavaScript (30 modules)

Every interactive element on the site has a dedicated, purpose-built JS file:

| Module | Purpose |
|---|---|
| `hero-auto-scroll.js` | Timed hero carousel with scroll-state detection |
| `market-carousel.js` | Horizontal market segment carousel |
| `scroll-animations.js` | Intersection Observer-based entrance animations |
| `stats-counter.js` | Animated number counters triggered on scroll |
| `gallery-filter.js` | Live category filtering for gallery |
| `gallery-cycle.js` | Step-by-step image cycling (Moments of Transformation) |
| `testimonials-carousel.js` | Auto-advancing testimonials slider |
| `l4l-programs-cards.js` | Interactive programme cards |
| `video-modal.js` | Accessible video modal overlay |
| `zoho-validation.js` | Contact form validation & Zoho CRM integration |
| `navbar.js` | Transparent → solid scroll transition, mobile menu |
| `honeycomb-logos.js` | Hexagonal animated logo grid |
| + 18 more | Section-specific animations and interactions |

---

## Features & Technical Highlights

### Performance
- PageSpeed Insights: **100 SEO / 100 Accessibility / 100 Best Practices**
- Mobile performance score: **60** (up from 55, actively being improved)
- Hero images served in WebP with mobile-specific variants
- All below-fold images lazy-loaded
- Critical resources (logo, hero image) preloaded in `<head>`
- Google Fonts and icon libraries loaded asynchronously (non-blocking)

### SEO & Discoverability
- Full structured data (Schema.org `Organization` + `WebSite`)
- Open Graph & Twitter Card meta tags on every page
- Canonical URLs on all pages
- XML sitemap covering all 26 pages
- `robots.txt` correctly configured for Googlebot access
- Meta descriptions, titles, and `robots: index, follow` on every page

### Accessibility
- Semantic HTML throughout (headings hierarchy, landmark regions)
- ARIA labels on all interactive elements
- Keyboard-navigable navigation and modals
- Colour contrast compliant across all sections
- 100/100 Lighthouse Accessibility score

### Design System
- Two colour brands (Lead4Life green + LifeClub navy/teal) fully separated
- Consistent spacing tokens, typography scale, and component patterns
- Fully responsive — mobile-first breakpoints across all 26 pages
- Smooth CSS animations with `prefers-reduced-motion` awareness
- 60 client and partner logos organised by tier (priority vs standard)

### Integrations
- **Zoho CRM** — contact form connected to live CRM pipeline
- **Chatbase** — embedded AI chat widget
- **Google Fonts** — Inter + Poppins
- **Font Awesome 6** — icon library
- **Bootstrap Icons** — supplementary icons
- **Lordicon** — animated icons in navigation dropdown

---

## Deployment

Hosted on **Afrihost** shared hosting (South Africa), deployed via FTP. The site is a fully static build — no frameworks, no build dependencies, no server-side runtime required. Pure HTML, CSS, and vanilla JavaScript.

---

## Development Process

Built entirely from scratch over 4+ months across 222+ commits covering:

- Full design and layout from wireframe to pixel-perfect implementation
- Custom CSS architecture designed for long-term maintainability
- Progressive performance optimisation (SEO, accessibility, Core Web Vitals)
- Iterative content and copy refinement with the client
- Cross-browser and mobile testing at each major milestone
- Ongoing post-launch refinements — image optimisation, performance tuning, new sections

---

## About Lead4Life

Lead4Life designs and delivers experiential leadership programmes that engage, enrich, and empower schools, corporates, and communities across South Africa. Operating since 2001, they have reached 180,000+ individuals through outdoor challenge courses, workshops, camps, and community initiatives.

**Address:** 11 Imam Haron Rd, Claremont, Cape Town, 7708
**Website:** [www.lead4life.co.za](https://www.lead4life.co.za)

---

*Built by Makanaka Mamutse*
