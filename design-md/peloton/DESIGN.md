# Peloton Design System

> Premium, motivational fitness design built around bold metrics and cinematic instructor content. Peloton's public product pairs a near-black studio-inspired shell with a confident red accent, large legible data displays, and high-production video imagery that makes performance data feel energizing rather than clinical.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Peloton feels like **a boutique fitness studio translated into a digital dashboard**. Dark, cinematic surfaces frame instructor video and live metrics, while a disciplined red accent and large numerals give every workout a sense of premium intensity.

### Mood & Feeling
- Premium, energetic, and motivational
- Cinematic and studio-like, not clinical
- Confident, disciplined use of a single red accent
- Data-forward but never overwhelming
- Aspirational yet approachable

### Design Density
**Low-to-medium density.** Workout and metrics screens emphasize a few large numbers and a hero video/image; class browsing grids are denser but still generously spaced compared to typical media grids.

### Visual Character
- Near-black (`#0B0B0B`) primary surfaces with white text
- Signature red (`#DF0A22`-adjacent) reserved for CTAs, live indicators, and key metrics
- Large, bold numeral displays for output, heart rate, and cadence
- High-contrast instructor video thumbnails with minimal overlay chrome
- Rounded cards and pill-shaped filter chips over a dark canvas

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--pel-black` | `#0B0B0B` | Primary app surface |
| `--pel-white` | `#FFFFFF` | Primary text, light-mode surface |
| `--pel-red` | `#DF0A22` | Primary brand accent, CTAs, live badge |
| `--pel-ink` | `#FFFFFF` | Primary text (dark mode) |
| `--pel-ink-light` | `#101010` | Primary text (light mode) |

### Support Palette

| Token | Hex | Role |
|-------|-----|------|
| `--pel-gray-900` | `#1A1A1A` | Card and panel surfaces |
| `--pel-gray-700` | `#3A3A3A` | Borders, dividers |
| `--pel-gray-400` | `#8C8C8C` | Secondary text, metadata |
| `--pel-gold` | `#D9A441` | Achievement/milestone accent |
| `--pel-green` | `#3DB56B` | Positive metric, zone indicator |
| `--pel-blue` | `#3E7CB1` | Heart-rate zone accent |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Sailec", "Circular", "Helvetica Neue", sans-serif;
--font-sans: "Circular", "Helvetica Neue", Arial, sans-serif;
--font-numeral: "Sailec", "Helvetica Neue", sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Metric Display (output/HR) | 56px | 700 | 1.0 | -0.01em | `#FFFFFF` |
| Page Title | 28px | 700 | 1.2 | 0 | `#FFFFFF` |
| Class Card Title | 16px | 600 | 1.3 | 0 | `#FFFFFF` |
| Body | 14px | 400 | 1.5 | 0 | `#FFFFFF` |
| Meta / Instructor Name | 13px | 500 | 1.3 | 0.01em | `#8C8C8C` |
| Button Label | 14px | 700 | 1.2 | 0.02em | `#FFFFFF` |

### Typography Philosophy
Type should be **bold and metric-forward** — oversized numerals for live performance data, with a clean geometric sans handling everything else so metrics remain the visual anchor.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #df0a22;
  color: #ffffff;
  border: none;
  border-radius: 4px;
  min-height: 48px;
  padding: 0 28px;
  font-size: 14px;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.02em;
}

.button-primary:hover {
  background: #c00919;
}

.button-secondary {
  background: transparent;
  color: #ffffff;
  border: 1px solid #ffffff;
  border-radius: 4px;
  min-height: 48px;
  padding: 0 28px;
}
```

### Class Card

```css
.class-card {
  background: #1a1a1a;
  border-radius: 12px;
  overflow: hidden;
}

.class-thumbnail {
  width: 100%;
  aspect-ratio: 16 / 9;
  object-fit: cover;
}

.live-badge {
  background: #df0a22;
  color: #ffffff;
  border-radius: 4px;
  padding: 2px 8px;
  font-size: 11px;
  font-weight: 700;
  text-transform: uppercase;
}
```

### Metric Tile

```css
.metric-tile {
  display: flex;
  flex-direction: column;
  align-items: center;
  background: #1a1a1a;
  border-radius: 12px;
  padding: 16px 24px;
}

.metric-value {
  font-size: 40px;
  font-weight: 700;
  color: #ffffff;
}

.metric-label {
  font-size: 12px;
  color: #8c8c8c;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
```

### Component Notes
- Live classes always pair a red "LIVE" badge with a subtle pulse or dot indicator
- Metric tiles keep the numeral dominant, label small and secondary beneath it
- Buttons favor sharp, low-radius corners over pill shapes, reinforcing an athletic tone
- Instructor imagery is high-contrast and full-bleed within its card or hero frame

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-1` | `4px` | Icon-to-label gaps |
| `--space-2` | `8px` | Metric tile internal spacing |
| `--space-3` | `16px` | Card internal padding |
| `--space-4` | `24px` | Section spacing |
| `--space-5` | `40px` | Hero and dashboard margins |
| `--space-6` | `64px` | Marketing section spacing |

### Layout Behavior
- Class discovery uses horizontal carousels and grids of 16:9 video thumbnails grouped by discipline
- Active workout screen centers large metric tiles beneath or beside instructor video
- Marketing pages use full-bleed cinematic hero imagery with centered bold headlines
- Dashboard/history views summarize streaks and achievements in compact stat rows

### Whitespace Philosophy
Whitespace should feel **studio-calm and confident** — dark negative space frames video and metrics without competing for attention, reinforcing a premium, focused atmosphere.

---

## 6. Depth & Elevation

### Elevation Strategy
Peloton favors **subtle elevation on a dark canvas** — cards and tiles lift gently off the near-black background using slightly lighter gray fills rather than heavy shadows.

```css
--shadow-card: 0 2px 8px rgba(0, 0, 0, 0.4);
--shadow-hero-overlay: linear-gradient(180deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.7) 100%);
--surface-lift: #1a1a1a;
```

### Surface Hierarchy
- Near-black base canvas
- Slightly lighter gray cards and metric tiles
- Gradient overlays on hero video/imagery for text legibility

---

## 7. Do's and Don'ts

### Do
- Keep red disciplined and reserved for CTAs, live badges, and key highlights
- Make performance metrics the largest, boldest element on any workout screen
- Use high-contrast instructor video/imagery to carry emotional energy
- Maintain a dark, cinematic base canvas across core product screens

### Don't
- Do not lighten the core app canvas into a bright, clinical white
- Do not let secondary metadata compete visually with primary metrics
- Do not use rounded pill buttons; keep corners sharp and athletic
- Do not overuse red beyond CTAs, live indicators, and key accents

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Single-column class feed, stacked metric tiles, full-width video |
| Tablet | `768px - 1023px` | Two-column class grid, side-by-side metric tiles |
| Desktop | `1024px+` | Multi-column carousels, metrics displayed alongside instructor video |

### Responsive Rules
- Metric numerals scale down proportionally but never drop below clear legibility at a glance
- Class thumbnail grids reflow from carousels to stacked lists on narrow viewports
- Live badges and key CTAs remain fixed and visible during scroll on workout screens
- Maintain minimum 44px touch targets for in-workout controls

---

## 9. Agent Prompt Guide

### Quick Reference
- Near-black cinematic canvas with a disciplined red accent
- Oversized bold numerals for live performance metrics
- High-contrast instructor video/imagery with gradient overlays
- Sharp-cornered buttons and cards, subtle dark-mode elevation

### Prompt Template
```text
Design this like Peloton's current public product and brand style:
- near-black cinematic canvas with a disciplined red accent for CTAs and live badges
- oversized, bold numeral displays for performance metrics (output, heart rate, cadence)
- high-contrast, full-bleed instructor video/imagery with gradient overlays for legibility
- sharp-cornered buttons and cards instead of pill shapes, subtle dark-mode elevation
- premium, motivational, studio-inspired atmosphere
```
