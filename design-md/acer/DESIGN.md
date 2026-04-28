# Acer Design System

> Accessible performance technology with sharp retail clarity. Acer's current public site combines deep charcoal framing, bright green accents, white commerce surfaces, and product-family storytelling around AI PCs, gaming, business, and sustainability, creating a tech storefront that feels energetic, broad, and easy to browse.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Acer feels like **mass-market computing presented through fast product merchandising**. The system balances mainstream retail energy with product-family identity. AI PCs, gaming hardware, business devices, and sustainable lines all sit inside one sharp, high-contrast visual language.

### Mood & Feeling
- Fast and practical
- Product-led and category-rich
- Accessible rather than luxurious
- Modern, energetic, and browse-friendly
- Broad in scope without losing scanability

### Design Density
**Medium density.** Acer shows many categories, offers, and campaigns, but keeps them readable through strong card blocks, obvious product rails, and bold contrast between sections.

### Visual Character
- Dark charcoal and black support surfaces
- Bright Acer green as the core action and identity accent
- White product and promo cards on retail-like grids
- Strong category segmentation for gaming, business, and AI PCs
- Utility-first banners, offers, and campaign tiles

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--acer-black` | `#111111` | Deep contrast sections and navigation |
| `--acer-charcoal` | `#1E1E1E` | Secondary dark surfaces |
| `--acer-white` | `#FFFFFF` | Main canvas and cards |
| `--acer-surface` | `#F5F6F8` | Light section background |
| `--acer-text` | `#1F2937` | Primary body text |

### Brand and Support

| Token | Hex | Role |
|-------|-----|------|
| `--acer-green` | `#83B81A` | Primary brand accent and CTA support |
| `--acer-green-deep` | `#6B9815` | Hover and active state |
| `--acer-green-soft` | `#EEF6D8` | Light callout fill |
| `--acer-border` | `#D7DDE5` | Card borders and dividers |
| `--acer-muted` | `#6B7280` | Secondary text |

### Utility

| Token | Hex | Role |
|-------|-----|------|
| `--acer-success` | `#148A58` | Positive product or support state |
| `--acer-warning` | `#BE7B00` | Warning state |
| `--acer-danger` | `#D14343` | Error or critical notice |
| `--acer-focus` | `#CDE88B` | Focus ring tint |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Acer Foco", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Acer Foco", system-ui, -apple-system, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 68px | 700 | 1.02 | -0.03em | `#111111` |
| Page Title | 48px | 700 | 1.08 | -0.02em | `#111111` |
| Section Title | 34px | 700 | 1.12 | -0.015em | `#111111` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#1F2937` |
| Body Large | 18px | 400 | 1.6 | 0 | `#1F2937` |
| Body | 16px | 400 | 1.6 | 0 | `#1F2937` |
| Small Body | 14px | 400 | 1.45 | 0 | `#6B7280` |
| Label | 12px | 700 | 1.3 | 0.04em | `#6B7280` |

### Typography Philosophy
Acer typography should feel **clear, commercial, and performance-aware**. Headlines need enough presence for launches and promos, but the system must stay easy to scan across a broad product catalog.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #83b81a;
  color: #111111;
  border: none;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
  font-size: 16px;
  font-weight: 700;
}

.button-primary:hover {
  background: #6b9815;
  color: #ffffff;
}

.button-secondary {
  background: #ffffff;
  color: #111111;
  border: 1px solid #d7dde5;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
}
```

### Cards and Product Tiles

```css
.product-card {
  background: #ffffff;
  border: 1px solid #d7dde5;
  border-radius: 20px;
  box-shadow: 0 14px 28px rgba(17, 17, 17, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #1f2937;
  border: 1px solid #d7dde5;
  border-radius: 14px;
  min-height: 48px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #83b81a;
  box-shadow: 0 0 0 4px rgba(205, 232, 139, 0.42);
}
```

### Component Notes
- Product-family cards should be easy to compare and browse quickly
- Promotions and offers can be bold, but should stay contained within clean card or banner shells
- Sustainability and AI messaging should feel integrated into the product lineup, not like a separate brand

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight alignment |
| `--space-3` | `8px` | Small gaps |
| `--space-4` | `12px` | Compact internal spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card interiors |
| `--space-7` | `32px` | Module grouping |
| `--space-8` | `48px` | Section rhythm |
| `--space-9` | `64px` | Hero spacing |
| `--space-10` | `96px` | Large campaign and category sections |

### Layout Behavior
- Organize by product family and buyer intent: AI PCs, gaming, business, accessories, sustainability
- Use broad hero campaigns followed by category rails and offer blocks
- Keep retail actions obvious and low-friction
- Mix product imagery, merchandising copy, and utility links without clutter

### Whitespace Philosophy
Whitespace should feel **commercially efficient**, leaving enough room to scan offers and product families without making the page feel crowded or bargain-bin noisy.

---

## 6. Depth & Elevation

### Elevation Strategy
Acer uses **light retail-tech elevation**. Cards float gently off pale surfaces, while dark section framing and green highlights provide the stronger depth signals.

```css
--shadow-soft: 0 8px 18px rgba(17, 17, 17, 0.04);
--shadow-card: 0 14px 28px rgba(17, 17, 17, 0.08);
--shadow-focus: 0 0 0 4px rgba(205, 232, 139, 0.42);
```

### Surface Hierarchy
- White base and product cards
- Pale gray support sections
- Dark charcoal category or nav framing
- Green CTA and accent moments for product emphasis

---

## 7. Do's and Don'ts

### Do
- Keep Acer browseable, energetic, and product-family aware
- Use green as a clear identity and action signal
- Let product categories and offers stay obvious
- Preserve contrast between retail, gaming, business, and sustainability narratives

### Don't
- Do not make Acer feel like ultra-luxury minimal hardware branding
- Do not bury key products under abstract marketing copy
- Do not overcomplicate retail flows with too many visual effects
- Do not let promos overwhelm product clarity

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked hero campaigns, single-column product rails, clear offer tiles |
| Tablet | `768px - 1023px` | Two-column category and merchandising grids |
| Desktop | `1024px+` | Broad retail-tech storytelling, category hubs, and multi-tile product sections |

### Responsive Rules
- Preserve category clarity when product grids collapse
- Keep CTAs and price/offer messaging readable on mobile
- Stack related campaign and promo cards before shrinking type too far
- Maintain visible separation between dark framing and light content cards

---

## 9. Agent Prompt Guide

### Quick Reference
- Charcoal and white structure with bright Acer green accents
- Retail-tech product browsing, category cards, and promo blocks
- Rounded product tiles, clear offer hierarchy, and mainstream performance framing
- Fast, accessible, and catalog-friendly rather than premium-minimal

### Prompt Template
```text
Design this like Acer's current public website:
- charcoal framing with white product cards and bright green action accents
- broad AI PC, gaming, business, and sustainability category rails
- rounded retail-tech product tiles with clean merchandising copy
- practical, fast product-browsing energy with clear offers and CTAs
- accessible performance-computing feel rather than luxury hardware minimalism
```
