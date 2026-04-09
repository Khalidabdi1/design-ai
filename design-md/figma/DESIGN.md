# Figma Design System

> Collaborative product-design platform with a sharp black-and-white foundation and bright product accents. The current public Figma site ships `figmaSans`, `figmaMono`, and `ABCWhytePlusVariable`, and repeatedly pairs hard black (`#000000`) and white (`#FFFFFF`) surfaces with vivid platform colors like indigo (`#4D49FC`), green (`#24CB71`), cyan (`#00B6FF`), orange (`#FF7237`), coral (`#FFC9C1`), lavender (`#C4BAFF`), aqua (`#C7F8FB`), lilac (`#CB9FD2`), and lime (`#E4FF97`).

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Figma feels like **a product-design operating system translated into marketing form**. It is highly structured, intentionally graphic, and confident about contrast. Even when the site becomes playful, the design still feels tool-like rather than whimsical. The system communicates precision first, then creativity.

### Mood & Feeling
- **Design-tool confidence**: Built for people who care about craft and systems
- **High-contrast clarity**: Bold black-and-white structure anchors the experience
- **Creative energy**: Product modules use bright, categorical accent colors
- **Modular intelligence**: Cards, demos, and content blocks feel snapped to a grid
- **Professional optimism**: Color is vivid, but never childish

### Design Density
**Medium density**. Figma gives product stories and demos room to breathe, but it also likes compact interface examples, data blocks, and tightly grouped actions. The overall system feels editorially spacious and operationally precise at the same time.

### Visual Character
- Strong black/white contrast with minimal muddiness
- Large product-story sections broken into modular blocks
- Bright accent swatches used to distinguish products and feature families
- Big type with crisp spacing and tool-like UI demos
- Mostly flat surfaces, with separation coming from outlines, fills, and contrast
- Rounded rectangles that stay geometric rather than soft or bubbly

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--figma-black` | `#000000` | Primary canvas, dark sections, strong CTAs |
| `--figma-white` | `#FFFFFF` | Inverse canvas, cards, text on dark |
| `--figma-gray-100` | `#E6E6E6` | Soft separators and muted surfaces |
| `--figma-gray-200` | `#E2E2E2` | Light outlines and subtle fills |
| `--figma-gray-700` | `#697485` | Support text and quiet metadata |

### Product Accent Colors

| Token | Hex | Role |
|-------|-----|------|
| `--figma-indigo` | `#4D49FC` | Core platform accent, links, key highlights |
| `--figma-green` | `#24CB71` | Positive/product accent, confirmations |
| `--figma-cyan` | `#00B6FF` | Informational accent, tool energy |
| `--figma-orange` | `#FF7237` | Warm callout accent and feature differentiation |
| `--figma-coral` | `#FFC9C1` | Soft warm background block |
| `--figma-lavender` | `#C4BAFF` | Secondary highlight background |
| `--figma-aqua` | `#C7F8FB` | Light cool surface highlight |
| `--figma-lilac` | `#CB9FD2` | Illustrative/support accent |
| `--figma-lime` | `#E4FF97` | Bright attention surface |
| `--figma-mint` | `#F3FFE3` | Pale green support surface |
| `--figma-sand` | `#FADCA2` | Warm neutral feature tile |

### Error / Form Feedback

| Token | Hex | Role |
|-------|-----|------|
| `--figma-error` | `#FF3737` | Error emphasis and destructive attention |
| `--figma-error-soft` | `#FFB3B3` | Error background |
| `--figma-error-deep` | `#972121` | Deep error state background |
| `--figma-error-deeper` | `#721C1C` | Very dark error surface |

### Form Surface Tokens Exposed by the Site

| Token | Value | Role |
|-------|-------|------|
| `--f-form-input-bg-color` | `rgba(0, 0, 0, 0.08)` | Light-mode input fill |
| `--f-form-input-bg-color` | `rgba(255, 255, 255, 0.16)` | Dark-mode/inverse input fill |
| `--f-form-placeholder-text-color` | `rgba(0, 0, 0, 0.5)` | Light placeholder text |
| `--f-form-placeholder-text-color` | `rgba(255, 255, 255, 0.6)` | Dark placeholder text |
| `--f-primary-transparent-color` | `rgba(0, 0, 0, 0.16)` | Light hover/active wash |
| `--f-primary-transparent-color` | `rgba(255, 255, 255, 0.24)` | Dark hover/active wash |

### Color Usage Philosophy
Figma uses color **categorically rather than decoratively**. The black-and-white frame stays stable, while accent colors label products, demos, feature stories, and supportive illustrations. Avoid gradients and soft haze unless a specific surface clearly calls for them.

---

## 3. Typography Rules

### Font Stack

```css
--font-sans: "figmaSans", "figmaSans Fallback", "SF Pro Display",
             system-ui, Helvetica, sans-serif;

--font-display: "ABCWhytePlusVariable", "ABCWhytePlusVariable Fallback",
                Whyte, sans-serif;

--font-mono: "figmaMono", "figmaMono Fallback", "SF Mono",
             Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 72px | 550 | 1.0 | -0.03em | `#000000` |
| Page Title | 56px | 550 | 1.02 | -0.025em | `#000000` |
| Section Title | 40px | 550 | 1.08 | -0.02em | `#000000` |
| Card Title | 24px | 500 | 1.18 | -0.01em | `#000000` |
| Subsection | 18px | 500 | 1.35 | -0.01em | `#000000` |
| Body Large | 18px | 400 | 1.5 | 0 | `#000000` |
| Body | 16px | 400 | 1.5 | 0 | `#000000` |
| Small Body | 14px | 400 | 1.45 | 0 | `#697485` |
| Label | 13px | 500 | 1.3 | 0.02em | `#000000` |
| Mono | 13px | 400 | 1.4 | 0 | `#000000` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 400 | Regular | Explanatory copy and metadata |
| 500 | Medium | Product labels, navigation, buttons |
| 550 | Display Medium | Large headlines and product storytelling |

### Typography Philosophy
Figma typography is **precise, modern, and product-led**. It is not ornate. Display moments can feel bold and brand-owned, but body text remains straightforward and highly scannable. Monospace should be used when the surface references code, tokens, or developer workflows.

```css
--tracking-tight: -0.03em;
--tracking-display: -0.02em;
--tracking-normal: 0;
```

---

## 4. Component Stylings

### Buttons

#### Primary Button
```css
.button-primary {
  background: #000000;
  color: #ffffff;
  border: 1px solid #000000;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
  font-size: 14px;
  font-weight: 500;
  transition: transform 120ms ease, opacity 160ms ease;
}

.button-primary:hover {
  opacity: 0.88;
}

.button-primary:active {
  transform: scale(0.98);
}
```

#### Secondary / Inverse Button
```css
.button-secondary {
  background: #ffffff;
  color: #000000;
  border: 1px solid rgba(0, 0, 0, 0.12);
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
}

.button-secondary:hover {
  background: #f7f7f7;
}
```

### Cards and Demo Blocks
```css
.product-card {
  background: #ffffff;
  color: #000000;
  border: 1px solid #e2e2e2;
  border-radius: 20px;
  overflow: hidden;
}

.product-card-accent {
  background: #c7f8fb;
}
```

### Inputs and Selects
```css
.input {
  background: rgba(0, 0, 0, 0.08);
  color: #000000;
  border: 1px solid transparent;
  border-radius: 14px;
  min-height: 48px;
  padding: 12px 14px;
}

.input::placeholder {
  color: rgba(0, 0, 0, 0.5);
}

.input:focus {
  outline: none;
  border-color: #4d49fc;
}
```

### Code / Token Surfaces
```css
.code-surface {
  background: #000000;
  color: #ffffff;
  border-radius: 16px;
  padding: 16px 18px;
  font-family: "figmaMono", "SF Mono", monospace;
}
```

### Badges and Product Pills
```css
.badge {
  display: inline-flex;
  align-items: center;
  min-height: 28px;
  padding: 0 12px;
  border-radius: 999px;
  background: #ffffff;
  color: #000000;
  border: 1px solid rgba(0, 0, 0, 0.08);
}
```

### Component Philosophy
Figma components should feel **systematic and tool-ready**. The right default is crisp shape, strong legibility, and functional contrast. Do not make the UI overly soft, misty, or skeuomorphic.

---

## 5. Layout Principles

### Grid and Width
The live site exposes a modular grid approach with `12`, `24`, and `48` column configurations, `24px` gutters, and max content widths around `1440px` to `1680px`.

```css
--layout-columns-desktop: 24;
--layout-columns-wide: 48;
--layout-columns-mobile: 12;
--layout-gutter: 24px;
--layout-max-width: 1440px;
--layout-max-width-wide: 1680px;
```

### Section Spacing
Figma uses large modular padding values for feature blocks and storytelling sections.

```css
--section-padding-tight: 5rem;
--section-padding-default: 7.5rem;
--section-padding-large: 10rem;
```

### Layout Style
- Alternate black, white, and accent-backed sections for rhythm
- Keep demos and product previews inside clearly bounded modules
- Let headlines span wide, but keep body copy in readable columns
- Use strong alignment and repeatable spacing over decorative asymmetry
- Make room for screenshots, canvases, and workflow diagrams

### Whitespace Philosophy
Whitespace in Figma should feel **intentional and grid-driven**, not airy for its own sake. Leave breathing room around major product moments, but keep internal spacing disciplined and repeatable.

---

## 6. Depth & Elevation

### Elevation Style
Figma leans **mostly flat**. Separation usually comes from contrast, outlines, section switching, and clean shape boundaries more than from dramatic shadow stacks.

### Recommended Elevation System

```css
--shadow-none: none;
--shadow-soft: 0 1px 0 rgba(0, 0, 0, 0.08);
--shadow-medium: 0 12px 32px rgba(0, 0, 0, 0.08);
```

### Surface Hierarchy
1. Base black or white canvas
2. Bounded cards with 1px outline
3. High-emphasis demo blocks or code surfaces
4. Accent-backed feature modules

### Elevation Rules
- Prefer outlines before shadows
- Use deeper shadow only for modal or floating showcase content
- Keep cards visually crisp; avoid cloudy blur-heavy panels
- Let color blocking do most of the separation work

---

## 7. Do's and Don'ts

### Do
- Use black and white as the stable structural frame
- Introduce accent colors in clear, intentional blocks
- Keep interface chrome precise and grid-aligned
- Use display type sparingly for large product moments
- Make code, design, and collaboration surfaces feel equally native

### Don't
- Don’t turn the system into a gradient-heavy startup landing page
- Don’t use muddy neutral palettes or weak contrast
- Don’t over-round cards into a soft consumer-app look
- Don’t mix too many accent colors inside the same small component
- Don’t make interactions feel playful at the cost of clarity

---

## 8. Responsive Behavior

### Breakpoints

```css
--bp-sm: 560px;
--bp-md: 960px;
--bp-lg: 1280px;
--bp-xl: 1680px;
```

### Mobile Adaptation
- Collapse wide demo grids into vertical story blocks
- Keep CTAs full-width or nearly full-width on small screens
- Reduce hero type aggressively to preserve control
- Stack feature comparisons rather than squeezing them
- Preserve strong contrast and clear section breaks at every size

### Touch Targets

```css
--touch-target-min: 44px;
--control-height-default: 48px;
```

### Responsive Philosophy
Figma on smaller screens should still feel **like a design platform**, not like a generic mobile marketing page. Preserve structure, contrast, and product clarity first.

---

## 9. Agent Prompt Guide

### Quick Visual Summary
- Use a black-and-white structural base
- Add bright product accents like `#4D49FC`, `#24CB71`, `#00B6FF`, and `#FF7237`
- Prefer `figmaSans` for UI, `ABCWhytePlusVariable` for hero moments, and `figmaMono` for code/tokens
- Keep cards geometric, outlined, and mostly flat
- Use disciplined grids, strong alignment, and modular spacing

### Prompt Snippet

```txt
Design this interface like Figma's current public design system: strong black/white structure, crisp modular cards, bright categorical accent colors, figmaSans-style UI typography, ABC Whyte-like display headlines, figmaMono for code surfaces, large product-story sections, outlined components, and a precise grid-driven layout. Avoid soft gradients, muddy neutrals, or overly playful consumer-app styling.
```
