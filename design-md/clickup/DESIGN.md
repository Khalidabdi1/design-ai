# ClickUp Design System

> Productivity software with a bright gradient brand, polished dashboards, and all-in-one work platform messaging. ClickUp's public site combines violet, pink, and blue gradients with white cards and dense productivity demos.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
ClickUp feels like **productivity SaaS with more visual energy than typical work software**.
### Mood & Feeling
- Fast
- Energetic
- Productive
- All-in-one
- Modern
### Design Density
**Medium density.** Demos are feature-rich, but the framing is polished and spacious.
### Visual Character
- Gradient brand accents
- White rounded cards
- Dashboard and document demos
- Bright modern SaaS polish

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--clickup-violet` | `#7B61FF` | Primary brand accent |
| `--clickup-pink` | `#F63D68` | Gradient support |
| `--clickup-blue` | `#3B82F6` | Supporting accent |
| `--clickup-white` | `#FFFFFF` | Main surface |
| `--clickup-ink` | `#101828` | Text |
| `--clickup-muted` | `#667085` | Secondary text |
| `--clickup-border` | `#E7EAF3` | Borders |
| `--clickup-surface` | `#F7F8FF` | Soft background |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Axiforma", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Axiforma", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `58/700`, H1 `42/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use modern productivity-focused type with strong, upbeat hierarchy.

## 4. Component Stylings
```css
.button-primary { background:linear-gradient(135deg,#7b61ff,#f63d68); color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:700; }
.button-secondary { background:#fff; color:#101828; border:1px solid #e7eaf3; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #e7eaf3; border-radius:24px; box-shadow:0 12px 24px rgba(16,24,40,.06); }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Lead with all-in-one platform positioning
- Use dense but polished work demos
- Let gradients highlight, not dominate

## 6. Depth & Elevation
ClickUp uses **soft elevated cards** with bright accent energy.

## 7. Do's and Don'ts
### Do
- Keep it vivid and modern
- Use gradient accents intentionally
- Preserve polished board/doc/dashboard demos
### Don't
- Don’t make it dull monochrome SaaS
- Don’t let bright colors become chaotic

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack demos before shrinking
- Keep gradient CTA hierarchy obvious

## 9. Agent Prompt Guide
```text
Design this like ClickUp: bright productivity SaaS with violet-pink gradient accents, white rounded dashboard cards, polished all-in-one work-platform demos, and modern energetic typography.
```
