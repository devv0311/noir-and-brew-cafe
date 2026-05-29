<div align="center">

<br/>

```
✦  N O I R  &  B R E W  ✦
```

# Noir & Brew — Specialty Café Landing Page

**A premium, editorial café landing page built with pure HTML, CSS & JavaScript.**  
Designed for a fictional specialty café in Koregaon Park, Pune — focused on luxury branding, conversion-led UX, and immersive visual storytelling.

<br/>

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Google Fonts](https://img.shields.io/badge/Google_Fonts-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://fonts.google.com/)
[![WhatsApp](https://img.shields.io/badge/WhatsApp_API-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/)
[![Responsive](https://img.shields.io/badge/Responsive-Mobile--First-green?style=for-the-badge)]()

<br/>

![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-orange?style=flat-square)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Live Demo](#-live-demo)
- [Screenshots](#-screenshots)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [JavaScript Functionality](#-javascript-functionality)
- [Design System](#-design-system)
- [Responsive Design](#-responsive-design)
- [WhatsApp & Maps Integration](#-whatsapp--maps-integration)
- [Challenges & Learnings](#-challenges--learnings)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

## 🌟 Overview

**Noir & Brew** is a fully responsive, single-page restaurant/café landing website built as a frontend portfolio project. It simulates a real-world client brief — a premium specialty café located in Koregaon Park, Pune — and is designed to demonstrate production-grade HTML/CSS/JS skills in a hospitality context.

The design philosophy prioritises **editorial luxury**: slow scroll, intentional spacing, rich typographic contrast, and a conversion funnel built around WhatsApp reservations. Every section is built to move a visitor from discovery to reservation.

> **This is a static frontend project** — no frameworks, no build tools, no dependencies. Just clean, handcrafted code.

---

## 🚀 Live Demo

<div align="center">

### 🔗 [View Live Site →](https://noir-and-brew.netlify.app/)

*Hosted on Netlify*

</div>

---

## 📸 Screenshots

<div align="center">

### Hero Section
![Hero Section](https://via.placeholder.com/1200x680/080f0a/c9a84c?text=Hero+Section+—+Full+Screen+Dark+Coffee+Background)

---

### Menu Section
![Menu Section](https://via.placeholder.com/1200x620/faf7f0/0d1a10?text=Menu+Section+—+Card+Grid+Layout)

---

### Experience & Testimonials

---

### Contact & Map
![Contact Section](https://via.placeholder.com/1200x520/faf7f0/0d1a10?text=Contact+Section+—+Split+Layout+with+Google+Maps)

</div>

---

## ✨ Features

### 🎨 Brand & Design
- **Premium café brand presentation** — full editorial identity system
- **Cormorant Garamond** serif typography for high-end hospitality feel
- **Green & gold luxury color palette** — consistent across all components
- **Glassmorphism-inspired navigation** — frosted backdrop-filter nav on scroll
- **Animated grain texture** — SVG noise overlay on hero for editorial depth

### 🧭 Navigation & UX
- **Fixed glassmorphism navbar** — transparent on load, frosted dark on scroll
- **Animated hamburger menu** — custom 3-line toggle with CSS transitions
- **Smooth anchor scrolling** — native CSS `scroll-behavior: smooth`
- **Auto-close mobile nav** — closes on any nav link click

### 📋 Sections
| Section | Description |
|---|---|
| **Hero** | Full-viewport image, editorial headline, dual CTA buttons |
| **Marquee** | Animated scrolling brand strip |
| **About** | 2-column grid: café story + stats (rating, menu size, years) |
| **Menu** | 4-card grid with SVG icons and pricing |
| **Experience** | 4-column dark panel with highlight cards |
| **Testimonials** | 3-column review cards with featured dark card |
| **Contact** | Split layout with info list and embedded Google Maps |
| **Footer** | Brand mark, navigation, and credits |

### ⚡ Performance & Interaction
- **Intersection Observer animations** — scroll-triggered fade-up reveal on all major elements
- **Passive scroll listener** — optimised `{ passive: true }` for navbar state
- **Lazy-loaded images** — `loading="lazy"` on all below-fold images
- **CSS custom properties** — full design token system for maintainability

### 📱 Mobile
- **Mobile-first responsive layout** — two breakpoints: 768px and 900px
- **Full-screen mobile nav overlay** — dropdown with full-width links
- **Touch-friendly button sizing** — minimum 44px tap targets
- **Fixed parallax disabled on mobile** — `background-attachment: scroll` to fix iOS performance

---

## 🛠 Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Semantic page structure, accessibility attributes, embedded SVGs |
| **CSS3** | Custom properties, CSS Grid, Flexbox, animations, keyframes |
| **Vanilla JavaScript** | DOM manipulation, Intersection Observer API, scroll events |
| **Google Fonts** | Cormorant Garamond (display) + Outfit (body) |
| **WhatsApp API** | `wa.me` deep-link for direct reservation flow |
| **Google Maps Embed** | `iframe`-based location map |
| **Unsplash** | High-quality placeholder photography |

> **Zero dependencies.** No npm, no bundler, no framework. Intentional.

---

## 📁 Project Structure

```
noir-and-brew/
│
├── index.html          # Full page structure — 8 sections + nav + footer
├── style.css           # All styles — design tokens, layout, animations, responsive
├── script.js           # Mobile nav, sticky navbar, scroll reveal animations
│
└── README.md           # This file
```

### HTML Architecture

```
<nav>           Sticky glassmorphism navbar
<section.hero>  Full-viewport hero — headline, CTA, scroll indicator
<div.marquee>   Animated scrolling brand strip
<section.about> 2-column about grid with image + stats
<section.menu>  4-card menu grid
<section.experience>  4-column dark experience highlights
<section.testimonials> 3-column review cards
<section.contact>     Split contact + embedded map
<footer>        Brand mark, nav, credits
```

---

## ⚙️ JavaScript Functionality

All JS lives in **`script.js`** — 30 lines of clean, purposeful vanilla JavaScript.

### 1. Mobile Navigation Toggle
```javascript
navToggle.addEventListener('click', () => {
  navLinks.classList.toggle('open');
  spans.forEach(s => s.classList.toggle('active'));
});
```
Toggles the mobile dropdown menu and animates the hamburger icon spans on each click.

---

### 2. Auto-Close on Nav Link Click
```javascript
document.querySelectorAll('.nav-links a').forEach(link => {
  link.addEventListener('click', () => {
    navLinks.classList.remove('open');
  });
});
```
Removes the `open` class from the nav overlay whenever any navigation link is clicked — ensuring smooth mobile UX during anchor navigation.

---

### 3. Sticky Navbar on Scroll
```javascript
window.addEventListener('scroll', () => {
  navbar.classList.toggle('scrolled', window.scrollY > 60);
}, { passive: true });
```
Adds the `scrolled` class after 60px of scroll, triggering the CSS backdrop-filter and padding transition. The `passive: true` flag prevents scroll jank.

---

### 4. Scroll Reveal — Intersection Observer
```javascript
const observer = new IntersectionObserver((entries) => {
  entries.forEach((entry, i) => {
    if (entry.isIntersecting) {
      setTimeout(() => entry.target.classList.add('visible'), 80);
      observer.unobserve(entry.target);
    }
  });
}, { threshold: 0.1, rootMargin: '0px 0px -40px 0px' });
```
Every `.menu-card`, `.exp-card`, `.testi-card`, `.stat-item`, `.about-text`, `.about-visual`, `.contact-info`, and `.map-wrap` is observed. When entering the viewport at 10% visibility (with a -40px bottom margin to prevent premature trigger), the `visible` class is applied, transitioning the element from `opacity: 0; transform: translateY(24px)` to its natural position.

---

## 🎨 Design System

All visual tokens are defined as **CSS custom properties** in `:root`.

### Color Palette

| Token | Value | Usage |
|---|---|---|
| `--green-deep` | `#080f0a` | Hero bg, footer, dark sections |
| `--green-dark` | `#0d1a10` | Experience section, featured card |
| `--green-mid` | `#162b1c` | Card backgrounds |
| `--green-card` | `#1c3524` | Card hover states |
| `--gold` | `#c9a84c` | Primary accent, CTAs, icons |
| `--gold-light` | `#e2c97e` | Hero italic text, light accent |
| `--gold-dim` | `rgba(201,168,76,0.15)` | Borders, dividers |
| `--cream` | `#faf7f0` | About, menu section backgrounds |
| `--cream-dark` | `#f2ede2` | Testimonials section |
| `--text-dark` | `#0d1a10` | Body text on light backgrounds |
| `--text-muted` | `#5c6e60` | Secondary body text |
| `--whatsapp` | `#25d366` | WhatsApp CTA button |

### Typography

| Role | Font | Weight | Size |
|---|---|---|---|
| Display / Headings | Cormorant Garamond | 600–700 | `clamp(3.5rem, 8vw, 6.5rem)` |
| Body / UI | Outfit | 300–600 | 0.78rem – 1.05rem |
| Section Tags | Outfit | 600 | 0.7rem, 3.5px tracking |

### Spacing & Radius

```css
--radius:    12px;   /* Cards */
--radius-lg: 20px;   /* Image frames, contact panel */
section { padding: 100px 0; }
.container { max-width: 1120px; padding: 0 2rem; }
```

### Button Variants

| Class | Style | Use Case |
|---|---|---|
| `.btn-gold` | Solid gold | Primary CTA |
| `.btn-ghost` | Frosted glass border | Hero secondary CTA |
| `.btn-whatsapp` | WhatsApp green | Reservation |
| `.btn-outline-dark` | Gold border, transparent | Secondary actions |

---

## 📱 Responsive Design

Three layout tiers are implemented:

### Desktop — `> 900px`
- About: 2-column grid (`1fr 1fr`)
- Menu: 2×2 grid
- Experience: 4-column horizontal panel
- Testimonials: 3-column grid
- Contact: Split panel (`1fr 1.2fr`)

### Tablet — `≤ 900px`
- Experience: 2-column grid
- About: Single column, image aspect ratio `16/9`
- Testimonials & Contact: Single column

### Mobile — `≤ 768px`
- Full mobile nav overlay replaces horizontal links
- Hero headline scaled to `3rem`
- Hero CTAs stacked vertically
- Stats section stacked vertically
- Experience grid collapses to single column
- Footer stacked and centred
- `background-attachment: scroll` applied (fixes iOS parallax bug)

---

## 📲 WhatsApp & Maps Integration

### WhatsApp Deep Link

The reservation flow bypasses a traditional contact form entirely in favour of a **direct WhatsApp conversation** — a proven high-conversion pattern for hospitality businesses in India.

```html
<!-- Hero CTA -->
<a href="https://wa.me/919999999999?text=Hi%2C%20I'd%20like%20to%20reserve%20a%20table%20at%20Noir%20%26%20Brew."
   class="btn btn-ghost" target="_blank">
  Reserve on WhatsApp
</a>

<!-- Contact Section -->
<a href="https://wa.me/919999999999?text=Hi%2C%20I'd%20like%20to%20know%20more%20about%20Noir%20%26%20Brew."
   class="btn btn-whatsapp" target="_blank">
  WhatsApp Us
</a>
```

**Implementation details:**
- Uses the `wa.me` short URL format for universal mobile/desktop compatibility
- Pre-filled message text is URL-encoded to reduce friction
- `target="_blank"` opens in WhatsApp app (mobile) or WhatsApp Web (desktop)

### Google Maps Embed

```html
<iframe
  src="https://www.google.com/maps/embed?pb=..."
  width="100%" height="100%"
  style="border:0;" allowfullscreen loading="lazy">
</iframe>
```

- `loading="lazy"` defers map load until the contact section enters the viewport
- `allowfullscreen` enables full-screen map view on supported devices
- The wrapper div `min-height: 400px` ensures consistent map display across viewports

---

## 🧗 Challenges & Learnings

### 1. Parallax on iOS
`background-attachment: fixed` causes rendering issues on iOS Safari — it disables the parallax effect and creates visual glitches. This was solved by wrapping the property in a media query override:
```css
@media (max-width: 768px) {
  .hero { background-attachment: scroll; }
}
```

### 2. Intersection Observer Timing
Early implementation fired all animations simultaneously on page load because elements were already partially in the viewport. The `rootMargin: '0px 0px -40px 0px'` setting was added to ensure only elements well within the viewport trigger, creating a more natural staggered reveal.

### 3. Glassmorphism Navbar Contrast
Pure `backdrop-filter: blur()` without sufficient background opacity can fail WCAG contrast requirements on bright sections. The scrolled state uses `rgba(8,15,10,0.94)` opacity to maintain readable nav links at all scroll positions.

### 4. Marquee Infinite Loop
A seamless infinite marquee requires the track to contain **two identical sets** of content. When the animation reaches `-50%` translateX (the end of the first set), it resets to `0` — creating a seamless loop without JavaScript.

---

## 🔭 Future Improvements

- [ ] **Menu page** — full menu with filtering by category (Coffee / Food / Cold)
- [ ] **Online reservation form** — date/time picker with basic validation
- [ ] **Gallery section** — masonry photo grid with lightbox
- [ ] **Dark mode toggle** — system-preference detection + manual override
- [ ] **AOS library replacement** — replace Intersection Observer with Web Animations API for more control
- [ ] **PWA support** — service worker + manifest for offline capability
- [ ] **Accessibility audit** — ARIA labels, focus management, keyboard nav testing
- [ ] **Page speed optimisation** — critical CSS inlining, font subsetting, image WebP conversion
- [ ] **Blog / Journal section** — coffee origin stories and brewing guides
- [ ] **Loyalty programme page** — stamp card system with QR code

---

## 👨‍💻 Author

<div align="center">

**Dev Choudhary**

Frontend Developer · Pune, India

[![GitHub](https://img.shields.io/badge/GitHub-devv0311-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/devv0311)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-c9a84c?style=for-the-badge&logo=firefoxbrowser&logoColor=white)](https://portfolio-devch.netlify.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dev-choudhary-168355394/)

</div>

---

<div align="center">

*This project is part of a frontend portfolio series. It simulates a real client brief for a premium café brand and demonstrates production-level HTML/CSS/JS skills without any frameworks or build tools.*

<br/>

**If you found this project useful, consider leaving a ⭐**

<br/>

```
✦  N O I R  &  B R E W  ·  K O R E G A O N  P A R K  ·  P U N E  ✦
```

</div>