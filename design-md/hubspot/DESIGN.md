# HubSpot Design System

> CRM and growth software with approachable enterprise warmth. HubSpot's current public site mixes friendly display type with practical UI text, pairing white surfaces with warm neutrals, deep text, and a strong orange-coral brand accent anchored by HubSpot orange (`#FF5C35`).

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
HubSpot feels like **B2B software explained by a friendly, content-savvy brand**. It stays practical enough for CRM workflows while keeping the visual system warm and approachable.

### Mood & Feeling
- Helpful and growth-oriented
- Warm enterprise software
- Friendly but not casual
- Content-rich and approachable
- Modern go-to-market energy

### Design Density
**Medium density.** HubSpot presents many products, teams, and use cases, but uses cards, grouped sections, and approachable tone to keep the experience manageable.

### Visual Character
- White and warm off-white surfaces
- Orange-coral brand emphasis
- Rounded cards and feature blocks
- Clear team/use-case grouping
- Enterprise structure softened by warm palettes and illustration-friendly framing

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--hubspot-orange` | `#FF5C35` | Primary brand and CTA accent |
| `--hubspot-white` | `#FFFFFF` | Main surface and cards |
| `--hubspot-cream` | `#FFF8F4` | Warm background tint |
| `--hubspot-ink` | `#213343` | Primary text |
| `--hubspot-muted` | `#516F90` | Secondary copy |

### Support and Utility

| Token | Hex | Role |
|-------|-----|------|
| `--hubspot-border` | `#D8E1EA` | Card borders and dividers |
| `--hubspot-blue-soft` | `#EAF2FF` | Support tint for product or AI blocks |
| `--hubspot-orange-soft` | `#FFE2D9` | Soft brand tint |
| `--hubspot-success` | `#168A63` | Positive state |
| `--hubspot-focus` | `rgba(255, 92, 53, 0.16)` | Focus ring |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Lexend Deca", "Avenir Next", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Lexend Deca", system-ui, -apple-system, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 60px | 700 | 1.04 | -0.03em | `#213343` |
| Page Title | 44px | 700 | 1.08 | -0.02em | `#213343` |
| Section Title | 32px | 700 | 1.14 | -0.01em | `#213343` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#213343` |
| Body Large | 18px | 400 | 1.6 | 0 | `#213343` |
| Body | 16px | 400 | 1.6 | 0 | `#213343` |
| Small Body | 14px | 400 | 1.5 | 0 | `#516F90` |
| Label | 12px | 700 | 1.35 | 0.04em | `#516F90` |

### Typography Philosophy
HubSpot typography should feel **friendly, confident, and readable at scale**. It should support marketing education, CRM product messaging, and AI features without feeling stiff.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #ff5c35;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
  font-size: 15px;
  font-weight: 700;
}

.button-primary:hover {
  background: #e74c25;
}

.button-secondary {
  background: #ffffff;
  color: #213343;
  border: 1px solid #d8e1ea;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
}
```

### Cards and Feature Blocks

```css
.feature-card {
  background: #ffffff;
  border: 1px solid #d8e1ea;
  border-radius: 24px;
  box-shadow: 0 12px 28px rgba(33, 51, 67, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #213343;
  border: 1px solid #d8e1ea;
  border-radius: 14px;
  min-height: 48px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #ff5c35;
  box-shadow: 0 0 0 4px rgba(255, 92, 53, 0.16);
}
```

### Component Notes
- Product modules should feel practical, not abstract
- Orange is the brand anchor, but the broader layout should stay balanced
- AI features fit naturally into the CRM and content story rather than feeling bolted on

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Fine rhythm |
| `--space-3` | `8px` | Tight spacing |
| `--space-4` | `12px` | Compact controls |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card interiors |
| `--space-7` | `32px` | Module separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero structure |

### Layout Behavior
- Group products by team and outcome
- Use approachable cards and explanatory content blocks
- Support dense product breadth with clean section framing
- Let CTA and proof modules stay close together

### Whitespace Philosophy
Whitespace should feel **helpful and conversion-aware**, keeping broad B2B messaging accessible without losing product credibility.

---

## 6. Depth & Elevation

### Elevation Strategy
HubSpot uses **soft SaaS elevation** with warm neutrality and clear card grouping.

```css
--shadow-soft: 0 8px 20px rgba(33, 51, 67, 0.05);
--shadow-card: 0 16px 34px rgba(33, 51, 67, 0.08);
```

### Surface Hierarchy
- White base
- Warm cream support bands
- Elevated product cards
- Orange action anchors and soft blue/orange tints

---

## 7. Do's and Don'ts

### Do
- Keep the tone warm, helpful, and business-capable
- Use orange as a strong but controlled brand signal
- Balance educational content with clear product action
- Preserve CRM/product credibility even in marketing-heavy pages

### Don't
- Do not make HubSpot feel like cold enterprise software
- Do not overuse orange across large surfaces
- Do not let feature sprawl overwhelm hierarchy
- Do not use overly technical styling that loses approachability

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked use-case cards and simplified product grouping |
| Tablet | `768px - 1023px` | Two-column feature sections and compact promo layouts |
| Desktop | `1024px+` | Full product-family storytelling with rich section grouping |

### Responsive Rules
- Keep CTA clarity high near the top
- Stack broad CRM category grids before over-compressing content
- Preserve rounded cards and comfortable padding
- Keep educational and product modules visually distinct on mobile

---

## 9. Agent Prompt Guide

### Quick Reference
- White and warm-neutral SaaS foundation with HubSpot orange
- Friendly modern type and rounded feature cards
- Growth-software clarity, CRM credibility, approachable enterprise tone
- Balanced AI, content, sales, and service product framing

### Prompt Template
```text
Design this like HubSpot's current public website:
- white and warm-neutral enterprise SaaS foundation
- HubSpot-orange CTAs with soft blue and orange support tints
- friendly modern typography and rounded feature cards
- broad CRM and growth-platform storytelling that stays approachable
- helpful, content-rich B2B energy without cold enterprise stiffness
```
