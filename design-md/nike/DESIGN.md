# Nike Design System

> Performance retail with aggressive simplicity and image-led energy. Nike's public site stays rooted in black (`#111111`), white (`#FFFFFF`), soft grays, strong product photography, and bold uppercase or condensed headline moments that keep the brand athletic and direct.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Nike feels like **sport culture distilled into a direct, high-impact commerce interface**. The system is image-forward, minimal in chrome, and comfortable letting product photography and bold headline attitude carry the page.

### Mood & Feeling
- Athletic and confident
- Sharp, direct, and modern
- Editorial but commerce-ready
- Product-first, not UI-first
- Energetic without excessive ornament

### Design Density
**Medium density.** Product grids can become information-rich, but the overall design stays simple through monochrome framing and generous imagery.

### Visual Character
- Black and white base with minimal accent noise
- Large shoe and apparel photography
- Strong editorial sale or campaign banners
- Clean product cards with sparse chrome
- Bold, punchy type moments

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--nike-black` | `#111111` | Primary text, nav, CTAs |
| `--nike-white` | `#FFFFFF` | Main canvas and cards |
| `--nike-gray-050` | `#F5F5F5` | Section background |
| `--nike-gray-200` | `#E5E5E5` | Borders and quiet dividers |
| `--nike-muted` | `#757575` | Secondary copy |

### Support Colors

| Token | Hex | Role |
|-------|-----|------|
| `--nike-ink` | `#000000` | Strongest contrast and hero framing |
| `--nike-sale` | `#D33918` | Sale, urgency, or promo accent |
| `--nike-success` | `#12805C` | Positive state |
| `--nike-warm` | `#F7EBDD` | Warm campaign background support |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Futura Condensed Extra Bold", "Helvetica Neue Condensed", Arial, sans-serif;
--font-sans: "Helvetica Neue", Helvetica, Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 72px | 700 | 0.98 | -0.03em | `#111111` |
| Page Title | 48px | 700 | 1.02 | -0.02em | `#111111` |
| Section Title | 32px | 700 | 1.1 | -0.01em | `#111111` |
| Card Title | 20px | 600 | 1.2 | -0.01em | `#111111` |
| Body Large | 18px | 400 | 1.55 | 0 | `#111111` |
| Body | 16px | 400 | 1.55 | 0 | `#111111` |
| Small Body | 14px | 400 | 1.45 | 0 | `#757575` |
| Label | 12px | 600 | 1.35 | 0.06em | `#111111` |

### Typography Philosophy
Nike typography should feel **assertive, sporty, and culturally current**. Keep body text clean and neutral, but let display moments hit hard.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #111111;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 40px;
  padding: 0 18px;
  font-size: 15px;
  font-weight: 500;
}

.button-primary:hover {
  background: #2a2a2a;
}

.button-secondary {
  background: #ffffff;
  color: #111111;
  border: 1px solid #e5e5e5;
  border-radius: 999px;
  min-height: 40px;
  padding: 0 18px;
}
```

### Product Cards

```css
.product-card {
  background: #ffffff;
  border-radius: 16px;
  overflow: hidden;
}
```

### Inputs and Filters

```css
.input,
.filter-pill {
  background: #ffffff;
  color: #111111;
  border: 1px solid #e5e5e5;
  border-radius: 999px;
  min-height: 40px;
  padding: 0 14px;
}
```

### Component Notes
- Product photography should always do more work than decorative UI
- Filters and chips should feel simple, tactile, and low-friction
- Sale accents are secondary to black-and-white framing

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight product metadata rhythm |
| `--space-3` | `8px` | Small gaps |
| `--space-4` | `12px` | Compact internal spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card and shelf spacing |
| `--space-7` | `32px` | Module separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and campaign spacing |

### Layout Behavior
- Use wide campaign imagery and clear product shelves
- Let retail filters stay accessible but secondary to product viewing
- Use bold merchandising rows and category groupings
- Favor clean alignment over decorative layouts

### Whitespace Philosophy
Whitespace should feel **confident and retail-smart**, giving products room to breathe while keeping browsing momentum high.

---

## 6. Depth & Elevation

### Elevation Strategy
Nike uses **minimal elevation**. Most separation comes from image blocks, whitespace, and subtle container edges rather than visible shadow systems.

```css
--shadow-soft: 0 6px 18px rgba(0, 0, 0, 0.06);
--shadow-card: 0 10px 24px rgba(0, 0, 0, 0.08);
```

### Surface Hierarchy
- White page foundation
- Occasional soft-gray category backgrounds
- Large image-led campaign panels
- Minimal card chrome

---

## 7. Do's and Don'ts

### Do
- Keep the system bold, simple, and product-led
- Let imagery and typography carry the emotion
- Preserve a sharp black-and-white retail foundation
- Use accent color selectively for promo or status

### Don't
- Do not overdecorate the commerce interface
- Do not use soft pastel SaaS styling
- Do not let UI chrome compete with product photography
- Do not weaken headline impact with timid type hierarchy

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked campaign panels, swipeable product rails, compact filters |
| Tablet | `768px - 1023px` | Wider product shelves and split campaign modules |
| Desktop | `1024px+` | Full editorial hero campaigns and broad category merchandising |

### Responsive Rules
- Keep product images large on mobile
- Prefer horizontal scrolling shelves over over-compressed grids
- Preserve bold CTA and campaign hierarchy at all sizes
- Keep filter controls thumb-friendly and concise

---

## 9. Agent Prompt Guide

### Quick Reference
- Black, white, and soft-gray retail base
- Bold sport-editorial display type with clean commerce body copy
- Large product photography and minimal chrome
- Direct, athletic, premium but accessible

### Prompt Template
```text
Design this like Nike's current public website:
- black-and-white performance retail foundation
- strong sporty display typography and simple product metadata
- image-led campaign modules and clean merchandising grids
- minimal rounded UI chrome with product-first browsing
- confident athletic energy without decorative clutter
```
