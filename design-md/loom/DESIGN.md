# Loom Design System

> Async video communication with gentle gradients, rounded UI, and simple productivity framing. Loom's public site uses a bright but soft brand palette, white surfaces, and product demos centered on recording, sharing, and collaboration.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Loom feels like **video-first productivity software with soft, approachable polish**.
### Mood & Feeling
- Friendly
- Lightweight
- Productive
- Collaborative
- Clear
### Design Density
**Medium density.** The product is simple, and the layout reflects that simplicity.
### Visual Character
- White surface base
- Soft purple/blue/pink accents
- Rounded demo cards
- Clear async communication workflows

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--loom-purple` | `#6D5EF8` | Primary accent |
| `--loom-blue` | `#4C8DFF` | Support accent |
| `--loom-pink` | `#F25FB5` | Soft support accent |
| `--loom-white` | `#FFFFFF` | Main surface |
| `--loom-surface` | `#F8F7FF` | Soft background |
| `--loom-ink` | `#111827` | Text |
| `--loom-muted` | `#667085` | Secondary text |
| `--loom-border` | `#E7E4FA` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `54/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Favor clean, friendly, low-friction type with soft modern polish.

## 4. Component Stylings
```css
.button-primary { background:#6d5ef8; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#111827; border:1px solid #e7e4fa; border-radius:999px; min-height:44px; padding:0 20px; }
.card { background:#fff; border:1px solid #e7e4fa; border-radius:24px; box-shadow:0 12px 24px rgba(17,24,39,.06); }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Keep the story simple: record, share, collaborate
- Use video UI demos as core proof
- Preserve lightweight page rhythm

## 6. Depth & Elevation
Loom uses **soft rounded elevation** on bright, friendly product cards.

## 7. Do's and Don'ts
### Do
- Keep it friendly and async-work focused
- Use soft gradient accents sparingly
- Let video product demos lead
### Don't
- Don’t make Loom feel like heavy enterprise meetings software
- Don’t overload the page with dense navigation

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack product demos
- Keep record/share CTA paths obvious

## 9. Agent Prompt Guide
```text
Design this like Loom: friendly async-video productivity UI with white rounded cards, soft purple-blue accents, clear product demos, and simple modern collaboration flow.
```
