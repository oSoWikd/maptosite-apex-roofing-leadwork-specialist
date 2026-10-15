# DESIGN SPECIFICATION (DESIGN.md)
## Client: Apex Roofing & Leadwork Specialist (Roofer)
*Compiled via MapToSite Engine for Google Stitch Fulfillment*

---

### 1. Brand Identity & Strategy
- **Client Trade**: Roofer
- **Primary Market**: Bristol, UK
- **Core Value Proposition**: Rapid, reliable, fully-insured trade craftsmanship with direct owner accountability.
- **Key Trust Anchor**: Google Maps verified score of **4.9★** over **64 customer reviews**.

---

### 2. Color Palette & Design Tokens
```css
:root {
  /* Brand Primary */
  --color-primary: #0f172a;
  --color-surface: #1e293b;

  /* High-Visibility Trade Accent */
  --color-accent: #ea580c;
  --color-accent-hover: #c2410c;
  --color-text-accent: #fb923c;

  /* Base Typography & Backgrounds */
  --color-bg-base: #090d16;
  --color-text-main: #f8fafc;
  --color-text-muted: #94a3b8;
  --color-border: #334155;
  --color-success: #10b981;
}
```

---

### 3. Typography Scale & Fonts
- **Primary Font Family**: `Plus Jakarta Sans`, system-ui, -apple-system, sans-serif
- **Font Import**:
  ```html
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=JetBrains+Mono:wght@500;700&display=swap" rel="stylesheet">
  ```
- **Scale**:
  - `h1` (Hero Title): `text-3xl md:text-5xl font-extrabold tracking-tight`
  - `h2` (Section Header): `text-2xl md:text-3xl font-bold`
  - `h3` (Card Title): `text-lg font-semibold`
  - `body`: `text-base text-slate-300 leading-relaxed`
  - `meta`: `text-xs uppercase tracking-wider text-slate-400 font-mono`

---

### 4. Layout Architecture (Zero-Pill Discipline)
- **Container**: Max width `1200px` (`max-w-7xl mx-auto px-4 sm:px-6 lg:px-8`).
- **Header**: Sticky `h-16` with high contrast logo mark and tap-to-call button (`+44 117 942 8821`).
- **Hero Section**:
  - Two-column layout on desktop: Headline + CTA on left, interactive verified Google Review card on right.
  - Social proof quote:
    > "Apex came out the same afternoon after the storm ripped three tiles off our roof and rain was coming into the loft. Fixed it cleanly in an hour and didn’t charge astronomical callout money. Top honest lads."
    > — **Dave Higgins** (Verified Google Review)
- **Services Showcase**:
  - `Emergency Storm Damage & Leak Sealing`
  - `Natural Slate & Clay Tile Roof Renewals`
  - `Lead Valley Flashing & Chimney Repairs`
  - `Flat EPDM Rubber & Fibreglass GRP Systems`
  - `uPVC Gutters, Soffits & Dry Verge Fitting`

- **Extra Turnkey Pages**: `Emergency Storm Callouts`, `Leadwork & Chimney Restorations`

---

### 5. Contact Form & Handover Specifications
- **Submission Engine**: Web3Forms static endpoint (`https://api.web3forms.com/submit`).
- **No Database Overhead**: Form triggers automated email alerts to the business owner instantly.
- **Hosting Target**: Cloudflare Pages / Static CDN (0 monthly hosting costs).
- **DNS Handover**: Direct A-record or CNAME pointing to static distribution.
- **Client Turnkey Price**: £480 one-off (zero monthly retainers).
