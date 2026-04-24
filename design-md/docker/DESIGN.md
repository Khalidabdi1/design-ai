# Docker Design System

> Container tooling with unmistakable blue branding and developer-centric product proof. Docker's public site uses a bright blue palette, white base surfaces, rounded cards, and code/product screenshots that keep the experience technical but accessible.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Docker feels like **developer tooling with product confidence and accessible platform messaging**.
### Mood & Feeling
- Developer-first
- Clean
- Technical
- Approachable
- Platform-oriented
### Design Density
**Medium density.** Platform breadth is balanced with clear sections and cards.
### Visual Character
- Bright Docker blue
- White and pale-blue surfaces
- Container and workflow imagery
- Product screenshots and code examples

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--docker-blue` | `#2496ED` | Primary brand color |
| `--docker-blue-deep` | `#0B6FC2` | Hover/support |
| `--docker-white` | `#FFFFFF` | Canvas and cards |
| `--docker-surface` | `#F4FAFF` | Soft background |
| `--docker-ink` | `#0F172A` | Text |
| `--docker-muted` | `#64748B` | Secondary text |
| `--docker-border` | `#DCEAF8` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "JetBrains Mono", "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `56/700`, H1 `40/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use precise developer-friendly type with clear hierarchy and strong code support.

## 4. Component Stylings
```css
.button-primary { background:#2496ed; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#0f172a; border:1px solid #dceaf8; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #dceaf8; border-radius:22px; box-shadow:0 12px 24px rgba(15,23,42,.06); }
.code-card { background:#0f172a; color:#fff; border-radius:20px; font-family:var(--font-mono); }
```
### Component Notes
- Blue brand accents should stay bright and recognizable
- Code and workflow proof should remain visible

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Group by build, ship, and run workflow
- Support clear developer scanning
- Use screenshots and diagrams to anchor capability claims

## 6. Depth & Elevation
Docker uses **clean product-card elevation** with strong border separation.

## 7. Do's and Don'ts
### Do
- Keep it developer-native and clear
- Use blue strongly but structurally
- Preserve code and product realism
### Don't
- Don’t replace technical proof with generic marketing visuals
- Don’t muddy the palette with too many extra accents

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack code and workflow cards
- Keep pricing and primary CTA paths obvious

## 9. Agent Prompt Guide
```text
Design this like Docker: bright blue developer-platform branding, white and pale-blue product surfaces, code-aware cards, clean technical typography, and clear build-ship-run workflow storytelling.
```
