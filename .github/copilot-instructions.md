---
applyTo: '**'
---
# Copilot Instructions for `eshophome05dec`

## 1. Project Context
- This repo is a **static e‑commerce landing page** called **eShop Home**.
- Primary artifacts should be:
  - `index.html` (root or `src/`),
  - `css/index.css` (or similar),
  - `js/index.js` (or similar),
  - supporting assets (icons, images, favicon).
- Design language: **sky‑blue theme**, **glassmorphism**, **modern, clean layout**.
- README already contains **CDD (Comment Driven Development)** examples – keep them consistent.

## 2. Technology & Libraries
- Use **vanilla HTML/CSS/JS** only (no frameworks unless explicitly requested).
- Styling:
  - Prefer **Tailwind CSS via CDN** *plus* light custom CSS for glassmorphism.
  - Do not introduce complex build steps (no PostCSS/webpack/Vite) unless the user asks.
- Icons: **Font Awesome 6.x** via CDN.
- Fonts: **Google Fonts – Roboto**.

## 3. Coding Style & Structure
- Keep the project **single‑page** unless the user requests routing or multiple views.
- Organize sections roughly as:
  1. Sticky navbar
  2. Hero section with CTA
  3. Feature/services grid
  4. Product showcase grid
  5. (Optional) product data table
  6. Testimonials / trust signals (optional)
  7. Footer + scroll‑to‑top FAB
- Focus on **semantic HTML** (`<header>`, `<main>`, `<section>`, `<nav>`, `<footer>`).
- Ensure **responsive behavior**: mobile‑first layout, sensible breakpoints.
- Favor **small, focused JS functions** for interactions (carousel, smooth scroll, toggles).

## 4. Comment Driven Development (CDD)
- **Respect the CDD workflow**:
  - Start by writing **clear, high‑level comments** describing sections, components, and behaviors.
  - Only then generate the implementation beneath those comments.
- When expanding the UI, follow patterns already used in `README.md`, for example:
  - Section‑level comments: `<!-- SECTION: ... -->`
  - Component‑level comments: `<!-- COMPONENT: ... -->`
  - Behavioral comments in JS: `// CDD: ... Requirements: ... Accessibility: ...`.
- Do **not** remove existing well‑structured comments; extend or refine them when needed.

## 5. UX, Accessibility & Performance
- Ensure basic accessibility:
  - Use **ARIA labels** for nav, buttons, and interactive elements.
  - Provide **keyboard navigation** for menus and carousels.
  - Respect **reduced motion** preferences when adding animations.
- Keep animations **subtle** and **performance‑friendly** (CSS transforms/opacity; avoid layout thrash).
- Optimize for readability: sensible contrast, font sizes, spacing.

## 6. Git & Files
- Do **not** add large binaries or uncompressed assets.
- Prefer **reusable utility classes** (especially with Tailwind) instead of over‑nested custom CSS.
- When adding new files, use **lowercase‑kebab** naming (e.g., `product-card.js`, `hero-section.css`) unless aligning with an existing convention.

## 7. AI Interaction Guidance
- When the user asks for help:
  - First, **infer intent** from the README and existing files.
  - Prefer **small, targeted changes** over sweeping rewrites.
  - Before editing, briefly **summarize the plan** and keep the user’s design language and CDD style in mind.
- Avoid introducing new major technologies (e.g., React, Vue, Tailwind build pipelines) unless **explicitly requested**.

## 8. Documentation
- Keep `README.md` the **single source of truth** for:
  - Project description and features (implemented vs planned),
  - Tech stack,
  - Basic run instructions.
- If you change structure, styling approach, or behavior meaningfully, **update `README.md` accordingly**.
