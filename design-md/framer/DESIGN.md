# Framer Design System

> Designer-first site building with minimal structure and modern motion-ready polish. Framer's public site uses a sharp, clean sans system with a mostly black-and-white base, vivid blue accents, and product framing that feels fast, premium, and creator-oriented.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Framer feels like **a design-native site builder with startup sharpness and product confidence**. The system is minimal, modern, and direct, with enough color and motion to feel contemporary without losing restraint.

### Mood & Feeling
- Fast and premium
- Design-native, not generic SaaS
- Crisp, minimal, and modern
- Startup-forward with strong product proof
- Built for creators and growth teams

### Design Density
**Medium density.** Framer uses simple structure, strong contrast, and broad product shots to keep a lot of capability messaging feeling light.

### Visual Character
- Black and white frame with bright blue accents
- Big, sharp hero messaging
- Minimal but premium chrome
- Motion- and AI-friendly product framing
- Clean creator-tool energy

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--framer-black` | `#0B0B0D` | Primary contrast and hero framing |
| `--framer-white` | `#FFFFFF` | Main canvas and cards |
| `--framer-surface` | `#F7F8FA` | Soft section fill |
| `--framer-ink` | `#111827` | Primary text |
| `--framer-muted` | `#6B7280` | Secondary text |

### Accent and Utility

| Token | Hex | Role |
|-------|-----|------|
| `--framer-blue` | `#0055FF` | Primary action and accent |
| `--framer-blue-soft` | `#E7EEFF` | Soft blue tint |
| `--framer-border` | `#E5E7EB` | Card and divider stroke |
| `--framer-purple` | `#6D5EF8` | Motion/creative support accent |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, -apple-system, sans-serif;
--font-mono: "JetBrains Mono", "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 64px | 700 | 1.01 | -0.03em | `#0B0B0D` |
| Page Title | 48px | 700 | 1.06 | -0.02em | `#0B0B0D` |
| Section Title | 34px | 700 | 1.12 | -0.02em | `#0B0B0D` |
| Card Title | 24px | 600 | 1.2 | -0.01em | `#111827` |
| Body Large | 18px | 400 | 1.6 | 0 | `#111827` |
| Body | 16px | 400 | 1.6 | 0 | `#111827` |
| Small Body | 14px | 400 | 1.5 | 0 | `#6B7280` |
| Label | 12px | 700 | 1.35 | 0.04em | `#6B7280` |

### Typography Philosophy
Framer typography should feel **sharp, current, and creator-focused**. It should communicate speed and design fluency without unnecessary ornament.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #0055ff;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 46px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #0040cc;
}

.button-secondary {
  background: #ffffff;
  color: #0b0b0d;
  border: 1px solid #e5e7eb;
  border-radius: 999px;
  min-height: 46px;
  padding: 0 20px;
}
```

### Demo Cards

```css
.demo-card {
  background: #ffffff;
  border: 1px solid #e5e7eb;
  border-radius: 24px;
  box-shadow: 0 16px 32px rgba(17, 24, 39, 0.08);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #111827;
  border: 1px solid #e5e7eb;
  border-radius: 14px;
  min-height: 46px;
  padding: 12px 14px;
}
```

### Component Notes
- Product framing should feel premium and fast
- Blue accents work best as action points and signals
- Motion and AI messaging should feel like natural extensions of creation speed

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Fine alignment |
| `--space-3` | `8px` | Tight rhythm |
| `--space-4` | `12px` | Compact spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card spacing |
| `--space-7` | `32px` | Module separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and product-demo rhythm |

### Layout Behavior
- Lead with speed, quality, and builder confidence
- Use crisp demo frames and creator-focused proof
- Keep the page tight and intentional rather than sprawling
- Let motion and AI stories amplify, not distract

### Whitespace Philosophy
Whitespace should feel **modern and premium**, helping the product feel fast and well-designed rather than empty.

---

## 6. Depth & Elevation

### Elevation Strategy
Framer uses **clean premium elevation** with minimal but confident shadowing around demos and cards.

```css
--shadow-soft: 0 8px 20px rgba(17, 24, 39, 0.06);
--shadow-card: 0 18px 36px rgba(17, 24, 39, 0.10);
```

### Surface Hierarchy
- White base
- Occasional black contrast framing
- Elevated demo cards
- Blue and purple accents for action and modernity

---

## 7. Do's and Don'ts

### Do
- Keep the system crisp, premium, and creator-oriented
- Use blue accents with restraint and confidence
- Let product proof and hero messaging stay sharp
- Preserve a strong sense of speed and design fluency

### Don't
- Do not overdecorate Framer into generic gradient startup UI
- Do not crowd the page with too many low-signal sections
- Do not dilute the minimal premium structure
- Do not replace strong product framing with abstract fluff

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked demo blocks and direct CTA hierarchy |
| Tablet | `768px - 1023px` | Two-column product stories and compact hero structure |
| Desktop | `1024px+` | Wide premium demos and broad creator-tool storytelling |

### Responsive Rules
- Preserve big headline impact on mobile
- Keep demo frames legible and visually premium
- Stack motion-heavy or feature-rich layouts before over-compressing them
- Maintain thumb-friendly CTAs and clean spacing

---

## 9. Agent Prompt Guide

### Quick Reference
- Minimal premium black-white builder foundation with Framer blue
- Sharp modern typography and polished demo-card shells
- Creator-first site-builder energy with motion-ready clarity
- Fast, design-native, premium, and restrained

### Prompt Template
```text
Design this like Framer's current public website:
- minimal premium black-and-white builder foundation
- vivid Framer-blue CTAs and selective modern accent color
- sharp modern typography with polished demo cards
- creator-first, motion-ready site-builder product framing
- fast, premium, design-native energy with very little visual waste
```
