# Mapbox Design System
> Maps and location developer platform with a dark cartographic aesthetic — deep charcoal surfaces, electric teal map accents, and geo-data-first UI.

---

## 1. Visual Theme & Atmosphere
Mapbox merges the precision of cartography with the flexibility of a developer platform. The visual identity is dark and technical, anchored by the map canvas itself — a rich dark cartographic style with carefully chosen color layers. UI chrome is minimal and subordinate to the map: dark sidebars, compact controls, and teal highlights that echo the water and route colors of their signature dark map style.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#1DAADC` | Brand teal, CTAs, interactive elements |
| `--color-primary-dark` | `#1589B8` | Hover/active states |
| `--color-primary-light` | `#E3F5FB` | Light mode accents |
| `--color-map-water` | `#193B50` | Map water fill (dark style) |
| `--color-map-land` | `#1A1A2E` | Map land fill (dark style) |
| `--color-map-road` | `#2C3E50` | Road network |
| `--color-map-highlight` | `#1DAADC` | Active route, selected feature |
| `--color-bg-base` | `#191919` | App sidebar background |
| `--color-bg-card` | `#232323` | Card surfaces |
| `--color-bg-elevated` | `#2D2D2D` | Dropdowns, tooltips |
| `--color-border` | `#383838` | Default borders |
| `--color-text-primary` | `#F2F2F2` | Headings, primary labels |
| `--color-text-secondary` | `#9A9A9A` | Secondary info |
| `--color-text-muted` | `#5A5A5A` | Disabled, placeholders |
| `--color-success` | `#27AE60` | Success, safe routes |
| `--color-warning` | `#E67E22` | Traffic, caution zones |
| `--color-error` | `#E74C3C` | Errors, blocked routes |

## 3. Typography Rules
```css
--font-sans: 'Relative', 'Inter', -apple-system, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 24px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 24px | 700 | 1.25 |
| Section Header | 16px | 600 | 1.4 |
| Map Label | 12px | 600 | 1.2 |
| Body | 14px | 400 | 1.5 |
| UI Label | 12px | 500 | 1.4 |
| Code | 13px | 400 | 1.6 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #1DAADC;
  color: #FFFFFF;
  border: none;
  border-radius: 4px;
  padding: 8px 16px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #1589B8; }

/* Map Control Button */
.map-control {
  width: 36px;
  height: 36px;
  border-radius: 4px;
  background: #232323;
  border: 1px solid #383838;
  color: #F2F2F2;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: background 0.12s;
}
.map-control:hover { background: #2D2D2D; }
.map-control + .map-control { border-top: none; border-radius: 0; }
.map-control:last-child { border-radius: 0 0 4px 4px; }
.map-control:first-child { border-radius: 4px 4px 0 0; }

/* Geocoder Input */
.geocoder-input {
  background: #232323;
  border: 1px solid #383838;
  border-radius: 4px;
  padding: 10px 14px;
  font-size: 14px;
  color: #F2F2F2;
  width: 100%;
}
.geocoder-input:focus {
  outline: none;
  border-color: #1DAADC;
  box-shadow: 0 0 0 2px rgba(29,170,220,0.2);
}

/* Feature Popup */
.map-popup {
  background: #232323;
  border: 1px solid #383838;
  border-radius: 6px;
  padding: 12px 16px;
  box-shadow: 0 4px 16px rgba(0,0,0,0.6);
  min-width: 180px;
}
.map-popup__title {
  font-size: 14px;
  font-weight: 600;
  color: #F2F2F2;
  margin-bottom: 4px;
}
.map-popup__detail {
  font-size: 12px;
  color: #9A9A9A;
}

/* Coordinate Badge */
.coord-badge {
  display: inline-flex;
  gap: 6px;
  padding: 4px 8px;
  background: #191919;
  border: 1px solid #383838;
  border-radius: 4px;
  font-family: var(--font-mono);
  font-size: 11px;
  color: #9A9A9A;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Control button gaps |
| `--spacing-sm` | `8px` | Compact padding |
| `--spacing-md` | `12px` | Panel inner spacing |
| `--spacing-lg` | `16px` | Sidebar sections |
| `--spacing-xl` | `24px` | Page gutter |
| `--sidebar-width` | `320px` | Geocoder + controls sidebar |
| `--control-size` | `36px` | Map control button fixed size |
| `--radius-sm` | `4px` | Buttons, controls, badges |
| `--radius-md` | `6px` | Popups, cards |

## 6. Depth & Elevation
```css
.shadow-popup { box-shadow: 0 4px 16px rgba(0,0,0,0.6); }
.shadow-sidebar { box-shadow: 2px 0 8px rgba(0,0,0,0.4); }
.shadow-control { box-shadow: 0 2px 4px rgba(0,0,0,0.5); }
```

## 7. Do's and Don'ts
**Do:**
- Let the map canvas be the dominant visual element — UI should recede
- Use the teal accent (#1DAADC) only for interactive map elements and primary CTAs
- Keep coordinate displays and data in monospace
- Stack map controls vertically as a connected group (zoom in/out pattern)

**Don't:**
- Don't use heavy sidebar styling that competes with the map
- Don't use rounded corners larger than 6px — cartographic tools prefer precision
- Don't display more than 3–4 lines of detail in a map popup
- Don't use warm colors for non-traffic/alert contexts

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Full-screen map, sidebar as bottom sheet |
| Tablet | 768px | Side panel overlay on map edge |
| Desktop | 1024px | Fixed sidebar + full map view |
| Wide | 1440px | Wider sidebar with analytics panels |

## 9. Agent Prompt Guide
```
You are designing for Mapbox — maps and location developer platform.
Use a dark sidebar (#191919) that frames a dark cartographic map canvas.
Primary accent is teal (#1DAADC) — for CTAs, active routes, and selected features.
Map controls are 36px square, grouped vertically with shared borders.
Popups over the map are dark cards with 1px borders and a subtle shadow.
Coordinate and geo data displays use monospace at 11–12px.
Keep UI chrome minimal — the map is always the hero.
Tone is cartographic, technical, and spatially-precise.
```
