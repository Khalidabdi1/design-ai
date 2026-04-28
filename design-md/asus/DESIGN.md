# ASUS Design System

> Personal computing with broad innovation energy. ASUS's current public site blends bright white merchandising surfaces, deep blue and black contrast areas, crisp product-family storytelling, and premium device imagery across laptops, gaming, creator tools, AI PCs, and mobile devices, creating a tech ecosystem that feels polished, ambitious, and current.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
ASUS feels like **mainstream and enthusiast computing unified under polished innovation branding**. The system needs to support Zenbook elegance, ROG power, ProArt creator credibility, and business utility without losing coherence. Public-facing pages use clean layouts, strong imagery, and measured brand contrast to keep that portfolio readable.

### Mood & Feeling
- Innovative and broad
- Premium but still commercial
- Product-polished and future-facing
- Capable across consumer, creator, business, and gaming contexts
- Confident without constant visual aggression

### Design Density
**Medium density.** ASUS presents many categories and launches, but the layout stays readable through strong product segmentation, clear hero blocks, and polished card groupings.

### Visual Character
- White and pale-gray content surfaces
- Deep blue and black anchors with product-specific accent variation
- Laptop, monitor, and phone imagery used as the primary proof medium
- Strong sub-brand organization around Zenbook, Vivobook, ProArt, ROG, and business devices
- Marketing that balances design elegance and technical credibility

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--asus-white` | `#FFFFFF` | Main canvas and product cards |
| `--asus-surface` | `#F4F6F8` | Soft section background |
| `--asus-ink` | `#0E1420` | Deep contrast background and nav framing |
| `--asus-ink-soft` | `#1D2635` | Secondary dark surface |
| `--asus-text` | `#1F2937` | Primary body text |

### Brand and Support

| Token | Hex | Role |
|-------|-----|------|
| `--asus-blue` | `#005BFF` | Primary action and brand accent |
| `--asus-blue-deep` | `#003EBC` | Hover and active state |
| `--asus-blue-soft` | `#E5EEFF` | Light callout fill |
| `--asus-border` | `#D7DFEA` | Borders and separators |
| `--asus-muted` | `#6B7280` | Secondary text |

### Utility

| Token | Hex | Role |
|-------|-----|------|
| `--asus-success` | `#148A58` | Positive status and support state |
| `--asus-warning` | `#BE7B00` | Warning state |
| `--asus-danger` | `#D14343` | Error or issue state |
| `--asus-focus` | `#A9C6FF` | Focus ring tint |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "TT Norms Pro", "Helvetica Neue", Arial, sans-serif;
--font-sans: "TT Norms Pro", system-ui, -apple-system, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 68px | 700 | 1.02 | -0.03em | `#0E1420` |
| Page Title | 48px | 700 | 1.08 | -0.02em | `#0E1420` |
| Section Title | 34px | 700 | 1.12 | -0.015em | `#0E1420` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#1F2937` |
| Body Large | 18px | 400 | 1.6 | 0 | `#1F2937` |
| Body | 16px | 400 | 1.6 | 0 | `#1F2937` |
| Small Body | 14px | 400 | 1.45 | 0 | `#6B7280` |
| Label | 12px | 700 | 1.3 | 0.04em | `#6B7280` |

### Typography Philosophy
ASUS typography should feel **clean, product-smart, and portfolio-flexible**. It should be premium enough for creator and flagship devices, but practical enough for broad category navigation and merchandising.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #005bff;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
  font-size: 16px;
  font-weight: 700;
}

.button-primary:hover {
  background: #003ebc;
}

.button-secondary {
  background: #ffffff;
  color: #0e1420;
  border: 1px solid #d7dfea;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
}
```

### Cards and Product Panels

```css
.product-card {
  background: #ffffff;
  border: 1px solid #d7dfea;
  border-radius: 22px;
  box-shadow: 0 14px 30px rgba(14, 20, 32, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #1f2937;
  border: 1px solid #d7dfea;
  border-radius: 14px;
  min-height: 48px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #005bff;
  box-shadow: 0 0 0 4px rgba(169, 198, 255, 0.38);
}
```

### Component Notes
- Product-family cards should clearly separate consumer, creator, gaming, and business offerings
- Device renders should feel premium and precise, not cluttered with extra chrome
- Sub-brand distinctions can be visible, but the overall system should still feel unified

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
| `--space-10` | `96px` | Large product, launch, and category sections |

### Layout Behavior
- Lead with current flagship launches and then branch into sub-brand pathways
- Use category rails to help people self-sort into creator, gaming, business, or consumer products
- Keep device imagery large and cleanly framed
- Balance promotional storytelling with practical browse and buy pathways

### Whitespace Philosophy
Whitespace should feel **polished and portfolio-aware**, making a broad product ecosystem feel intentional rather than crowded.

---

## 6. Depth & Elevation

### Elevation Strategy
ASUS uses **light premium-tech elevation**. Cards float subtly above pale surfaces, while dark-blue framing and product imagery create the stronger sense of depth.

```css
--shadow-soft: 0 8px 18px rgba(14, 20, 32, 0.04);
--shadow-card: 0 14px 30px rgba(14, 20, 32, 0.08);
--shadow-focus: 0 0 0 4px rgba(169, 198, 255, 0.38);
```

### Surface Hierarchy
- White main canvas
- Light gray support backgrounds
- Elevated white product cards
- Deep blue and black framing for premium and category emphasis

---

## 7. Do's and Don'ts

### Do
- Keep ASUS broad, polished, and product-family clear
- Use blue as the default action and innovation anchor
- Let device imagery and sub-brand pathways do major navigational work
- Preserve a balance between premium storytelling and practical browsing

### Don't
- Do not make ASUS feel like only a gaming brand
- Do not blur sub-brand distinctions until the catalog becomes confusing
- Do not overload product pages with decorative effects
- Do not let merchandising clutter overpower device clarity

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked launch cards, simplified category rails, clear browse CTAs |
| Tablet | `768px - 1023px` | Two-column product-family and promo layouts |
| Desktop | `1024px+` | Broad hero storytelling, multi-card product ecosystems, and sub-brand category hubs |

### Responsive Rules
- Preserve clean sub-brand navigation when cards stack
- Keep hero device imagery legible rather than overly reduced
- Maintain simple CTA paths from campaign to category to product
- Let dark framing sections collapse cleanly without losing contrast

---

## 9. Agent Prompt Guide

### Quick Reference
- White and deep-blue structure with bright blue action accents
- Broad product-family hierarchy across consumer, creator, gaming, and business
- Clean device renders, rounded cards, and polished launch storytelling
- Premium but browseable, portfolio-rich, and current

### Prompt Template
```text
Design this like ASUS's current public website:
- white merchandising canvas with deep blue framing and bright blue CTA accents
- broad product-family navigation across Zenbook, Vivobook, creator, gaming, and business
- clean laptop and device imagery with rounded product cards
- polished innovation storytelling balanced with practical browsing
- premium mainstream computing feel rather than a single-purpose gaming brand
```
