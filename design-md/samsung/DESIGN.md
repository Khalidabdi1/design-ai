# Samsung Design System

> Consumer electronics with premium hardware polish and broad product merchandising. Samsung's public site blends `Samsung Sharp Sans` with `SamsungOne`, using a black-and-white foundation, cool grays, brand blue highlights, and large product-stage imagery for phones, TVs, appliances, and accessories.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Samsung feels like **premium electronics retail at ecosystem scale**. The visual system is sleek and product-centric, but also flexible enough to support phones, TVs, home appliances, and accessories in one consistent frame.

### Mood & Feeling
- Premium and high-tech
- Broad but polished
- Product-led and aspirational
- Confident consumer electronics energy
- Clean and globally scalable

### Design Density
**Medium density.** Samsung supports many departments and promo modules, but large imagery and clean typography keep the site from feeling cramped.

### Visual Character
- Crisp black-and-white product framing
- Cool gray section backgrounds
- Large product hero stages
- Modest use of cobalt/blue product accents
- Promotional banners with strong merchandising cadence

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--samsung-black` | `#000000` | Hero framing, text, CTA |
| `--samsung-white` | `#FFFFFF` | Main canvas and cards |
| `--samsung-gray-050` | `#F7F7F7` | Soft background |
| `--samsung-gray-200` | `#E6E6E6` | Borders and dividers |
| `--samsung-muted` | `#666666` | Secondary text |

### Brand and Product Accent

| Token | Hex | Role |
|-------|-----|------|
| `--samsung-blue` | `#1428A0` | Brand anchor and links |
| `--samsung-blue-bright` | `#0B5FFF` | Stronger interaction blue |
| `--samsung-silver` | `#C9CDD4` | Premium hardware tint support |
| `--samsung-success` | `#12805C` | Positive state |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Samsung Sharp Sans", "Helvetica Neue", Arial, sans-serif;
--font-sans: "SamsungOne", "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 60px | 700 | 1.03 | -0.03em | `#000000` |
| Page Title | 44px | 700 | 1.08 | -0.02em | `#000000` |
| Section Title | 32px | 700 | 1.12 | -0.01em | `#000000` |
| Card Title | 22px | 600 | 1.2 | -0.01em | `#000000` |
| Body Large | 18px | 400 | 1.55 | 0 | `#000000` |
| Body | 16px | 400 | 1.55 | 0 | `#000000` |
| Small Body | 14px | 400 | 1.45 | 0 | `#666666` |
| Label | 12px | 600 | 1.35 | 0.05em | `#666666` |

### Typography Philosophy
Samsung typography should feel **sharp, premium, and modern**, with display moments that support product aspiration and body text that stays highly usable.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #000000;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #222222;
}

.button-secondary {
  background: #ffffff;
  color: #000000;
  border: 1px solid #e6e6e6;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Product Cards

```css
.product-card {
  background: #ffffff;
  border: 1px solid #e6e6e6;
  border-radius: 20px;
  overflow: hidden;
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #000000;
  border: 1px solid #e6e6e6;
  border-radius: 12px;
  min-height: 44px;
  padding: 12px 14px;
}
```

### Component Notes
- Hardware visuals should dominate product sections
- Buttons should stay premium and understated
- Use blue as a brand signal, not a default surface fill

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Dense retail alignment |
| `--space-3` | `8px` | Tight spacing |
| `--space-4` | `12px` | Compact internal rhythm |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card spacing |
| `--space-7` | `32px` | Product shelf separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero stages |

### Layout Behavior
- Use wide product heroes to showcase hardware form
- Support broad category navigation without making it feel cluttered
- Let merchandising modules remain highly scannable
- Separate product families with clear visual bands

### Whitespace Philosophy
Whitespace should feel **premium and merchandising-aware**, balancing product aspiration with retail utility.

---

## 6. Depth & Elevation

### Elevation Strategy
Samsung uses **light premium-ecommerce elevation**. Most depth comes from product rendering, clean cards, and restrained shadows.

```css
--shadow-soft: 0 8px 18px rgba(0, 0, 0, 0.05);
--shadow-card: 0 14px 30px rgba(0, 0, 0, 0.08);
```

### Surface Hierarchy
- White and cool-gray base
- Elevated product cards
- Dark CTA anchors
- Blue for links and product branding support

---

## 7. Do's and Don'ts

### Do
- Keep the system sleek and hardware-forward
- Use sharp typography and strong product imagery
- Preserve a premium black-white foundation
- Keep category breadth organized and legible

### Don't
- Do not make Samsung look like generic low-cost retail
- Do not overuse blue or gradients as full backgrounds
- Do not crowd hero sections with too much secondary copy
- Do not use playful soft-app styling for hardware commerce

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked product stages and swipeable merchandising rows |
| Tablet | `768px - 1023px` | Wider cards with split product promos |
| Desktop | `1024px+` | Full premium hardware heroes and broad category merchandising |

### Responsive Rules
- Keep product imagery dominant on mobile
- Simplify category navigation before shrinking copy excessively
- Preserve CTA clarity and card grouping
- Maintain generous image ratios for flagship products

---

## 9. Agent Prompt Guide

### Quick Reference
- Premium electronics retail with black, white, cool gray, and Samsung blue
- Sharp Sans-style display and SamsungOne-style body typography
- Hardware-led hero stages and polished product cards
- Broad ecosystem merchandising without visual chaos

### Prompt Template
```text
Design this like Samsung's current public website:
- premium consumer-electronics retail foundation in black, white, and cool gray
- sharp display typography with clean SamsungOne-style UI text
- large hardware-led hero visuals and polished rounded product cards
- modest Samsung-blue brand accents for links and product support
- sleek, broad ecosystem merchandising with premium restraint
```
