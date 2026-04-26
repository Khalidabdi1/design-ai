# N26 Design System

> Digital banking with calm European clarity. N26's current public site combines white surfaces, deep charcoal and teal-green brand accents, soft gradients, clean app previews, and quiet premium plan framing to make mobile banking feel secure, transparent, and beautifully simple.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
N26 feels like **minimal digital banking with design-led trust**. The system is cleaner and quieter than many fintech brands, leaning on spacious layouts, curated color, and phone-first product proof rather than loud hype. Plan tiers and security messaging are integrated into the same calm visual system.

### Mood & Feeling
- Calm and modern
- Transparent and secure
- Minimal without being cold
- Mobile-native and quietly premium
- Trustworthy with light editorial polish

### Design Density
**Medium density.** N26 includes plans, savings, investing, and security messaging, but the layout stays digestible because each section is tightly focused and visually restrained.

### Visual Character
- White and charcoal foundation with distinctive teal-green support
- Soft dark gradients behind premium cards and plan showcases
- Clean smartphone previews with minimal chrome
- Rounded modules and clear, direct trust messaging
- Product framing that feels elegant rather than flashy

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--n26-white` | `#FFFFFF` | Main background and elevated cards |
| `--n26-surface` | `#F5F7F8` | Soft section background |
| `--n26-ink` | `#111111` | Primary dark contrast and hero framing |
| `--n26-charcoal` | `#1E2428` | Secondary dark surface |
| `--n26-text` | `#1F2933` | Default body text |

### Brand and Support

| Token | Hex | Role |
|-------|-----|------|
| `--n26-teal` | `#2AA89B` | Primary brand accent |
| `--n26-teal-deep` | `#1F7F76` | Hover and active accent |
| `--n26-teal-soft` | `#D9F1ED` | Light brand fill |
| `--n26-border` | `#D8E1E4` | Card and input border |
| `--n26-muted` | `#69757D` | Secondary text |

### Utility

| Token | Hex | Role |
|-------|-----|------|
| `--n26-gold` | `#C8A96B` | Premium plan highlight |
| `--n26-success` | `#2E8B57` | Positive savings or approval state |
| `--n26-danger` | `#C74B4B` | Error or risk notice |
| `--n26-focus` | `#9EE2D9` | Focus ring tint |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "N26 Sans", "Helvetica Neue", Arial, sans-serif;
--font-sans: "N26 Sans", system-ui, -apple-system, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 68px | 700 | 1.02 | -0.03em | `#111111` |
| Page Title | 48px | 700 | 1.08 | -0.02em | `#111111` |
| Section Title | 34px | 700 | 1.12 | -0.015em | `#111111` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#1F2933` |
| Body Large | 18px | 400 | 1.6 | 0 | `#1F2933` |
| Body | 16px | 400 | 1.6 | 0 | `#1F2933` |
| Small Body | 14px | 400 | 1.45 | 0 | `#69757D` |
| Label | 12px | 700 | 1.3 | 0.04em | `#69757D` |

### Typography Philosophy
N26 typography should feel **clean, direct, and quietly premium**. Headlines can be large and confident, but the overall reading experience should stay calm and transparent.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #111111;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
  font-size: 16px;
  font-weight: 700;
}

.button-primary:hover {
  background: #1e2428;
}

.button-secondary {
  background: #ffffff;
  color: #111111;
  border: 1px solid #d8e1e4;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
}
```

### Cards and Plan Panels

```css
.plan-card {
  background: #ffffff;
  border: 1px solid #d8e1e4;
  border-radius: 24px;
  box-shadow: 0 16px 34px rgba(17, 17, 17, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #1f2933;
  border: 1px solid #d8e1e4;
  border-radius: 14px;
  min-height: 48px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #2aa89b;
  box-shadow: 0 0 0 4px rgba(158, 226, 217, 0.38);
}
```

### Component Notes
- Plan and card modules should feel premium but not flashy
- Teal should guide focus and freshness, not dominate the whole screen
- Security and trust details should remain extremely easy to scan

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
| `--space-10` | `96px` | Large product and plan sections |

### Layout Behavior
- Let one product promise lead each section clearly
- Use phone previews and plan cards as primary proof blocks
- Keep plan comparisons, security claims, and feature benefits separated cleanly
- Use soft gradient or dark backdrops selectively for premium plan emphasis

### Whitespace Philosophy
Whitespace should feel **deliberate and calm**, reinforcing transparency and making the product feel beautifully simple rather than sparse by accident.

---

## 6. Depth & Elevation

### Elevation Strategy
N26 uses **subtle premium-product elevation**. Cards rise gently above the background while dark gradients and plan framing create most of the depth.

```css
--shadow-soft: 0 8px 20px rgba(17, 17, 17, 0.04);
--shadow-card: 0 16px 34px rgba(17, 17, 17, 0.07);
--shadow-focus: 0 0 0 4px rgba(158, 226, 217, 0.38);
```

### Surface Hierarchy
- White base canvas
- Light gray support surfaces
- Elevated white plan and product cards
- Dark charcoal or gradient premium plan sections

---

## 7. Do's and Don'ts

### Do
- Keep N26 calm, elegant, and trust-first
- Use teal as a clean accent with clear purpose
- Let product previews and plan framing carry the story
- Preserve strong simplicity across features and security messaging

### Don't
- Do not make N26 loud or hype-driven
- Do not overload the interface with too many bright accent colors
- Do not make plan tiers feel gaudy or overly luxurious
- Do not bury trust and security details under visual ornament

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked phone previews, simple plan cards, clear trust blocks |
| Tablet | `768px - 1023px` | Two-column feature and plan groupings |
| Desktop | `1024px+` | Wide product storytelling, plan showcases, and dark premium sections |

### Responsive Rules
- Keep plan tiers and trust cues legible before adding decorative chrome
- Stack phone previews and copy into straightforward vertical flows
- Preserve teal accent clarity and comfortable tap targets
- Maintain the calm white-space rhythm on smaller screens

---

## 9. Agent Prompt Guide

### Quick Reference
- White and charcoal structure with restrained teal-green accents
- Calm premium mobile-banking layout with clean plan framing
- Rounded product cards, simple phone previews, and strong trust clarity
- Elegant, minimal, transparent, and secure

### Prompt Template
```text
Design this like N26's current public website:
- white and charcoal surfaces with restrained teal-green accents
- clean smartphone previews and quietly premium plan cards
- rounded modules, soft gradients, and very direct trust messaging
- minimal, elegant mobile-banking feel with strong simplicity
- transparent, secure, and beautifully simple rather than loud fintech hype
```
