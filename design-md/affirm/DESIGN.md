# Affirm Design System

> Buy-now-pay-later fintech with deep blue trust, consumer-retail clarity, and installment-friendly messaging. Affirm's public site uses navy and blue accents, white surfaces, rounded cards, and purchase-focused financial education.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Affirm feels like **consumer financing made transparent, modern, and approachable**.
### Mood & Feeling
- Trustworthy
- Consumer-friendly
- Clear
- Financially modern
- Purchase-oriented
### Design Density
**Medium density.** Merchant and payment-plan information is structured and easy to scan.
### Visual Character
- Deep blue trust frame
- White rounded cards
- Installment and purchase education modules
- Clean consumer-fintech polish

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--affirm-blue` | `#1A5CFF` | Primary action accent |
| `--affirm-navy` | `#102A43` | Trust anchor |
| `--affirm-white` | `#FFFFFF` | Main surface |
| `--affirm-surface` | `#F5F8FF` | Soft background |
| `--affirm-ink` | `#102A43` | Text |
| `--affirm-muted` | `#6B7280` | Secondary text |
| `--affirm-border` | `#DCE5F5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Calibre", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Calibre", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `54/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#1a5cff; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#102a43; border:1px solid #dce5f5; border-radius:999px; min-height:44px; padding:0 18px; }
.card { background:#fff; border:1px solid #dce5f5; border-radius:20px; box-shadow:0 12px 24px rgba(16,42,67,.06); }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Lead with how-pay-over-time works
- Keep merchants, terms, and trust cues simple
- Use blue to reinforce transparency and action

## 6. Depth & Elevation
Affirm uses **light fintech-card elevation** with rounded educational and merchant modules.

## 7. Do's and Don'ts
### Do
- Keep it transparent, consumer-readable, and trust-first
- Use navy and blue consistently
- Preserve shopping-and-payment clarity
### Don't
- Don’t make it flashy crypto or startup-finance UI
- Don’t bury education and terms beneath aggressive promo styling

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep payment-plan explanations and CTAs close together
- Stack merchant and education cards cleanly

## 9. Agent Prompt Guide
```text
Design this like Affirm: deep-blue consumer-finance UI with rounded white cards, clear pay-over-time education, trust-first messaging, and simple mainstream fintech purchase flows.
```
