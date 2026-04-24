# Robinhood Design System

> Investing and trading with a stripped-down, high-contrast fintech identity. Robinhood's public site uses a mostly black-and-white base with its signature vivid green (`#00C805`), minimal chrome, and direct product framing for investing, crypto, cards, and brokerage tools.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Robinhood feels like **finance simplified into a direct, high-contrast consumer interface**. The system is modern, sparse, and unmistakably fintech, with green providing the emotional and brand anchor.

### Mood & Feeling
- Bold and disruptive
- Minimal and current
- Consumer-finance focused
- Fast, direct, and low-friction
- Slightly rebellious compared with traditional brokerage UX

### Design Density
**Medium density.** The UI stays relatively sparse, but there is a lot of product breadth across investing, crypto, and financial services.

### Visual Character
- Black, white, and vivid green
- Large, direct hero statements
- Minimal decorative UI
- Finance products framed with clean contrast
- Dense product menus under a sparse visual shell

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--robinhood-green` | `#00C805` | Primary brand and action accent |
| `--robinhood-black` | `#0A0A0A` | Main text and dark framing |
| `--robinhood-white` | `#FFFFFF` | Main surface and cards |
| `--robinhood-surface` | `#F7F7F7` | Soft section background |
| `--robinhood-muted` | `#666666` | Secondary copy |

### Support and Utility

| Token | Hex | Role |
|-------|-----|------|
| `--robinhood-border` | `#E5E5E5` | Dividers and card strokes |
| `--robinhood-green-soft` | `#DDFBE3` | Soft success/brand tint |
| `--robinhood-danger` | `#FF5000` | Negative risk or loss signal |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Graphik", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Graphik", system-ui, -apple-system, sans-serif;
--font-mono: "Roboto Mono", "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 64px | 700 | 1.01 | -0.03em | `#0A0A0A` |
| Page Title | 48px | 700 | 1.06 | -0.02em | `#0A0A0A` |
| Section Title | 34px | 700 | 1.12 | -0.02em | `#0A0A0A` |
| Card Title | 24px | 600 | 1.2 | -0.01em | `#0A0A0A` |
| Body Large | 18px | 400 | 1.6 | 0 | `#0A0A0A` |
| Body | 16px | 400 | 1.6 | 0 | `#0A0A0A` |
| Small Body | 14px | 400 | 1.5 | 0 | `#666666` |
| Label | 12px | 700 | 1.35 | 0.05em | `#666666` |

### Typography Philosophy
Robinhood typography should feel **direct, current, and uncompromisingly simple**. The interface should read fast and feel modern.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #00c805;
  color: #0a0a0a;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 700;
}

.button-primary:hover {
  background: #00ad04;
}

.button-secondary {
  background: #ffffff;
  color: #0a0a0a;
  border: 1px solid #e5e5e5;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Cards and Market Modules

```css
.market-card {
  background: #ffffff;
  border: 1px solid #e5e5e5;
  border-radius: 20px;
  box-shadow: 0 12px 28px rgba(10, 10, 10, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #0a0a0a;
  border: 1px solid #e5e5e5;
  border-radius: 12px;
  min-height: 44px;
  padding: 12px 14px;
}
```

### Component Notes
- Green should remain a sharp, high-recognition brand signal
- Finance modules should feel stripped down rather than decorative
- Robinhood works best when the UI feels fast and uncluttered

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Dense data alignment |
| `--space-3` | `8px` | Tight rhythm |
| `--space-4` | `12px` | Compact spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card spacing |
| `--space-7` | `32px` | Module separation |
| `--space-8` | `48px` | Section rhythm |
| `--space-9` | `64px` | Hero structure |

### Layout Behavior
- Lead with clear financial action and account creation
- Keep visuals sparse and modern
- Use product menus and category depth without cluttering the page frame
- Let black, white, and green do most of the brand work

### Whitespace Philosophy
Whitespace should feel **deliberate and high-contrast**, giving finance products a sense of calm clarity and speed.

---

## 6. Depth & Elevation

### Elevation Strategy
Robinhood uses **low-drama elevation**. Minimal containers and high contrast matter more than strong shadow systems.

```css
--shadow-soft: 0 8px 18px rgba(10, 10, 10, 0.05);
--shadow-card: 0 14px 30px rgba(10, 10, 10, 0.08);
```

### Surface Hierarchy
- White base with occasional black contrast zones
- Lightly elevated cards
- Green used for key action and brand-recognition moments

---

## 7. Do's and Don'ts

### Do
- Keep the design minimal, bold, and fast
- Let green serve as the unmistakable brand signal
- Preserve strong hierarchy for onboarding and core finance actions
- Keep the UI modern and uncluttered

### Don't
- Do not overdecorate with gradients or excessive fintech futurism
- Do not turn Robinhood into a traditional banking UI
- Do not bury CTAs under dense copy
- Do not dilute the black-white-green contrast system

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked finance promos and simplified signup focus |
| Tablet | `768px - 1023px` | Two-column product explanation modules |
| Desktop | `1024px+` | Full sparse hero and broad product-navigation depth |

### Responsive Rules
- Preserve the direct signup path on mobile
- Keep product categories easy to browse without visual overload
- Maintain high contrast and large CTAs
- Prefer stacking over shrinking dense finance content too aggressively

---

## 9. Agent Prompt Guide

### Quick Reference
- Minimal black-white fintech frame with Robinhood green
- Direct, modern typography and low-chrome finance cards
- Fast onboarding, sparse UI, bold consumer-investing energy
- Disruptive but still readable and trustworthy

### Prompt Template
```text
Design this like Robinhood's current public website:
- stripped-down black-and-white fintech foundation
- vivid Robinhood-green CTAs and brand signals
- direct modern typography with sparse, high-contrast layout
- clean finance modules and low-chrome product presentation
- fast, consumer-investing energy without traditional banking stiffness
```
