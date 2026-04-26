# Revolut Design System

> Global money movement with sleek app-first confidence. Revolut's current public site uses bright white surfaces, deep near-black framing, sharp product screenshots, metallic card imagery, and blue-forward accents to make spending, saving, travel, and multi-currency money management feel premium, fast, and highly controlled.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Revolut feels like **modern finance with a premium digital edge**. The system is clean and app-centered, but more dramatic than a typical bank site. Product cards, account modules, and travel or savings features are presented with dark contrast moments, crisp device frames, and smooth mobile-first storytelling.

### Mood & Feeling
- Premium and fast
- Global, flexible, and mobile-native
- Highly controlled rather than playful
- Clear enough for everyday money tasks
- Product-polished with a luxury-tech undertone

### Design Density
**Medium density.** Revolut covers many financial jobs at once, but the experience stays readable through large app previews, strong card grouping, and very deliberate hierarchy.

### Visual Character
- White canvas with deep charcoal anchors
- Blue-forward accent language with metallic card imagery
- Mobile app screens as primary proof objects
- Rounded modules with sharp contrast and polished screenshot presentation
- Travel, spending, and savings framed as one fluid ecosystem

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--revolut-white` | `#FFFFFF` | Main background and cards |
| `--revolut-surface` | `#F6F7FB` | Soft section background |
| `--revolut-ink` | `#0B0D12` | Deep contrast background and primary text |
| `--revolut-ink-soft` | `#1A1F2C` | Secondary dark panels |
| `--revolut-text` | `#1F2937` | Default body text |

### Brand and Support

| Token | Hex | Role |
|-------|-----|------|
| `--revolut-blue` | `#2563FF` | Primary action and feature accent |
| `--revolut-blue-deep` | `#1746D1` | Hover and active state |
| `--revolut-blue-soft` | `#E7EEFF` | Light callout fill |
| `--revolut-border` | `#D8E0ED` | Card and input borders |
| `--revolut-muted` | `#6B7280` | Secondary text |

### Utility

| Token | Hex | Role |
|-------|-----|------|
| `--revolut-success` | `#119E5A` | Positive balance or savings state |
| `--revolut-warning` | `#B7791F` | Warning or fee-related notice |
| `--revolut-danger` | `#D14343` | Error or fraud alert |
| `--revolut-focus` | `#9FB9FF` | Focus ring tint |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Aeonik", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Aeonik", system-ui, -apple-system, sans-serif;
--font-mono: "SF Mono", "Roboto Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 70px | 700 | 1.02 | -0.035em | `#0B0D12` |
| Page Title | 50px | 700 | 1.08 | -0.025em | `#0B0D12` |
| Section Title | 34px | 700 | 1.12 | -0.02em | `#0B0D12` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#1F2937` |
| Body Large | 18px | 400 | 1.6 | 0 | `#1F2937` |
| Body | 16px | 400 | 1.6 | 0 | `#1F2937` |
| Small Body | 14px | 400 | 1.45 | 0 | `#6B7280` |
| Label | 12px | 700 | 1.3 | 0.04em | `#6B7280` |

### Typography Philosophy
Revolut typography should feel **precise, modern, and premium-digital**. Headlines can be bold and sleek, but the body system must keep broad feature sets understandable and fast to scan.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #0b0d12;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
  font-size: 16px;
  font-weight: 700;
}

.button-primary:hover {
  background: #1a1f2c;
}

.button-secondary {
  background: #ffffff;
  color: #0b0d12;
  border: 1px solid #d8e0ed;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
}
```

### Cards and App Panels

```css
.product-card {
  background: #ffffff;
  border: 1px solid #d8e0ed;
  border-radius: 24px;
  box-shadow: 0 16px 34px rgba(11, 13, 18, 0.07);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #1f2937;
  border: 1px solid #d8e0ed;
  border-radius: 14px;
  min-height: 48px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #2563ff;
  box-shadow: 0 0 0 4px rgba(159, 185, 255, 0.35);
}
```

### Component Notes
- Card and screenshot modules should feel polished and device-native
- Dark sections should add premium contrast, not visual heaviness
- Product breadth should be grouped by money jobs like spend, save, travel, invest, and send

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight alignment |
| `--space-3` | `8px` | Small gaps |
| `--space-4` | `12px` | Compact internal spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card internals |
| `--space-7` | `32px` | Module grouping |
| `--space-8` | `48px` | Section rhythm |
| `--space-9` | `64px` | Hero spacing |
| `--space-10` | `96px` | Large product storytelling blocks |

### Layout Behavior
- Use the app and card ecosystem as the central storytelling device
- Group products by user outcomes instead of by financial jargon
- Alternate between bright and dark sections to create pace
- Keep global reach and multi-currency proof close to feature messaging

### Whitespace Philosophy
Whitespace should feel **premium and controlled**, giving the page room to breathe while still supporting a broad set of financial products and travel features.

---

## 6. Depth & Elevation

### Elevation Strategy
Revolut uses **soft premium-product elevation**. Surfaces lift cleanly, while contrast, device frames, and card imagery do much of the visual work.

```css
--shadow-soft: 0 8px 20px rgba(11, 13, 18, 0.05);
--shadow-card: 0 16px 34px rgba(11, 13, 18, 0.08);
--shadow-focus: 0 0 0 4px rgba(159, 185, 255, 0.35);
```

### Surface Hierarchy
- White base canvas
- Light gray-blue support surfaces
- Elevated white feature cards
- Deep dark contrast blocks for hero or premium storytelling

---

## 7. Do's and Don'ts

### Do
- Keep Revolut sleek, fast, and product-polished
- Use dark contrast and blue accents to signal control and modernity
- Let app screens and card visuals carry trust
- Preserve clarity across a wide range of money features

### Don't
- Do not make Revolut feel like a playful neobank toy
- Do not overdecorate with unnecessary gradients or color noise
- Do not flatten product depth into generic landing-page marketing
- Do not make premium contrast sections muddy or low-contrast

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked app proofs, simplified feature clusters, full-width CTAs |
| Tablet | `768px - 1023px` | Two-column product and proof groupings |
| Desktop | `1024px+` | Wide app storytelling, dark-light section rhythm, multi-card layouts |

### Responsive Rules
- Keep the app screens legible rather than shrinking them too aggressively
- Stack related money tasks into vertical flows on mobile
- Maintain strong CTA visibility and dark/light contrast balance
- Preserve card and device prominence across breakpoints

---

## 9. Agent Prompt Guide

### Quick Reference
- White and deep-charcoal surfaces with blue accent guidance
- Sleek app-first fintech storytelling with polished card imagery
- Rounded product cards, premium contrast moments, and clear global-money messaging
- Fast, controlled, modern, and mobile-native

### Prompt Template
```text
Design this like Revolut's current public website:
- bright white and deep charcoal sections with blue feature accents
- polished mobile app screenshots and premium card imagery
- sleek rounded product cards and concise global-money messaging
- premium digital-finance feel with strong contrast and clean hierarchy
- fast, mobile-first, multi-currency product energy
```
