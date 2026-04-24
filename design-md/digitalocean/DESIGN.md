# DigitalOcean Design System

> Developer cloud infrastructure with approachable blue branding and practical product clarity. DigitalOcean's public site uses a bright blue anchor, white surfaces, rounded cards, and a friendly developer-cloud tone.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
DigitalOcean feels like **developer cloud made accessible and clean**.
### Mood & Feeling
- Friendly
- Technical
- Clear
- Cloud-native
- Startup-to-scale
### Design Density
**Medium density.** Platform breadth is present but digestible.
### Visual Character
- Strong blue brand accent
- White cards and illustrations
- Rounded SaaS surfaces
- Developer-focused clarity

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--do-blue` | `#0080FF` | Primary action |
| `--do-blue-deep` | `#0069D9` | Hover/support |
| `--do-white` | `#FFFFFF` | Main surface |
| `--do-surface` | `#F5F9FF` | Soft background |
| `--do-ink` | `#0F172A` | Text |
| `--do-muted` | `#64748B` | Secondary text |
| `--do-border` | `#DCE7F7` | Borders |
| `--do-success` | `#16825D` | Positive state |

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
Use modern developer-friendly typography with direct hierarchy and high clarity.

## 4. Component Stylings
```css
.button-primary { background:#0080ff; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#0f172a; border:1px solid #dce7f7; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #dce7f7; border-radius:22px; box-shadow:0 12px 24px rgba(15,23,42,.06); }
.code-card { background:#0f172a; color:#fff; border-radius:20px; font-family:var(--font-mono); }
```
### Component Notes
- Platform cards should stay approachable
- Code examples and infra proof should feel first-class

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Group by developer use case and infrastructure capability
- Use bright blue sparingly but clearly
- Pair marketing copy with code/product proof

## 6. Depth & Elevation
DigitalOcean uses **light developer-SaaS elevation** with strong border clarity.

## 7. Do's and Don'ts
### Do
- Keep it approachable and developer-native
- Use blue as the main structural accent
- Preserve product clarity over visual flourish
### Don't
- Don’t overcomplicate it with cloud-theater gradients
- Don’t make it feel corporate-heavy

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack code and product modules
- Keep pricing/product CTAs visible

## 9. Agent Prompt Guide
```text
Design this like DigitalOcean: approachable developer cloud UI with bright blue accents, white rounded cards, clean technical typography, code-aware product sections, and simple infrastructure clarity.
```
