# Netlify Design System

> Modern web platform with bright teal-blue energy, black-and-white structure, and agent-ready developer tooling. Netlify's public site uses clean sans typography, strong contrast, code examples, and bright cyan/teal accents.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Netlify feels like **the modern web stack packaged for fast building and shipping**.
### Mood & Feeling
- Fast
- Developer-native
- Modern
- Agent-ready
- Productive
### Design Density
**Medium density.** There is lots of capability detail, but sections remain clean and readable.
### Visual Character
- White and black contrast zones
- Bright cyan-teal accents
- Code examples and workflow diagrams
- Polished developer-platform cards

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--netlify-teal` | `#00C7B7` | Brand action accent |
| `--netlify-teal-deep` | `#00A89A` | Hover/support |
| `--netlify-black` | `#0F172A` | Dark contrast |
| `--netlify-white` | `#FFFFFF` | Main surface |
| `--netlify-surface` | `#F5FBFA` | Soft background |
| `--netlify-ink` | `#111827` | Text |
| `--netlify-muted` | `#64748B` | Secondary text |
| `--netlify-border` | `#DCEEEB` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "JetBrains Mono", "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `58/700`, H1 `42/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use sharp, modern, web-native type with strong support for code and workflow examples.

## 4. Component Stylings
```css
.button-primary { background:#00c7b7; color:#0f172a; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:700; }
.button-secondary { background:#fff; color:#111827; border:1px solid #dceeeB; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #dceeeB; border-radius:22px; box-shadow:0 12px 24px rgba(17,24,39,.06); }
.code-card { background:#0f172a; color:#fff; border-radius:20px; font-family:var(--font-mono); }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Organize by workflow: prompt, preview, ship
- Use code examples and platform primitives as core proof
- Keep developer actions obvious

## 6. Depth & Elevation
Netlify uses **crisp developer-card elevation** with contrast-rich code surfaces.

## 7. Do's and Don'ts
### Do
- Keep it modern, web-native, and fast
- Use teal as a bright structural accent
- Preserve code and infra realism
### Don't
- Don’t flatten it into generic enterprise SaaS
- Don’t bury workflow clarity under decorative visual noise

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack code examples and workflow cards
- Keep build/ship CTAs prominent

## 9. Agent Prompt Guide
```text
Design this like Netlify: modern web-platform UI with teal accents, black-and-white contrast, crisp code-aware cards, workflow-first structure, and fast developer-tool clarity.
```
