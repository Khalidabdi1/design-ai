# Expedia Design System

> Travel booking with royal-blue trust signals, search-led layouts, and marketplace clarity. Expedia's public site uses strong blue framing, white cards, rounded search modules, and broad travel category browsing.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Expedia feels like **travel planning organized into a high-trust booking marketplace**.
### Mood & Feeling
- Travel-ready
- Mainstream
- Helpful
- Search-first
- Trustworthy
### Design Density
**Medium density.** Many travel products and offers are present, but the search-led frame organizes them.
### Visual Character
- Royal blue trust anchors
- White cards and search surfaces
- Rounded trip-planning modules
- Large destination imagery

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--expedia-blue` | `#1668E3` | Primary action |
| `--expedia-blue-deep` | `#003E9A` | Strong support blue |
| `--expedia-white` | `#FFFFFF` | Main surface |
| `--expedia-surface` | `#F5F8FF` | Background |
| `--expedia-ink` | `#1F2937` | Text |
| `--expedia-muted` | `#6B7280` | Secondary text |
| `--expedia-border` | `#DCE5F5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `54/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use highly readable booking-marketplace typography with strong search and conversion hierarchy.

## 4. Component Stylings
```css
.button-primary { background:#1668e3; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#1f2937; border:1px solid #dce5f5; border-radius:999px; min-height:44px; padding:0 18px; }
.card { background:#fff; border:1px solid #dce5f5; border-radius:20px; }
.search-shell { background:#fff; border:1px solid #dce5f5; border-radius:20px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Lead with trip search and travel category selection
- Keep recommendation and promo cards clearly segmented
- Use destination imagery to add aspiration without losing utility

## 6. Depth & Elevation
Expedia uses **search-card elevation** with clean rounded booking modules.

## 7. Do's and Don'ts
### Do
- Keep travel search central
- Use blue as a trust anchor
- Preserve marketplace scanability
### Don't
- Don’t overdo luxury editorial styling
- Don’t hide booking actions under decorative imagery

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack booking inputs and recommendation cards
- Keep search CTA visible at all times

## 9. Agent Prompt Guide
```text
Design this like Expedia: blue-led travel-booking marketplace UI with white rounded search cards, practical trip-planning hierarchy, destination imagery, and high-trust mainstream booking design.
```
