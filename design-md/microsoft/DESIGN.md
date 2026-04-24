# Microsoft Design System

> Broad computing and productivity ecosystem with Fluent-driven clarity. Microsoft's current public site combines `Segoe UI Variable`, `Segoe UI`, and product-specific illustration gradients with a bright white foundation, soft gray surfaces, dark neutral text, and the familiar Microsoft blue (`#0067B8`) supported by multi-product accent colors.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Microsoft feels like **a massive product ecosystem organized through calm, modern utility**. The experience balances enterprise trust, consumer approachability, and a quietly polished interface language rooted in Fluent principles.

### Mood & Feeling
- Practical and confident
- Broad but well-structured
- Friendly enterprise utility
- Clean, modern, and scalable
- Product-family driven rather than single-brand theatrical

### Design Density
**Medium density.** Microsoft surfaces carry many product categories, but cards, tiles, and whitespace keep the layout manageable.

### Visual Character
- Bright white page shells
- Soft gray and pale-tinted support surfaces
- Modular product tiles and promo cards
- Blue-led action hierarchy
- Gentle gradients and ribbon-like illustrations for AI and cloud content

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--ms-white` | `#FFFFFF` | Main canvas and cards |
| `--ms-gray-050` | `#F5F5F5` | Soft section background |
| `--ms-gray-100` | `#F2F2F2` | Secondary fills |
| `--ms-ink` | `#1A1A1A` | Primary text |
| `--ms-muted` | `#616161` | Secondary copy |

### Brand and Product Accent

| Token | Hex | Role |
|-------|-----|------|
| `--ms-blue` | `#0067B8` | Primary link and CTA accent |
| `--ms-blue-bright` | `#0078D4` | Hover and Fluent action blue |
| `--ms-teal` | `#00B7C3` | AI/cloud support accent |
| `--ms-green` | `#107C10` | Xbox/product support accent |
| `--ms-violet` | `#8661C5` | Copilot and premium support accents |

### Structure Tokens

| Token | Hex | Role |
|-------|-----|------|
| `--ms-border` | `#D1D1D1` | Dividers and tile edges |
| `--ms-surface` | `#FAFAFA` | Light elevated panel fill |
| `--ms-focus` | `rgba(0, 120, 212, 0.18)` | Focus ring glow |

---

## 3. Typography Rules

### Font Stack

```css
--font-sans: "Segoe UI Variable", "Segoe UI", "Helvetica Neue", Arial, sans-serif;
--font-display: "Segoe UI Variable Display", "Segoe UI Variable", "Segoe UI", sans-serif;
--font-mono: "Cascadia Code", "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 60px | 600 | 1.05 | -0.03em | `#1A1A1A` |
| Page Title | 44px | 600 | 1.08 | -0.02em | `#1A1A1A` |
| Section Title | 32px | 600 | 1.14 | -0.01em | `#1A1A1A` |
| Card Title | 22px | 600 | 1.2 | -0.01em | `#1A1A1A` |
| Body Large | 18px | 400 | 1.55 | 0 | `#1A1A1A` |
| Body | 16px | 400 | 1.6 | 0 | `#1A1A1A` |
| Small Body | 14px | 400 | 1.5 | 0 | `#616161` |
| Label | 12px | 600 | 1.35 | 0.04em | `#616161` |

### Typography Philosophy
Microsoft typography should feel **clear, adaptable, and product-system oriented**. It should support many product stories without becoming visually loud or decorative.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #0067b8;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #0078d4;
}

.button-secondary {
  background: #ffffff;
  color: #1a1a1a;
  border: 1px solid #d1d1d1;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Tiles and Promo Cards

```css
.tile {
  background: #ffffff;
  border: 1px solid #d1d1d1;
  border-radius: 20px;
  box-shadow: 0 10px 24px rgba(0, 0, 0, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #1a1a1a;
  border: 1px solid #d1d1d1;
  border-radius: 12px;
  min-height: 44px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #0078d4;
  box-shadow: 0 0 0 4px rgba(0, 120, 212, 0.18);
}
```

### Component Notes
- Product promos should feel modular and ecosystem-aware
- Buttons are polished but restrained
- AI and cloud moments can support more gradient color than default commerce rows

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Fine alignment |
| `--space-3` | `8px` | Tight UI rhythm |
| `--space-4` | `12px` | Compact paddings |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card spacing |
| `--space-7` | `32px` | Major module gaps |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero structure |

### Layout Behavior
- Group content by product family and use case
- Use clean rows of promo tiles and product features
- Let broad ecosystem navigation stay visually stable across sections
- Use illustration gradients sparingly to avoid overpowering utility content

### Whitespace Philosophy
Whitespace should feel **organized and helpful**, giving a very large product ecosystem enough room to remain scannable.

---

## 6. Depth & Elevation

### Elevation Strategy
Microsoft uses **soft Fluent-style elevation**. Cards lift lightly, and contrast between white, gray, and tinted surfaces does much of the structural work.

```css
--shadow-soft: 0 8px 20px rgba(0, 0, 0, 0.05);
--shadow-card: 0 16px 32px rgba(0, 0, 0, 0.08);
```

### Surface Hierarchy
- White base canvas
- Soft-gray background bands
- Elevated white product cards
- Occasional gradient-backed highlight modules

---

## 7. Do's and Don'ts

### Do
- Keep the system clear, scalable, and product-family aware
- Use blue as the stable action anchor
- Let gradients and ribbons support AI or cloud storytelling, not everything
- Preserve strong readability for enterprise and consumer audiences

### Don't
- Do not make Microsoft feel sterile or outdated
- Do not overfill the page with competing product accents
- Do not collapse large navigation structures into visual clutter
- Do not turn every section into a loud marketing hero

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked promos and condensed category navigation |
| Tablet | `768px - 1023px` | Two-column product tiles with reduced promo density |
| Desktop | `1024px+` | Full multi-row ecosystem browsing and wide promo panels |

### Responsive Rules
- Preserve discoverability for product categories
- Stack large promo cards before shrinking copy too far
- Keep CTAs obvious and touchable
- Maintain clear card grouping when grids collapse

---

## 9. Agent Prompt Guide

### Quick Reference
- White, soft gray, and Microsoft blue foundation
- Fluent-style modular cards and calm enterprise-consumer utility
- Segoe UI Variable style typography and restrained gradients
- Broad ecosystem clarity with polished product promo tiles

### Prompt Template
```text
Design this like Microsoft's current public website:
- white and soft-gray Fluent-style layout foundation
- Microsoft blue actions with occasional AI/cloud gradient support
- Segoe UI Variable-like typography and modular product tiles
- broad but organized ecosystem navigation and promo rows
- practical, modern, scalable product-system energy
```
