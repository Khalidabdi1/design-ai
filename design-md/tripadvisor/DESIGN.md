# Tripadvisor Design System

> Travel discovery with content-heavy browsing, green brand cues, and review-driven utility. Tripadvisor's public site uses white surfaces, black text, rounded search controls, and the familiar Tripadvisor green (`#34E0A1`) with review-and-discovery framing.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Tripadvisor feels like **travel recommendations and reviews organized into a consumer discovery engine**.
### Mood & Feeling
- Helpful
- Review-driven
- Travel curious
- Mainstream
- Utility-first
### Design Density
**Medium density.** Review categories and destination modules are numerous but legible.
### Visual Character
- White interface with green highlights
- Search-led travel discovery
- Rounded modules and content cards
- Reviews and guides framed as first-class content

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--ta-green` | `#34E0A1` | Primary brand accent |
| `--ta-black` | `#111111` | Text |
| `--ta-white` | `#FFFFFF` | Main surface |
| `--ta-surface` | `#F7F7F7` | Background |
| `--ta-muted` | `#6B7280` | Secondary text |
| `--ta-border` | `#E5E5E5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Trip Sans", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Trip Sans", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `52/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use sturdy, mainstream travel-discovery typography with strong readability.

## 4. Component Stylings
```css
.button-primary { background:#111; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:600; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e5e5; border-radius:999px; min-height:44px; padding:0 18px; }
.card { background:#fff; border:1px solid #e5e5e5; border-radius:20px; }
.search-shell { background:#fff; border:1px solid #e5e5e5; border-radius:999px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Lead with search, reviews, and travel categories
- Keep destination and attraction content easy to browse
- Let content density remain organized through simple cards and tabs

## 6. Depth & Elevation
Tripadvisor uses **minimal content-card elevation** with strong emphasis on search and review browsing.

## 7. Do's and Don'ts
### Do
- Keep it review-first and search-led
- Use green as a light brand cue
- Preserve broad destination browsing clarity
### Don't
- Don’t make it luxury-travel editorial
- Don’t crowd cards with too much decorative chrome

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep search obvious
- Stack content shelves and destination modules cleanly

## 9. Agent Prompt Guide
```text
Design this like Tripadvisor: white travel-discovery UI with rounded search controls, review-driven content cards, light green brand accents, and mainstream browse-first marketplace clarity.
```
