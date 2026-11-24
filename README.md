# ESG Booster Workshop 2027 Landing Page

Official landing page for the **ESG Booster Workshop 2027** (*3rd Edition: From Compliance to Sustainable Leadership*), jointly organised by **Guru Gobind Singh Indraprastha University (GGSIPU)** and **EHS Guru Sustainable Solutions Pvt. Ltd.** (Council of EHS & ESG Excellence).

- **Event Date**: Saturday, 30 January 2027 (10:00 AM – 5:00 PM)
- **Venue**: GGSIPU, Sector 16C, Dwarka, New Delhi
- **Registration Deadline**: 15 January 2027

---

## 📁 Repository Structure

```
ESG_BOOSTER/
├── index.html                                    # Production ad landing page (external AVIF/WebP assets)
├── index-standalone.html                         # All-in-one standalone file (embedded base64 assets)
├── esg-booster-workshop-2027-for-website (1).html # Updated production prototype
├── ESG-Booster-Workshop-2027-Landing-Page-Spec.docx # Specification document
├── assets/                                       # Multi-format image assets
│   ├── logo-ehs-guru.{avif,webp,png}
│   ├── logo-ggsipu.{avif,webp,png}
│   ├── speaker-varun-joshi.{avif,webp,jpg}
│   ├── speaker-prodyut-bhattacharya.{avif,webp,jpg}
│   └── speaker-munish-kumar.{avif,webp,jpg}
└── README.md
```

---

## 🚀 Key Features & Performance

1. **Server-Side Synchronized Countdown Timer**:
   - Calibrated against the authoritative server HTTP `Date` response header via `HEAD` requests.
   - Elapsed time is tracked using `performance.now()` (monotonic clock), ensuring 100% immunity against user system clock drift, manual device time changes, or timezone skews.
   - Dynamic sticky CTA bar on mobile automatically updates with remaining days.
2. **Performance & Core Web Vitals**:
   - Zero render-blocking resources: inlined critical CSS with asynchronous print-swap font loading.
   - Next-gen image format negotiation (`<picture>` with AVIF + WebP fallback).
   - `content-visibility: auto` with `contain-intrinsic-size` on below-the-fold sections for instant initial rendering.
   - `DOM Content Loaded < 60ms` and `JS Heap < 1 MB`.
3. **SEO & Structured Data**:
   - Canonical URL, Open Graph meta tags, and Twitter Card tags.
   - Schema.org structured data (`Event` and `FAQPage` via JSON-LD).
4. **Mobile Responsiveness**:
   - Verified across viewports from 320px to 1920px with zero horizontal overflow.
   - Sticky mobile registration action bar with safe-area inset support (`env(safe-area-inset-bottom)`).
5. **Brand Design System**:
   - Locked strictly to the official light brand palette (`--teal-deep: #08465A`, `--sun: #FFD84D`, `--mist: #E4EFEA`, `--leaf: #178A4A`, `--paper: #F6F9F6`).

---

## 💻 Local Preview

Run any local static HTTP server:
```bash
python -m http.server 8080
```
Open `http://localhost:8080/index.html` in your browser.
