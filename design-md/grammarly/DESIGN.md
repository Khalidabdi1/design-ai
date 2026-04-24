# Grammarly Design System

> Writing assistance with polished calm and enterprise trust. Grammarly's current public site pairs a bright white canvas with deep forest-ink contrast, saturated mint-green action color, cool gray UI framing, rounded cards, and motion-driven product storytelling that makes AI feel helpful rather than flashy.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Grammarly feels like **professional writing support rendered as calm product guidance**. The system is clean, airy, and conversion-focused, but it avoids cold enterprise severity. Product demos, AI agents, and trust messages are framed with soft radii, generous spacing, and restrained accent use.

### Mood & Feeling
- Clear and reassuring
- Professional without feeling stiff
- AI-forward but grounded in utility
- Calm, polished, and high-trust
- Friendly enough for individual users and credible enough for enterprise buyers

### Design Density
**Medium density.** Grammarly presents a lot of capability and proof in one page, but uses spacing, sectional rhythm, and restrained color blocks to keep the interface easy to scan.

### Visual Character
- Bright white background with dark ink anchors
- Mint-green brand accents used primarily for action and emphasis
- Large, rounded demo cards and proof modules
- Clean text-heavy sections supported by product animation
- Security and trust messaging integrated directly into the visual system

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--grammarly-white` | `#FFFFFF` | Main background and cards |
| `--grammarly-surface` | `#F4F7FB` | Soft section background |
| `--grammarly-surface-2` | `#EAF3F1` | Light brand-tinted surface |
| `--grammarly-ink` | `#0E101A` | Primary dark text and deep surfaces |
| `--grammarly-text` | `#1F2430` | Default body copy |

### Brand and Support

| Token | Hex | Role |
|-------|-----|------|
| `--grammarly-green` | `#15C39A` | Primary CTA, brand accent |
| `--grammarly-green-deep` | `#0E9F80` | Hover and active state |
| `--grammarly-green-soft` | `#DFF7F1` | Highlight fills and soft callouts |
| `--grammarly-border` | `#D8E1EB` | Card and input border |
| `--grammarly-muted` | `#6D758D` | Secondary text and metadata |

### Utility

| Token | Hex | Role |
|-------|-----|------|
| `--grammarly-success` | `#168A6A` | Positive completion state |
| `--grammarly-warning` | `#B7791F` | Caution state |
| `--grammarly-danger` | `#C2413B` | Error emphasis |
| `--grammarly-focus` | `#78E2C7` | Focus ring tint |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Styrene A Web", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Styrene A Web", system-ui, -apple-system, sans-serif;
--font-mono: "SF Mono", "Roboto Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 72px | 700 | 1.02 | -0.035em | `#0E101A` |
| Page Title | 52px | 700 | 1.08 | -0.025em | `#0E101A` |
| Section Title | 36px | 700 | 1.12 | -0.02em | `#0E101A` |
| Card Title | 24px | 600 | 1.22 | -0.01em | `#1F2430` |
| Body Large | 18px | 400 | 1.6 | 0 | `#1F2430` |
| Body | 16px | 400 | 1.6 | 0 | `#1F2430` |
| Small Body | 14px | 400 | 1.5 | 0 | `#6D758D` |
| Label | 12px | 700 | 1.3 | 0.04em | `#6D758D` |

### Typography Philosophy
Grammarly typography should feel **confident, readable, and quietly premium**. Headlines can be bold and compact, but body copy must stay effortless to read because the brand promise is clarity itself.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #15c39a;
  color: #0e101a;
  border: none;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
  font-size: 16px;
  font-weight: 700;
}

.button-primary:hover {
  background: #0e9f80;
  color: #ffffff;
}

.button-secondary {
  background: #ffffff;
  color: #0e101a;
  border: 1px solid #d8e1eb;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
}
```

### Cards and Product Demos

```css
.product-card {
  background: #ffffff;
  border: 1px solid #d8e1eb;
  border-radius: 24px;
  box-shadow: 0 16px 40px rgba(14, 16, 26, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #1f2430;
  border: 1px solid #d8e1eb;
  border-radius: 14px;
  min-height: 48px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #15c39a;
  box-shadow: 0 0 0 4px rgba(120, 226, 199, 0.35);
}
```

### Component Notes
- Product surfaces should feel spacious and editorial, not cramped admin UI
- Demo modules can be elevated, but controls should stay simple and legible
- Trust badges, plan cards, and proof points should share one consistent radius language

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight alignment |
| `--space-3` | `8px` | Small gaps |
| `--space-4` | `12px` | Compact padding |
| `--space-5` | `16px` | Default UI spacing |
| `--space-6` | `24px` | Card internals |
| `--space-7` | `32px` | Section grouping |
| `--space-8` | `48px` | Major module rhythm |
| `--space-9` | `64px` | Hero spacing |
| `--space-10` | `96px` | Large storytelling sections |

### Layout Behavior
- Lead with a strong promise headline and concise support copy
- Use alternating light surfaces to separate trust, product, and pricing blocks
- Favor wide demo cards and controlled copy widths over dense dashboards
- Let proof sections breathe so enterprise credibility lands clearly

### Whitespace Philosophy
Whitespace should feel **supportive and high-confidence**, giving writing demos room to read naturally and keeping the page aligned with the product promise of clarity.

---

## 6. Depth & Elevation

### Elevation Strategy
Grammarly uses **soft SaaS elevation**. Cards lift gently off the canvas, while color and spacing do more work than dramatic shadows.

```css
--shadow-soft: 0 8px 20px rgba(14, 16, 26, 0.05);
--shadow-card: 0 16px 40px rgba(14, 16, 26, 0.08);
--shadow-focus: 0 0 0 4px rgba(120, 226, 199, 0.35);
```

### Surface Hierarchy
- White base canvas
- Soft gray and mint-tinted supporting sections
- Elevated white cards for demos and plans
- Dark ink sections reserved for contrast and trust framing

---

## 7. Do's and Don'ts

### Do
- Keep the experience clear, polished, and writing-first
- Use green as a precise action color rather than a background wash everywhere
- Make AI feel practical, assistive, and credible
- Preserve calm spacing and highly readable copy blocks

### Don't
- Do not make Grammarly look like neon AI hypeware
- Do not overload sections with too many accent colors
- Do not turn every module into a heavy bordered dashboard
- Do not sacrifice reading comfort for decorative motion

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked hero, simplified proof modules, full-width CTAs |
| Tablet | `768px - 1023px` | Two-column card layouts with reduced hero scale |
| Desktop | `1024px+` | Wide demo storytelling and multi-card trust sections |

### Responsive Rules
- Keep CTA buttons large and pill-shaped on touch devices
- Stack animation and copy modules rather than shrinking text too aggressively
- Maintain readable paragraph widths on small screens
- Collapse plan and proof grids into clear vertical sequences

---

## 9. Agent Prompt Guide

### Quick Reference
- White canvas with deep ink contrast and mint-green CTA accents
- Bold neo-grotesk headlines with highly readable body copy
- Rounded SaaS cards, calm spacing, and trust-heavy product framing
- AI should feel useful, credible, and quietly polished

### Prompt Template
```text
Design this like Grammarly's current public site:
- bright white layout with deep charcoal text and mint-green primary actions
- large rounded product cards with soft enterprise SaaS elevation
- bold, compact headlines and very readable supporting copy
- practical AI-writing demos and trust/security framing
- polished, calm, clarity-first visual language
```
