# 1Password Design System

> Identity and access security with a calm, premium SaaS frame. 1Password's public site uses deep indigo and blue gradients, white surfaces, rounded cards, and a modern sans stack to make security feel approachable and controlled.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
1Password feels like **security software with product warmth**. It balances enterprise seriousness with polished, rounded, modern UI.
### Mood & Feeling
- Trustworthy
- Modern
- Calm
- Security-forward
- AI-era enterprise
### Design Density
**Medium density.** Dashboards, cards, and proof points are rich, but spacing keeps the experience breathable.
### Visual Character
- Indigo and blue foundations
- White elevated cards
- Rounded dashboard shells
- Controlled gradients

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--onepass-indigo` | `#13233A` | Deep brand background |
| `--onepass-blue` | `#3B82F6` | Primary action |
| `--onepass-blue-soft` | `#EAF2FF` | Soft surface tint |
| `--onepass-white` | `#FFFFFF` | Cards and main canvas |
| `--onepass-ink` | `#172033` | Primary text |
| `--onepass-muted` | `#667085` | Secondary text |
| `--onepass-border` | `#DCE4F0` | Borders |
| `--onepass-success` | `#16825D` | Positive state |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Hero | 60px | 700 | 1.04 |
| H1 | 42px | 700 | 1.08 |
| H2 | 30px | 700 | 1.14 |
| Body | 16px | 400 | 1.6 |
| Small | 14px | 400 | 1.5 |
### Typography Philosophy
Use crisp, readable sans-serif type with strong hierarchy and minimal flourish.

## 4. Component Stylings
```css
.button-primary { background:#3b82f6; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#172033; border:1px solid #dce4f0; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #dce4f0; border-radius:24px; box-shadow:0 14px 28px rgba(19,35,58,.08); }
.input { background:#fff; border:1px solid #dce4f0; border-radius:14px; min-height:46px; padding:12px 14px; }
```
### Component Notes
- Rounded analytics cards
- Strong CTA pills
- Security dashboards framed as approachable modules

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Lead with trust and governance outcomes
- Pair copy with dashboard proof
- Use wide hero rows and modular feature grids

## 6. Depth & Elevation
1Password uses **soft premium elevation**.
```css
--shadow-soft: 0 8px 18px rgba(19,35,58,.06);
--shadow-card: 0 16px 32px rgba(19,35,58,.1);
```

## 7. Do's and Don'ts
### Do
- Keep it calm, modern, and security-trustworthy
- Use indigo and blue as the stable brand frame
- Preserve rounded premium cards
### Don't
- Don’t make it flashy fintech neon
- Don’t crowd dashboards or proof modules

## 8. Responsive Behavior
### Breakpoints
- Mobile: `< 768px`
- Tablet: `768px - 1023px`
- Desktop: `1024px+`
### Responsive Rules
- Stack dashboard demos on mobile
- Keep CTAs large and clear
- Preserve readable metrics and labels

## 9. Agent Prompt Guide
### Quick Reference
- Indigo security SaaS
- Rounded white cards
- Blue pill CTAs
- Calm dashboard-led trust
### Prompt Template
```text
Design this like 1Password: indigo-and-blue security SaaS, rounded white dashboard cards, crisp modern sans typography, strong trust cues, and premium but calm enterprise polish.
```
