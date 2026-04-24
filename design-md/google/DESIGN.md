# Google Design System

> High-clarity product ecosystem with Material influence and playful restraint. Google's public brand surfaces pair `Google Sans` with `Roboto`, white backgrounds, soft gray section fills, and the multicolor brand system of blue (`#4285F4`), red (`#EA4335`), yellow (`#FBBC05`), and green (`#34A853`).

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Google feels like **high-scale product infrastructure made approachable through softness, clarity, and color precision**. The system is lightweight and optimistic, but never messy.

### Mood & Feeling
- Helpful and intelligent
- Bright, clean, and approachable
- Product-ecosystem driven
- Technically advanced without looking severe
- Playful in controlled ways

### Design Density
**Medium density.** Google shows many products, initiatives, and AI stories, but uses large cards, airy spacing, and familiar color logic to stay readable.

### Visual Character
- White surfaces with light gray section bands
- Large rounded cards and media blocks
- Blue-led links with multicolor brand accents
- Material-inspired spacing and shape logic
- Friendly editorial and product storytelling

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--google-white` | `#FFFFFF` | Primary canvas and cards |
| `--google-gray-050` | `#F8F9FA` | Soft page background |
| `--google-gray-100` | `#F1F3F4` | Secondary fills |
| `--google-ink` | `#202124` | Primary text |
| `--google-muted` | `#5F6368` | Secondary copy |

### Brand Accent System

| Token | Hex | Role |
|-------|-----|------|
| `--google-blue` | `#4285F4` | Links and primary actions |
| `--google-red` | `#EA4335` | Highlight and alert accent |
| `--google-yellow` | `#FBBC05` | Warm emphasis and brand support |
| `--google-green` | `#34A853` | Success and supportive brand accent |
| `--google-blue-deep` | `#1A73E8` | Stronger interaction blue |

### Structure Tokens

| Token | Hex | Role |
|-------|-----|------|
| `--google-border` | `#DADCE0` | Card and divider stroke |
| `--google-focus` | `rgba(26, 115, 232, 0.18)` | Focus treatment |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Google Sans", "Product Sans", Arial, sans-serif;
--font-sans: "Google Sans", "Roboto", Arial, sans-serif;
--font-mono: "Roboto Mono", "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 56px | 500 | 1.08 | -0.02em | `#202124` |
| Page Title | 44px | 500 | 1.1 | -0.015em | `#202124` |
| Section Title | 32px | 500 | 1.15 | -0.01em | `#202124` |
| Card Title | 24px | 500 | 1.22 | -0.01em | `#202124` |
| Body Large | 18px | 400 | 1.6 | 0 | `#202124` |
| Body | 16px | 400 | 1.6 | 0 | `#202124` |
| Small Body | 14px | 400 | 1.5 | 0 | `#5F6368` |
| Label | 12px | 500 | 1.35 | 0.03em | `#5F6368` |

### Typography Philosophy
Google typography should feel **clear, friendly, and quietly advanced**. Use rounded, readable type with strong hierarchy but avoid unnecessary drama.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #1a73e8;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 14px;
  font-weight: 500;
}

.button-primary:hover {
  background: #1765cc;
}

.button-secondary {
  background: #ffffff;
  color: #1a73e8;
  border: 1px solid #dadce0;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Cards and Story Panels

```css
.card {
  background: #ffffff;
  border: 1px solid #dadce0;
  border-radius: 28px;
  box-shadow: 0 8px 20px rgba(60, 64, 67, 0.08);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #202124;
  border: 1px solid #dadce0;
  border-radius: 12px;
  min-height: 44px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #1a73e8;
  box-shadow: 0 0 0 4px rgba(26, 115, 232, 0.18);
}
```

### Component Notes
- Large rounded cards are preferred over hard-edged boxes
- Multicolor accents should usually appear as highlights, icons, or art support
- Base UI should still feel calm and mostly neutral

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Dense UI alignment |
| `--space-3` | `8px` | Tight component rhythm |
| `--space-4` | `12px` | Compact spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card interiors |
| `--space-7` | `32px` | Module separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and editorial blocks |

### Layout Behavior
- Use large media-backed cards for product and research stories
- Keep content groupings highly scannable
- Let white space and rounded shapes soften complex technical content
- Maintain a stable neutral frame even when multiple product stories coexist

### Whitespace Philosophy
Whitespace should feel **generous and helpful**, reducing cognitive load and making advanced topics feel approachable.

---

## 6. Depth & Elevation

### Elevation Strategy
Google uses **Material-like soft elevation** with subtle shadows and clear container boundaries.

```css
--shadow-soft: 0 6px 16px rgba(60, 64, 67, 0.08);
--shadow-card: 0 12px 28px rgba(60, 64, 67, 0.12);
```

### Surface Hierarchy
- White base
- Pale gray section bands
- Rounded elevated cards
- Multicolor accents and illustrations as supporting structure

---

## 7. Do's and Don'ts

### Do
- Keep the system clear, human, and highly readable
- Use brand colors with discipline
- Prefer rounded, friendly containers
- Balance technical sophistication with low-friction presentation

### Don't
- Do not saturate every interface area with the four brand colors
- Do not harden the UI into severe enterprise minimalism
- Do not make advanced technology pages feel cold or intimidating
- Do not overcomplicate card layouts or reduce whitespace too aggressively

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked cards, reduced hero width, simplified nav |
| Tablet | `768px - 1023px` | Two-column editorial and product modules |
| Desktop | `1024px+` | Full multi-card story layouts and product overview groupings |

### Responsive Rules
- Preserve readable rounded cards on mobile
- Reduce visual complexity before reducing text legibility
- Keep primary CTAs easy to locate on content-heavy pages
- Maintain consistent rhythm between product and editorial sections

---

## 9. Agent Prompt Guide

### Quick Reference
- White and light-gray Material-style foundation
- Google Sans / Roboto feel with rounded card containers
- Blue-led actions and restrained red/yellow/green accents
- Friendly, intelligent, approachable product-system presentation

### Prompt Template
```text
Design this like Google's current public brand surfaces:
- white and soft-gray Material-influenced layout foundation
- Google Sans / Roboto-like typography with generous rounded cards
- blue-first actions with restrained multicolor brand accents
- intelligent but approachable product and AI storytelling
- clean, helpful, high-clarity ecosystem design
```
