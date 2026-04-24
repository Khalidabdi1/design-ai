# Intercom Design System

> Customer support software with AI-era warmth, rounded surfaces, and a conversational product tone. Intercom's public site uses clean typography, white and soft-neutral surfaces, black anchors, and warm orange support accents.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Intercom feels like **support software made more human and more current**.
### Mood & Feeling
- Friendly
- Conversational
- SaaS-modern
- Support-centered
- AI-augmented
### Design Density
**Medium density.** Product detail is present, but the site remains calm and approachable.
### Visual Character
- White and warm-neutral base
- Rounded cards and UI demos
- Black anchor text with orange support accents
- Human-centered support visuals

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--intercom-black` | `#111111` | Primary anchor |
| `--intercom-orange` | `#FF6B3D` | Warm action accent |
| `--intercom-white` | `#FFFFFF` | Cards and canvas |
| `--intercom-surface` | `#F8F5F1` | Warm background |
| `--intercom-ink` | `#1F2937` | Primary text |
| `--intercom-muted` | `#6B7280` | Secondary text |
| `--intercom-border` | `#E7E0D8` | Borders |
| `--intercom-blue-soft` | `#E9F1FF` | AI/support tint |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `56/700`, H1 `40/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use friendly, contemporary typography that keeps support workflows readable and human.

## 4. Component Stylings
```css
.button-primary { background:#111; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#111; border:1px solid #e7e0d8; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #e7e0d8; border-radius:24px; box-shadow:0 12px 24px rgba(17,17,17,.06); }
.input { background:#fff; border:1px solid #e7e0d8; border-radius:14px; min-height:46px; padding:12px 14px; }
```
### Component Notes
- Support UI demos should feel visible and human
- Orange is supportive, not overwhelming

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Lead with AI-helpdesk positioning
- Use demo cards and conversation UI
- Keep support outcomes simple and scannable

## 6. Depth & Elevation
Intercom uses **soft rounded elevation** with warm-neutral contrast.

## 7. Do's and Don'ts
### Do
- Keep it conversational and current
- Use rounded surfaces and warm neutrals
- Preserve product clarity in chat/helpdesk demos
### Don't
- Don’t make it cold enterprise ticketing software
- Don’t overuse orange or novelty AI styling

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack demo UIs cleanly
- Keep CTAs and proof close together

## 9. Agent Prompt Guide
```text
Design this like Intercom: warm-neutral support SaaS with rounded white cards, black anchor CTAs, subtle orange accents, modern conversational UI demos, and approachable AI-helpdesk clarity.
```
