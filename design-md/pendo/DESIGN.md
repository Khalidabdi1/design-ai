# Pendo Design System

> Product experience design with bold indigo identity, in-app guide surfaces, NPS-first feedback clarity, and product-led growth UX.

---

## 1. Visual Theme & Atmosphere

Pendo should feel intelligent, product-focused, and customer-centric. The design language communicates in-app guides, tooltips, NPS surveys, feature analytics, and the bridge between product usage data and customer success.

- Mood: intelligent, customer-centric, product-led, modern
- Density: medium, with feature-usage dashboards, guide builders, path analysis charts, and NPS response feeds
- Character: bold indigo brand, white product-experience surfaces, guide-builder canvas, NPS score visualization

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--pen-indigo` | `#2348B1` | Primary brand CTA and active feature |
| `--pen-indigo-dark` | `#1A3A8F` | Hover and active states |
| `--pen-teal` | `#0891B2` | Engagement and session accent |
| `--pen-green` | `#16A34A` | Promoter (NPS 9-10) and positive feedback |
| `--pen-amber` | `#D97706` | Passive (NPS 7-8) and at-risk |
| `--pen-red` | `#DC2626` | Detractor (NPS 0-6) and churned |
| `--surface-card` | `#FFFFFF` | Feature and guide cards |
| `--surface-bg` | `#F8F9FC` | Dashboard background |
| `--surface-guide` | `#F0F4FF` | Guide builder canvas tint |
| `--text-primary` | `#111827` | Feature labels and guide text |
| `--text-secondary` | `#6B7280` | Timestamps and segment labels |
| `--border-default` | `#E5E7EB` | Panel and card borders |

The NPS color scale (green/amber/red for promoter/passive/detractor) is product-critical and must never be repurposed for other UI states.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-mono: "JetBrains Mono", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 30px | 700 | 1.1 |
| Section Title | 22px | 600 | 1.2 |
| NPS Score | 56px | 800 | 1.0 |
| Card Title | 18px | 600 | 1.3 |
| Body | 15px | 400 | 1.6 |
| Guide Text | 15px | 400 | 1.65 |
| Label | 12px | 600 | 1.35 |

## 4. Component Stylings

```css
.button-primary {
  min-height: 40px;
  padding: 0 18px;
  border: none;
  border-radius: 8px;
  background: #2348B1;
  color: #FFFFFF;
  font: 600 14px/1 Inter, sans-serif;
}

.in-app-guide {
  border-radius: 12px;
  background: #FFFFFF;
  border: 1px solid #E5E7EB;
  box-shadow: 0 8px 28px rgba(35, 72, 177, 0.14);
  padding: 20px;
  max-width: 320px;
}

.guide-beacon {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: #2348B1;
  box-shadow: 0 0 0 4px rgba(35, 72, 177, 0.25);
}

.nps-bar {
  display: flex;
  height: 8px;
  border-radius: 999px;
  overflow: hidden;
}

.feature-usage-row {
  display: flex;
  align-items: center;
  padding: 12px 16px;
  border-bottom: 1px solid #E5E7EB;
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `8px` | Feature row spacing |
| `--space-4` | `16px` | Card rhythm |
| `--space-6` | `24px` | Section padding |
| `--space-10` | `40px` | Dashboard section gaps |

NPS score is the hero number on the feedback dashboard. Feature adoption funnel leads the product analytics view. Guide builder uses a center-canvas with floating control panels.

## 6. Depth & Elevation

```css
.shadow-card    { box-shadow: 0 1px 4px rgba(17, 24, 39, 0.06); }
.shadow-guide   { box-shadow: 0 8px 28px rgba(35, 72, 177, 0.14); }
.shadow-modal   { box-shadow: 0 20px 50px rgba(17, 24, 39, 0.16); }
```

In-app guides use a stronger indigo shadow to ensure they visually float above the customer's application.

## 7. Do's and Don'ts

Do make NPS score the largest metric on the feedback dashboard. Do use the beacon animation to draw attention to new guide triggers. Do color-code NPS segments consistently (green/amber/red). Do not use indigo for at-risk or churned states. Do not bury feature usage behind multiple navigation levels.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | NPS summary, feature adoption overview |
| Tablet | `768px` | Feature analytics grid, guide list |
| Desktop | `1200px` | Full platform: analytics + guide builder + NPS + paths |

Guide building and path analysis require desktop. Mobile for NPS and adoption monitoring.

## 9. Agent Prompt Guide

Design like Pendo: bold indigo CTAs, NPS-score hero number, guide-beacon pulses, NPS segment color scale, in-app guide floating cards, feature-usage row tables, and product-led growth hierarchy.
