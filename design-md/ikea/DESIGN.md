# IKEA Design System

> Home retail with democratic warmth, practical utility, and unmistakable brand color. IKEA's public site uses a clean sans system, a white foundation, utility-led merchandising, and the classic IKEA blue (`#0058A3`) and yellow (`#FFDA1A`) identity across navigation and promotions.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
IKEA feels like **accessible home design turned into practical retail navigation**. The system blends Scandinavian clarity, strong merchandising, and a warm, everyday tone.

### Mood & Feeling
- Practical and welcoming
- Utility-first but friendly
- Affordable design confidence
- Family and home oriented
- Structured, not luxurious

### Design Density
**Medium density.** IKEA needs to support a huge catalog, but the site stays approachable through clean merchandising modules, strong labeling, and simple layout rhythms.

### Visual Character
- White page base with strong brand blue anchors
- Yellow used for selected promotion and branding moments
- Large lifestyle and room-setting imagery
- Utility-focused product and category cards
- A warm, everyday retail rhythm

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--ikea-blue` | `#0058A3` | Brand anchor, key navigation, links |
| `--ikea-yellow` | `#FFDA1A` | Brand support and promo highlight |
| `--ikea-white` | `#FFFFFF` | Main surface and cards |
| `--ikea-surface` | `#F5F5F5` | Soft background fill |
| `--ikea-ink` | `#111111` | Primary text |

### Support and Utility

| Token | Hex | Role |
|-------|-----|------|
| `--ikea-muted` | `#666666` | Secondary copy |
| `--ikea-border` | `#E3E3E3` | Divider and card stroke |
| `--ikea-success` | `#12805C` | Positive or sustainability state |
| `--ikea-warm` | `#FFF4D6` | Warm promotional or lifestyle support background |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Noto IKEA", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Noto IKEA", "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 56px | 700 | 1.04 | -0.02em | `#111111` |
| Page Title | 40px | 700 | 1.08 | -0.02em | `#111111` |
| Section Title | 30px | 700 | 1.14 | -0.01em | `#111111` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#111111` |
| Body Large | 18px | 400 | 1.6 | 0 | `#111111` |
| Body | 16px | 400 | 1.6 | 0 | `#111111` |
| Small Body | 14px | 400 | 1.5 | 0 | `#666666` |
| Label | 12px | 700 | 1.35 | 0.04em | `#666666` |

### Typography Philosophy
IKEA typography should feel **clear, democratic, and practical**. It should support navigation, merchandising, and home inspiration without looking precious or luxury-coded.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #111111;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #2a2a2a;
}

.button-secondary {
  background: #ffffff;
  color: #111111;
  border: 1px solid #e3e3e3;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Product and Category Cards

```css
.category-card {
  background: #ffffff;
  border: 1px solid #e3e3e3;
  border-radius: 16px;
  overflow: hidden;
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #111111;
  border: 1px solid #e3e3e3;
  border-radius: 12px;
  min-height: 44px;
  padding: 12px 14px;
}
```

### Component Notes
- Category modules should feel useful and easy to browse
- Brand colors belong mostly in navigation, labels, or promos
- Lifestyle imagery should support everyday realism, not exclusivity

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight product metadata |
| `--space-3` | `8px` | Small spacing |
| `--space-4` | `12px` | Compact padding |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Product shelf gaps |
| `--space-7` | `32px` | Category separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and room-setting modules |

### Layout Behavior
- Keep categories, promotions, and lifestyle inspiration clearly segmented
- Use large imagery to sell room ideas and home scenarios
- Maintain strong scanability for retail browsing
- Favor practical structure over high-fashion editorial layouts

### Whitespace Philosophy
Whitespace should feel **clear and usable**, helping a large retail catalog remain approachable and home-friendly.

---

## 6. Depth & Elevation

### Elevation Strategy
IKEA uses **subtle retail elevation**. Most depth comes from imagery, merchandising blocks, and clean product containers rather than heavy shadow.

```css
--shadow-soft: 0 8px 18px rgba(17, 17, 17, 0.05);
--shadow-card: 0 14px 26px rgba(17, 17, 17, 0.08);
```

### Surface Hierarchy
- White base
- Light gray support backgrounds
- Product and category cards
- Blue/yellow used mainly as brand and promo cues

---

## 7. Do's and Don'ts

### Do
- Keep the site welcoming, practical, and easy to navigate
- Use IKEA blue and yellow as strong brand signals
- Balance lifestyle inspiration with retail utility
- Support everyday affordability and accessibility in the tone

### Don't
- Do not turn IKEA into luxury editorial minimalism
- Do not overuse bright yellow across large reading surfaces
- Do not make navigation feel premium-boutique instead of practical
- Do not clutter category browsing with unnecessary decoration

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked category cards and swipeable promo/lifestyle modules |
| Tablet | `768px - 1023px` | Wider room and category sections with compact merch grids |
| Desktop | `1024px+` | Full home-retail storytelling and broad category navigation |

### Responsive Rules
- Keep category browsing easy on mobile
- Maintain large lifestyle imagery and clear promo labeling
- Stack dense retail sections before shrinking text too aggressively
- Preserve strong CTA and navigation clarity throughout

---

## 9. Agent Prompt Guide

### Quick Reference
- White and light-gray home-retail foundation with IKEA blue and yellow
- Clean practical typography and approachable category cards
- Lifestyle room imagery plus utility-first merchandising
- Warm, democratic, everyday design energy

### Prompt Template
```text
Design this like IKEA's current public website:
- practical home-retail foundation in white, light gray, IKEA blue, and yellow
- clear, democratic typography with easy-to-browse category and product cards
- lifestyle room imagery balanced with utility-focused retail navigation
- approachable, everyday home-design tone instead of luxury editorial styling
- strong merchandising clarity with warm, welcoming structure
```
