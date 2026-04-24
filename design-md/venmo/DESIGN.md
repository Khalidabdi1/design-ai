# Venmo Design System

> Peer-to-peer payments with bright blue consumer-fintech energy and playful simplicity. Venmo's public site uses its iconic blue, white space, rounded consumer UI, and social payment framing.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Venmo feels like **payments made social, simple, and highly mobile-native**.
### Mood & Feeling
- Friendly
- Social
- Fast
- Youthful
- Clear
### Design Density
**Low to medium density.** The product story is simple and consumer focused.
### Visual Character
- Bright Venmo blue
- White rounded app surfaces
- Phone mockups and social payment flows
- Light, mobile-first confidence

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--venmo-blue` | `#008CFF` | Primary brand accent |
| `--venmo-blue-deep` | `#0074D6` | Hover/support |
| `--venmo-white` | `#FFFFFF` | Main surface |
| `--venmo-surface` | `#F4FAFF` | Soft background |
| `--venmo-ink` | `#0F172A` | Text |
| `--venmo-muted` | `#64748B` | Secondary text |
| `--venmo-border` | `#D9EAF8` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Scto Grotesk", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Scto Grotesk", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `54/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#008cff; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#0f172a; border:1px solid #d9eaf8; border-radius:999px; min-height:44px; padding:0 18px; }
.card { background:#fff; border:1px solid #d9eaf8; border-radius:22px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Lead with app actions and social payment simplicity
- Use phone UI mockups prominently
- Keep the flow concise and mobile-first

## 6. Depth & Elevation
Venmo uses **soft mobile-app card elevation** on bright white and pale-blue surfaces.

## 7. Do's and Don'ts
### Do
- Keep it simple, fast, and social
- Use bright blue decisively
- Preserve friendly mobile payment flows
### Don't
- Don’t make it heavy banking UI
- Don’t overcomplicate with enterprise product framing

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep app download and payment actions prominent
- Preserve phone mockup visibility on small screens

## 9. Agent Prompt Guide
```text
Design this like Venmo: bright blue social-payments UI with rounded white app cards, mobile-first phone mockups, simple fintech messaging, and fast friendly consumer clarity.
```
