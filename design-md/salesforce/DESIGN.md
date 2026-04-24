# Salesforce Design System

> Enterprise CRM with bright cloud-brand optimism and structured product breadth. Salesforce's public site uses `Salesforce Sans`, cloud-heavy imagery, white and sky-blue surfaces, and a vivid brand blue anchored around `#0176D3`.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Salesforce feels like **enterprise software presented through optimistic cloud-platform branding**. The system is broad, bright, and highly productized, but softened by friendly illustrations, cloud shapes, and approachable color.

### Mood & Feeling
- Optimistic enterprise software
- Platform-scale and highly structured
- Cloud-native and product-rich
- Friendly enough for wide business audiences
- Built for solution browsing and trust

### Design Density
**Medium to high density.** Salesforce exposes many product categories and industries, but uses strong grouping, illustration, and clear section breaks to keep orientation intact.

### Visual Character
- White and sky-blue brand foundation
- Rounded modules and cloud-influenced shapes
- Product-family navigation and deep solution stacks
- Friendly enterprise illustrations
- Blue-led CTAs and links

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--sf-blue` | `#0176D3` | Primary brand and CTA blue |
| `--sf-blue-deep` | `#032D60` | Deep brand navy and footer anchor |
| `--sf-white` | `#FFFFFF` | Main canvas and cards |
| `--sf-sky` | `#EAF5FE` | Soft brand background |
| `--sf-ink` | `#181818` | Primary text |

### Support and Utility

| Token | Hex | Role |
|-------|-----|------|
| `--sf-muted` | `#5C5C5C` | Secondary copy |
| `--sf-border` | `#D8E6F4` | Dividers and container edges |
| `--sf-green` | `#2E844A` | Positive state |
| `--sf-orange` | `#FE9339` | Warm accent support |
| `--sf-focus` | `rgba(1, 118, 211, 0.16)` | Focus ring |

---

## 3. Typography Rules

### Font Stack

```css
--font-sans: "Salesforce Sans", "Helvetica Neue", Arial, sans-serif;
--font-display: "Salesforce Sans", "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 56px | 700 | 1.06 | -0.02em | `#032D60` |
| Page Title | 44px | 700 | 1.08 | -0.02em | `#032D60` |
| Section Title | 32px | 700 | 1.14 | -0.01em | `#032D60` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#181818` |
| Body Large | 18px | 400 | 1.6 | 0 | `#181818` |
| Body | 16px | 400 | 1.6 | 0 | `#181818` |
| Small Body | 14px | 400 | 1.5 | 0 | `#5C5C5C` |
| Label | 12px | 700 | 1.35 | 0.04em | `#032D60` |

### Typography Philosophy
Salesforce typography should feel **enterprise-ready, friendly, and scalable**. It should work across many product types without losing warmth or clarity.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #0176d3;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
  font-size: 15px;
  font-weight: 700;
}

.button-primary:hover {
  background: #0263b0;
}

.button-secondary {
  background: #ffffff;
  color: #032d60;
  border: 1px solid #d8e6f4;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 22px;
}
```

### Cards and Solution Blocks

```css
.solution-card {
  background: #ffffff;
  border: 1px solid #d8e6f4;
  border-radius: 24px;
  box-shadow: 0 12px 28px rgba(3, 45, 96, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #181818;
  border: 1px solid #d8e6f4;
  border-radius: 14px;
  min-height: 48px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #0176d3;
  box-shadow: 0 0 0 4px rgba(1, 118, 211, 0.16);
}
```

### Component Notes
- Solution blocks should feel polished and category-friendly
- Blue is the dominant action and brand cue
- Cloud and AI visuals can be more playful than routine product lists

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight alignment |
| `--space-3` | `8px` | Small rhythm |
| `--space-4` | `12px` | Compact spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card interiors |
| `--space-7` | `32px` | Module separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and solution rows |

### Layout Behavior
- Organize products by business function and workflow
- Use large solution groupings and clear section labels
- Let illustrations and clouds soften dense enterprise information
- Keep deep navigation obvious but not oppressive

### Whitespace Philosophy
Whitespace should feel **bright and guided**, making large enterprise solution sets feel easier to browse.

---

## 6. Depth & Elevation

### Elevation Strategy
Salesforce uses **soft enterprise-card elevation**. Bright surfaces, light borders, and subtle shadows are the main structural tools.

```css
--shadow-soft: 0 8px 20px rgba(3, 45, 96, 0.05);
--shadow-card: 0 16px 34px rgba(3, 45, 96, 0.08);
```

### Surface Hierarchy
- White base
- Sky-blue support sections
- Elevated white solution cards
- Deep navy used for strong anchors and contrast

---

## 7. Do's and Don'ts

### Do
- Keep the interface bright, optimistic, and highly structured
- Use blue and cloud-brand cues consistently
- Make enterprise solution browsing feel approachable
- Support broad product depth with strong grouping

### Don't
- Do not turn Salesforce into dull corporate gray SaaS
- Do not overcomplicate the page with too many accent colors
- Do not let playful illustrations reduce enterprise clarity
- Do not flatten solution hierarchies into generic card grids

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked solution cards and simplified category navigation |
| Tablet | `768px - 1023px` | Two-column feature groupings and compact illustration rows |
| Desktop | `1024px+` | Full ecosystem browsing and broad solution storytelling |

### Responsive Rules
- Preserve CTA clarity and section grouping at smaller sizes
- Stack heavy enterprise category content rather than shrinking it excessively
- Keep illustrations supportive, not dominant, on mobile
- Maintain easy scanability of product families and solution modules

---

## 9. Agent Prompt Guide

### Quick Reference
- White and sky-blue enterprise foundation with Salesforce blue
- Salesforce Sans feel, cloud-brand optimism, rounded solution cards
- Broad CRM platform hierarchy with approachable structure
- Friendly enterprise illustrations and clean navigation

### Prompt Template
```text
Design this like Salesforce's current public website:
- bright white and sky-blue enterprise cloud foundation
- Salesforce-blue CTAs and deep navy hierarchy anchors
- rounded solution cards with friendly cloud-platform polish
- broad CRM product families organized into clear business categories
- approachable enterprise software energy with strong structural clarity
```
