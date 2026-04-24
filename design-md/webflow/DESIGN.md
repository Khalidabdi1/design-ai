# Webflow Design System

> Visual website building with premium black-and-white structure and electric blue product energy. Webflow's current public site pairs a sharp sans-serif system with black, white, bright electric blue (`#146EF5`), and high-contrast product imagery for designers, marketers, developers, and agencies.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Webflow feels like **serious web creation software with a polished creative-tech edge**. The system is premium, crisp, and confident, balancing technical power with visually refined marketing.

### Mood & Feeling
- Creative but disciplined
- Modern and premium
- Confident product sophistication
- Builder-focused rather than lifestyle-focused
- Sharp, intentional, and slightly futuristic

### Design Density
**Medium density.** Webflow surfaces often contain a lot of capability messaging, but the design keeps things elegant through strong contrast, bounded modules, and clean typography.

### Visual Character
- Black and white structural frame
- Bright blue action and product accent
- Sharp, high-resolution product imagery
- Modern, premium SaaS composition
- Optional light/dark mode framing and tooling cues

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--webflow-black` | `#0A0A0A` | Hero framing, text, strong contrast |
| `--webflow-white` | `#FFFFFF` | Base surface and cards |
| `--webflow-surface` | `#F7F8FA` | Light section fill |
| `--webflow-ink` | `#111827` | Primary text |
| `--webflow-muted` | `#667085` | Secondary copy |

### Brand and Product Accent

| Token | Hex | Role |
|-------|-----|------|
| `--webflow-blue` | `#146EF5` | Primary action and brand anchor |
| `--webflow-blue-bright` | `#4353FF` | Stronger gradient or hover support |
| `--webflow-blue-soft` | `#E8F0FF` | Soft brand tint |
| `--webflow-border` | `#E5E7EB` | Card edges and dividers |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, -apple-system, sans-serif;
--font-mono: "Roboto Mono", "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 64px | 700 | 1.02 | -0.03em | `#0A0A0A` |
| Page Title | 48px | 700 | 1.06 | -0.02em | `#0A0A0A` |
| Section Title | 34px | 700 | 1.12 | -0.02em | `#0A0A0A` |
| Card Title | 24px | 600 | 1.2 | -0.01em | `#111827` |
| Body Large | 18px | 400 | 1.6 | 0 | `#111827` |
| Body | 16px | 400 | 1.6 | 0 | `#111827` |
| Small Body | 14px | 400 | 1.5 | 0 | `#667085` |
| Label | 12px | 700 | 1.35 | 0.04em | `#667085` |

### Typography Philosophy
Webflow typography should feel **sharp, premium, and digitally native**. It should support high-end product marketing without losing practical builder clarity.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #146ef5;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 46px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #0f5bd0;
}

.button-secondary {
  background: #ffffff;
  color: #0a0a0a;
  border: 1px solid #e5e7eb;
  border-radius: 999px;
  min-height: 46px;
  padding: 0 20px;
}
```

### Product Cards

```css
.product-card {
  background: #ffffff;
  border: 1px solid #e5e7eb;
  border-radius: 24px;
  box-shadow: 0 14px 30px rgba(17, 24, 39, 0.08);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #111827;
  border: 1px solid #e5e7eb;
  border-radius: 14px;
  min-height: 46px;
  padding: 12px 14px;
}
```

### Component Notes
- Product screenshots should feel premium and high fidelity
- Electric blue belongs on CTAs, logos, and specific highlights
- Builder controls can be dense, but surrounding marketing should stay elegant

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight alignment |
| `--space-3` | `8px` | Small UI rhythm |
| `--space-4` | `12px` | Compact spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card spacing |
| `--space-7` | `32px` | Module separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and demo blocks |

### Layout Behavior
- Use strong hero proof and premium builder screenshots
- Group stories by audience: marketer, designer, developer, agency
- Allow contrast-rich black sections to punctuate the lighter layout
- Keep page rhythm clean and intentional

### Whitespace Philosophy
Whitespace should feel **premium and creative-tech**, leaving room for product sophistication and strong visual confidence.

---

## 6. Depth & Elevation

### Elevation Strategy
Webflow uses **premium SaaS elevation** with crisp cards, high-fidelity imagery, and stronger contrast than typical enterprise tools.

```css
--shadow-soft: 0 8px 18px rgba(17, 24, 39, 0.06);
--shadow-card: 0 18px 36px rgba(17, 24, 39, 0.10);
```

### Surface Hierarchy
- White base
- Black contrast sections
- Electric blue action points
- Elevated demo cards and media frames

---

## 7. Do's and Don'ts

### Do
- Keep Webflow visually sharp and premium
- Use black-white contrast with disciplined electric blue accents
- Let product screenshots look advanced and high fidelity
- Preserve audience-based information architecture

### Don't
- Do not soften Webflow into generic rounded startup UI
- Do not overuse blue as a full-page background
- Do not clutter product demos with low-signal copy
- Do not lose the creative-tech edge

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked audience sections and simplified demo framing |
| Tablet | `768px - 1023px` | Two-column product modules and compact contrast sections |
| Desktop | `1024px+` | Full premium hero demos and broad audience-based storytelling |

### Responsive Rules
- Keep CTAs and demo previews prominent on mobile
- Preserve the premium image quality of screenshots
- Stack multi-audience content instead of over-compressing it
- Maintain clean rhythm between light and dark sections

---

## 9. Agent Prompt Guide

### Quick Reference
- Premium black-white builder foundation with electric Webflow blue
- Sharp modern sans typography and high-fidelity demo cards
- Audience-based product storytelling for marketers, designers, and developers
- Creative-tech polish with strong contrast and elegant spacing

### Prompt Template
```text
Design this like Webflow's current public website:
- premium black-and-white site-builder foundation
- electric Webflow-blue CTAs and selective accent highlights
- sharp modern typography with high-fidelity product screenshots
- creative-tech SaaS polish for marketers, designers, developers, and agencies
- elegant contrast, intentional spacing, and confident builder-tool energy
```
