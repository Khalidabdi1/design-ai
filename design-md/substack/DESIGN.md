# Substack Design System

> Publishing with literary simplicity, serif display tone, and restrained orange brand cues. Substack's public site uses a clean editorial layout, black-and-white structure, and orange accents to frame newsletters, writers, and subscriptions.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Substack feels like **independent publishing with modern internet simplicity**.
### Mood & Feeling
- Editorial
- Independent
- Minimal
- Literary
- Direct
### Design Density
**Low to medium density.** The site leaves space for writing and creator voice.
### Visual Character
- Black and white base
- Orange support accent
- Serif-friendly editorial tone
- Minimal chrome

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--substack-orange` | `#FF6719` | Brand accent |
| `--substack-black` | `#111111` | Text and strong contrast |
| `--substack-white` | `#FFFFFF` | Canvas |
| `--substack-surface` | `#F8F8F8` | Soft support background |
| `--substack-muted` | `#666666` | Secondary text |
| `--substack-border` | `#E5E5E5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Georgia", "Iowan Old Style", serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `56/700`, H1 `40/700`, H2 `28/700`, Body `17/400`, Small `14/400`
### Typography Philosophy
Mix literary editorial display tone with very simple modern UI text.

## 4. Component Stylings
```css
.button-primary { background:#ff6719; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e5e5; border-radius:999px; min-height:44px; padding:0 18px; }
.card { background:#fff; border:1px solid #e5e5e5; border-radius:18px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Let creators and writing lead
- Keep subscription actions visible but understated
- Preserve editorial breathing room

## 6. Depth & Elevation
Substack uses **minimal depth**; structure comes mostly from spacing and light borders.

## 7. Do's and Don'ts
### Do
- Keep it minimal and editorial
- Use orange as a compact brand signal
- Leave room for text and creator identity
### Don't
- Don’t overbuild the chrome
- Don’t turn it into colorful creator-economy UI noise

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep reading and subscription actions obvious
- Preserve generous text margins

## 9. Agent Prompt Guide
```text
Design this like Substack: minimal editorial publishing UI with black-and-white structure, subtle orange accents, serif-led literary tone, and simple subscription-focused creator pages.
```
