# Mux Design System
> Video infrastructure platform for developers with a dark engineering aesthetic — deep charcoal, electric pink accents, and video-player-first UI patterns.

---

## 1. Visual Theme & Atmosphere
Mux is how developers add professional video to their products. The brand is confident and a little punk — a vibrant pink that stands out against deep charcoal backgrounds. The UI is clean and developer-friendly: analytics dashboards with real-time playback quality metrics, asset management, and embedded player previews. The aesthetic communicates both technical depth and creative energy.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FA50B5` | Brand pink, CTAs, active elements |
| `--color-primary-dark` | `#D4368D` | Hover/active primary |
| `--color-primary-light` | `#FDE8F5` | Light badges (light mode) |
| `--color-bg-base` | `#121212` | App background |
| `--color-bg-card` | `#1C1C1C` | Card surfaces |
| `--color-bg-elevated` | `#252525` | Dropdowns, tooltips |
| `--color-bg-player` | `#000000` | Video player background |
| `--color-border` | `#333333` | Default borders |
| `--color-text-primary` | `#F5F5F5` | Headings, primary text |
| `--color-text-secondary` | `#A0A0A0` | Labels, secondary |
| `--color-text-muted` | `#606060` | Placeholder, disabled |
| `--color-success` | `#34D399` | Healthy playback, passed |
| `--color-warning` | `#FBBF24` | Buffering, rebuffering alerts |
| `--color-error` | `#F87171` | Playback errors, failed |
| `--color-chart-video` | `#FA50B5` | Video quality data series |
| `--color-chart-rebuffer` | `#FBBF24` | Rebuffering data series |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'IBM Plex Mono', monospace;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 28px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 28px | 700 | 1.25 |
| Section Header | 16px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label | 12px | 500 | 1.4 |
| Metric Value | 32px | 700 | 1.2 |
| Code / Asset ID | 13px | 400 | 1.5 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #FA50B5;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 9px 18px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #D4368D; }

/* Video Player Shell */
.player-shell {
  background: #000000;
  border-radius: 8px;
  overflow: hidden;
  position: relative;
  aspect-ratio: 16/9;
}
.player-controls {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 12px 16px;
  background: linear-gradient(transparent, rgba(0,0,0,0.7));
  display: flex;
  align-items: center;
  gap: 10px;
}

/* Asset Card */
.asset-card {
  background: #1C1C1C;
  border: 1px solid #333333;
  border-radius: 8px;
  overflow: hidden;
  cursor: pointer;
  transition: border-color 0.15s;
}
.asset-card:hover { border-color: #FA50B5; }
.asset-card__thumbnail {
  aspect-ratio: 16/9;
  background: #000000;
  position: relative;
}
.asset-card__info {
  padding: 10px 12px;
}
.asset-card__name {
  font-size: 13px;
  font-weight: 600;
  color: #F5F5F5;
}
.asset-card__meta {
  font-size: 11px;
  color: #A0A0A0;
  font-family: var(--font-mono);
  margin-top: 2px;
}

/* Quality Metric Card */
.metric-card {
  background: #1C1C1C;
  border: 1px solid #333333;
  border-radius: 8px;
  padding: 16px 20px;
}
.metric-card__value {
  font-size: 32px;
  font-weight: 700;
  color: #FA50B5;
  font-family: var(--font-mono);
}
.metric-card__label {
  font-size: 12px;
  color: #A0A0A0;
  margin-top: 4px;
}

/* Playback Error Badge */
.error-badge {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  padding: 3px 8px;
  border-radius: 4px;
  background: rgba(248,113,113,0.12);
  color: #F87171;
  font-size: 11px;
  font-weight: 600;
  font-family: var(--font-mono);
  border: 1px solid rgba(248,113,113,0.2);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Icon gaps |
| `--spacing-sm` | `8px` | Compact padding |
| `--spacing-md` | `12px` | Card inner spacing |
| `--spacing-lg` | `16px` | Section gaps |
| `--spacing-xl` | `24px` | Page padding |
| `--radius-sm` | `4px` | Error badges |
| `--radius-md` | `8px` | Buttons, cards |
| `--sidebar-width` | `240px` | Navigation sidebar |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-player { box-shadow: 0 8px 32px rgba(0,0,0,0.7); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.65); }
```

## 7. Do's and Don'ts
**Do:**
- Make video thumbnails 16:9 aspect ratio always
- Use pink (#FA50B5) for primary metrics and CTAs — it's the brand's most distinctive element
- Display asset IDs and technical metadata in monospace
- Show video quality scores (MUX Score) prominently

**Don't:**
- Don't use light backgrounds anywhere in the dashboard
- Don't use pink for error states — use red (#F87171) instead
- Don't crop or letterbox video thumbnails — always 16:9

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Asset list only; player expands to full screen |
| Tablet | 768px | Two-column asset grid; analytics simplified |
| Desktop | 1024px | Sidebar + full asset grid + analytics panels |
| Wide | 1440px | Wider analytics charts, more data per view |

## 9. Agent Prompt Guide
```
You are designing for Mux — video infrastructure for developers.
Use a deep dark background (#121212) with card surfaces at #1C1C1C.
Primary brand color is hot pink (#FA50B5) — bold, confident, and distinctive.
Video thumbnails are always 16:9 aspect ratio cards with dark backgrounds.
Metric cards display large pink monospace numbers (playback score, view count, rebuffer rate).
Asset IDs and technical metadata use monospace 11–13px in muted text.
Tone is developer-confident, video-native, and slightly punk.
```
