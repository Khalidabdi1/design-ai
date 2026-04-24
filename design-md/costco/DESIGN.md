# Costco Design System

> Membership retail with practical red-blue branding and warehouse-scale merchandising. Costco's public site uses white surfaces, brand blue and red, straightforward retail hierarchy, and practical shopping modules.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Costco feels like **bulk retail and membership shopping expressed through highly practical ecommerce structure**.
### Mood & Feeling
- Practical
- Value-oriented
- Retail-direct
- Mainstream
- Utility-first
### Design Density
**High density.** The site supports broad catalog browsing and deal discovery.
### Visual Character
- White retail frame
- Blue and red brand accents
- Utility-focused product and category modules
- Little decorative excess

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--costco-blue` | `#005DAA` | Primary brand accent |
| `--costco-red` | `#E31837` | Sale/highlight accent |
| `--costco-white` | `#FFFFFF` | Main surface |
| `--costco-surface` | `#F6F7F9` | Background |
| `--costco-ink` | `#111827` | Text |
| `--costco-muted` | `#6B7280` | Secondary text |
| `--costco-border` | `#E5E7EB` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Helvetica Neue", Arial, sans-serif;
--font-sans: "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `48/700`, H1 `34/700`, H2 `26/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use simple retail typography optimized for scanning, price comparison, and membership utility.

## 4. Component Stylings
```css
.button-primary { background:#005daa; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111827; border:1px solid #e5e7eb; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #e5e7eb; border-radius:14px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Prioritize shopping, categories, and deals
- Keep membership value and merchandising close together
- Favor utility over polish-first presentation

## 6. Depth & Elevation
Costco uses **minimal retail depth**, relying more on sections and borders than shadows.

## 7. Do's and Don'ts
### Do
- Keep it practical, value-driven, and easy to browse
- Use blue and red as recognizable retail cues
- Preserve mainstream ecommerce clarity
### Don't
- Don’t over-luxurize the presentation
- Don’t bury deal and category access

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack deal modules and simplify dense retail navigation
- Keep cart and category actions obvious

## 9. Agent Prompt Guide
```text
Design this like Costco: practical membership-retail UI with white surfaces, blue-and-red brand accents, straightforward shopping hierarchy, simple cards, and value-first ecommerce clarity.
```
