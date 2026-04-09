# Linear Design System

> Product-development platform with disciplined dark surfaces and indigo brand focus. The current public Linear site ships `Inter Variable`, `Berkeley Mono`, and `Tiempos Headline`, uses a dark default theme (`#08090A`, `#0F1011`, `#141516`, `#1C1C1F`, `#232326`, `#28282C`), bright text (`#F7F8F8`, `#D0D6E0`), subdued secondary text (`#8A8F98`, `#62666D`), and a distinct indigo accent family led by `#5E6AD2`, `#7070FF`, and `#828FFF`.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Linear feels like **an elite operating console for shipping software**. The product is compact, dark, deliberate, and deeply structured. Marketing and product surfaces share the same core personality: low-noise dark panels, crisp borders, high information density, and precise interaction design.

### Mood & Feeling
- **Focused velocity**: Built for teams that want momentum, not clutter
- **Calm precision**: Dense workflows presented without chaos
- **Dark-system confidence**: The UI is intentionally nocturnal and polished
- **Agent-native structure**: Product surfaces imply automation, reviews, and execution
- **Technical elegance**: Serious, minimal, and highly controlled

### Design Density
**Medium-to-high density**. Linear is comfortable showing issues, projects, diffs, dashboards, and stateful controls in a compact layout. The experience stays readable through strict spacing discipline, restrained color, and consistent card shells.

### Visual Character
- Near-black layered surfaces with fine border contrast
- Indigo brand accents used surgically for priority actions and focus
- Compact text rhythm with tight but readable spacing
- Rounded corners that are subtle, not soft
- Small icons, pills, avatars, and status markers
- Structured dashboards, lists, timelines, and code-aware surfaces

---

## 2. Color Palette & Roles

### Dark Foundations

| Token | Hex | Role |
|-------|-----|------|
| `--color-bg-level-0` | `#08090A` | Deepest app background |
| `--color-bg-level-1` | `#0F1011` | Main panel background |
| `--color-bg-level-2` | `#141516` | Elevated containers |
| `--color-bg-secondary` | `#1C1C1F` | Secondary cards and embedded panels |
| `--color-bg-tertiary` | `#232326` | Higher-elevation dark surface |
| `--color-bg-quaternary` | `#28282C` | Menus, popovers, strong containers |

### Text System

| Token | Hex | Role |
|-------|-----|------|
| `--color-text-primary` | `#F7F8F8` | Primary headings and main copy |
| `--color-text-secondary` | `#D0D6E0` | Secondary UI text |
| `--color-text-tertiary` | `#8A8F98` | Metadata, helper text |
| `--color-text-quaternary` | `#62666D` | Muted labels and lower-emphasis UI |

### Border and Surface Support

| Token | Hex | Role |
|-------|-----|------|
| `--color-border-primary` | `#23252A` | Standard divider and card border |
| `--color-border-secondary` | `#34343A` | Stronger boundary |
| `--color-border-tertiary` | `#3E3E44` | High-emphasis dark outline |
| `--color-bg-translucent` | `rgba(255,255,255,0.05)` | Frosted/overlay dark surface |
| `--color-bg-quaternary` | `rgba(255,255,255,0.15)` | Strong translucent hover surface |

### Brand and Utility Accent Colors

| Token | Hex | Role |
|-------|-----|------|
| `--color-brand-bg` | `#5E6AD2` | Main brand/action color |
| `--color-link-primary` | `#7070FF` | Links and bright active emphasis |
| `--color-accent-hover` | `#828FFF` | Hover/focus accent |
| `--color-blue` | `#4EA7FC` | Info and secondary UI accent |
| `--color-teal` | `#00B8CC` | Analytics/AI/support accent |
| `--color-green` | `#27A644` | Success/healthy state |
| `--color-yellow` | `#F0BF00` | Warning or at-risk state |
| `--color-orange` | `#FC7840` | Changelog and warm highlight accent |
| `--color-red` | `#EB5757` | Destructive or critical issue state |

### Product-Specific Support Colors

| Token | Hex | Role |
|-------|-----|------|
| `--color-linear-plan` | `#68CC58` | Planning / healthy progress |
| `--color-linear-build` | `#D4B144` | Build / active work emphasis |
| `--color-linear-security` | `#7A7FAD` | Security / secondary feature support |

---

## 3. Typography Rules

### Font Stack

```css
--font-sans: "Inter Variable", "SF Pro Display", -apple-system,
             BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;

--font-mono: "Berkeley Mono", ui-monospace, "SF Mono",
             Menlo, monospace;

--font-serif-display: "Tiempos Headline", Georgia, serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 72px | 590 | 1.0 | -0.022em | `#F7F8F8` |
| Page Title | 64px | 590 | 1.06 | -0.022em | `#F7F8F8` |
| Section Title | 48px | 590 | 1.1 | -0.022em | `#F7F8F8` |
| Title Large | 40px | 590 | 1.1 | -0.022em | `#F7F8F8` |
| Title Medium | 32px | 590 | 1.125 | -0.022em | `#F7F8F8` |
| Card Title | 24px | 590 | 1.33 | -0.012em | `#F7F8F8` |
| Body | 15px | 400 | 1.6 | -0.011em | `#D0D6E0` |
| Small Body | 14px | 400 | 1.5 | -0.013em | `#8A8F98` |
| Label | 13px | 510 | 1.5 | -0.01em | `#D0D6E0` |
| Micro | 12px | 510 | 1.4 | 0 | `#62666D` |
| Mono | 13px | 400 | 1.45 | 0 | `#D0D6E0` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 400 | Regular | Body text and descriptive UI |
| 510 | Medium | Controls, labels, metadata emphasis |
| 590 | Semibold | Titles, section headers, CTAs |
| 680 | Bold | Rare emphasis only |

### Typography Philosophy
Linear typography is **compact, calm, and rigorous**. It avoids loud brand theatrics. Most of the personality comes from control, rhythm, and precision rather than dramatic type tricks. Monospace appears naturally in code-aware or agent-aware contexts.

```css
--tracking-tight: -0.022em;
--tracking-body: -0.011em;
--tracking-small: -0.013em;
```

---

## 4. Component Stylings

### Buttons

#### Primary Button
```css
.button-primary {
  background: #5e6ad2;
  color: #ffffff;
  border: 1px solid transparent;
  border-radius: 9999px;
  min-height: 40px;
  padding: 0 18px;
  font-size: 14px;
  font-weight: 590;
  box-shadow: 0px 4px 24px rgba(0, 0, 0, 0.2);
  transition: background 150ms ease, transform 100ms ease;
}

.button-primary:hover {
  background: #828fff;
}

.button-primary:active {
  transform: scale(0.97);
}
```

#### Secondary Button
```css
.button-secondary {
  background: rgba(255, 255, 255, 0.03);
  color: #f7f8f8;
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 9999px;
  min-height: 40px;
  padding: 0 18px;
}

.button-secondary:hover {
  background: rgba(255, 255, 255, 0.07);
}
```

### Cards and Panels
```css
.panel {
  background: #0f1011;
  color: #f7f8f8;
  border: 1px solid #23252a;
  border-radius: 16px;
  box-shadow: 0px 3px 12px rgba(0, 0, 0, 0.09);
}

.panel-strong {
  background: #1c1c1f;
  border-color: #34343a;
}
```

### Inputs and Search
```css
.input {
  background: rgba(255, 255, 255, 0.03);
  color: #f7f8f8;
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 12px;
  min-height: 40px;
  padding: 0 12px;
}

.input::placeholder {
  color: #8a8f98;
}

.input:focus {
  outline: none;
  border-color: #5e6ad2;
  box-shadow: 0 0 0 1px #5e6ad2;
}
```

### Pills, Badges, and Status Chips
```css
.badge {
  display: inline-flex;
  align-items: center;
  min-height: 24px;
  padding: 0 10px;
  border-radius: 9999px;
  background: rgba(255, 255, 255, 0.05);
  color: #d0d6e0;
  border: 1px solid rgba(255, 255, 255, 0.08);
}

.badge-brand {
  background: rgba(94, 106, 210, 0.18);
  color: #ffffff;
  border-color: rgba(130, 143, 255, 0.4);
}
```

### Code and Diff Surfaces
```css
.code-surface {
  background: #08090a;
  color: #d0d6e0;
  border: 1px solid #23252a;
  border-radius: 12px;
  padding: 16px;
  font-family: "Berkeley Mono", "SF Mono", monospace;
}
```

### Component Philosophy
Linear components should feel **tight, polished, and quietly powerful**. The right feel is a premium internal tool, not a playful SaaS dashboard. Keep states obvious, borders subtle, and motion fast.

---

## 5. Layout Principles

### Spacing Scale
Linear repeatedly uses compact increments such as `4`, `6`, `8`, `10`, `12`, `16`, `20`, `24`, `40`, and `48` pixels across gaps and control spacing.

```css
--space-1: 4px;
--space-2: 6px;
--space-3: 8px;
--space-4: 10px;
--space-5: 12px;
--space-6: 16px;
--space-7: 20px;
--space-8: 24px;
--space-9: 40px;
--space-10: 48px;
```

### Corner Radius Scale

```css
--radius-4: 4px;
--radius-6: 6px;
--radius-8: 8px;
--radius-12: 12px;
--radius-16: 16px;
--radius-24: 24px;
--radius-32: 32px;
--radius-pill: 9999px;
```

### Layout Style
- Keep content in disciplined rows, lists, and stacked panels
- Use narrow gutters and clear hierarchy between page chrome and work surfaces
- Favor split layouts, dashboards, timelines, and side panels
- Let the indigo accent guide action, not dominate the whole page
- Use whitespace to improve scanability, not to create dramatic emptiness

### Whitespace Philosophy
Linear should feel **efficient, not cramped**. The layout can be dense, but spacing must stay deliberate and internally consistent so the interface reads as calm.

---

## 6. Depth & Elevation

### Exposed Shadow Tokens

```css
--shadow-none: 0px 0px 0px transparent;
--shadow-tiny: 0px 1px 1px 0px rgba(0, 0, 0, 0.09);
--shadow-low: 0px 1px 4px -1px rgba(0, 0, 0, 0.09);
--shadow-medium: 0px 3px 12px rgba(0, 0, 0, 0.09);
--shadow-high: 0px 7px 32px rgba(0, 0, 0, 0.35);
```

### Elevation Style
Linear uses **subtle dark-surface layering**. Many surfaces look distinguished primarily by fill and border, with restrained shadows reserved for popovers, command palettes, and floating panels.

### Surface Hierarchy
1. Base canvas `#08090A`
2. Main panels `#0F1011` / `#141516`
3. Elevated containers `#1C1C1F` / `#232326`
4. Menus and modal shells `#28282C`
5. Accent buttons, badges, and focused controls

### Elevation Rules
- Prefer border contrast before adding more shadow
- Use deeper shadow for overlays, not for routine cards
- Keep floating UI compact and crisp
- Avoid glossy glassmorphism or bright ambient glow

---

## 7. Do's and Don'ts

### Do
- Use near-black surfaces with tightly controlled layering
- Keep typography compact, calm, and highly legible
- Use indigo accents sparingly for action and focus
- Build structured lists, boards, dashboards, and side panels
- Make agent, issue, and project surfaces feel native to the same system

### Don't
- Don’t brighten the UI into a generic white SaaS dashboard
- Don’t overuse gradients, glow, or decorative noise
- Don’t make cards overly rounded or soft
- Don’t use oversized spacing that breaks the dense, productive feel
- Don’t flood the interface with too many accent colors at once

---

## 8. Responsive Behavior

### Breakpoints

```css
--bp-sm: 640px;
--bp-md: 768px;
--bp-lg: 1024px;
--bp-xl: 1280px;
```

### Mobile and Narrow-Screen Behavior
- Collapse secondary panels beneath the primary work area
- Convert wide data layouts into stacked cards with clear labels
- Preserve compact control height and list density where possible
- Keep primary actions accessible without visually dominating the screen
- Reduce hero headline size quickly on marketing pages to preserve rhythm

### Touch Targets

```css
--touch-target-min: 40px;
--control-height-sm: 24px;
--control-height-md: 40px;
--control-height-lg: 48px;
```

### Responsive Philosophy
On smaller screens, Linear should still feel **like a serious product-development tool**. Compress gracefully, but do not lose the strong structure, quiet borders, or dark-system identity.

---

## 9. Agent Prompt Guide

### Quick Visual Summary
- Use a deep dark foundation with layered charcoal panels
- Set type in Inter Variable, with Berkeley Mono for code-aware surfaces
- Use indigo accents like `#5E6AD2`, `#7070FF`, and `#828FFF`
- Keep borders fine, shadows restrained, and corners subtle
- Favor dense, high-signal layouts for issues, projects, dashboards, and agents

### Prompt Snippet

```txt
Design this interface like Linear's current public design system: near-black layered backgrounds, subtle bordered panels, compact Inter-style typography, Berkeley Mono for code and agent surfaces, indigo primary actions, restrained motion, quiet shadows, and dense but polished product-management layouts. Avoid bright consumer-app styling, large empty whitespace, or soft playful components.
```
