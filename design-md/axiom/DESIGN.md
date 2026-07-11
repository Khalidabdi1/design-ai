# Axiom Design System
> Observability and log analytics platform with a dark engineering aesthetic — deep navy, cyan data accents, and query-driven UI.

---

## 1. Visual Theme & Atmosphere
Axiom is built for engineers who live in logs. The design is dark and data-dense, prioritizing visibility of streams, queries, and time-series visualizations. A deep navy/charcoal palette frames bright cyan accents that highlight active queries, metrics, and data points. The UI is information-rich without feeling cluttered — whitespace is strategic, not generous.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#00D4FF` | Cyan accent, CTAs, active states |
| `--color-primary-dark` | `#00AACF` | Hover/pressed cyan |
| `--color-primary-dim` | `rgba(0,212,255,0.12)` | Subtle highlight backgrounds |
| `--color-bg-base` | `#0D1117` | Page/app background |
| `--color-bg-card` | `#161B22` | Card and panel surfaces |
| `--color-bg-elevated` | `#21262D` | Elevated dropdowns, tooltips |
| `--color-bg-input` | `#0D1117` | Input field backgrounds |
| `--color-border` | `#30363D` | Default borders |
| `--color-border-subtle` | `#21262D` | Dividers |
| `--color-text-primary` | `#E6EDF3` | Headings, primary text |
| `--color-text-secondary` | `#8B949E` | Labels, secondary info |
| `--color-text-muted` | `#484F58` | Placeholders, disabled |
| `--color-success` | `#3FB950` | Healthy, success |
| `--color-warning` | `#D29922` | Warning, degraded |
| `--color-error` | `#F85149` | Error, critical |
| `--color-chart-1` | `#00D4FF` | Primary data series |
| `--color-chart-2` | `#7EE787` | Secondary data series |
| `--color-chart-3` | `#F78166` | Tertiary data series |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', 'SF Mono', monospace;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 13px;
--font-size-md: 15px;
--font-size-lg: 18px;
--font-size-xl: 24px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--line-height-tight: 1.25;
--line-height-base: 1.5;
--line-height-code: 1.7;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 24px | 600 | 1.25 |
| Section Header | 18px | 600 | 1.3 |
| Label | 13px | 500 | 1.4 |
| Body | 13px | 400 | 1.5 |
| Log Line | 12px | 400 | 1.7 |
| Caption | 11px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #00D4FF;
  color: #0D1117;
  border: none;
  border-radius: 6px;
  padding: 7px 14px;
  font-size: 13px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.12s ease;
}
.button-primary:hover { background: #00AACF; }

/* Query Input */
.query-input {
  background: #0D1117;
  border: 1px solid #30363D;
  border-radius: 6px;
  padding: 10px 14px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #E6EDF3;
  width: 100%;
  transition: border-color 0.12s;
}
.query-input:focus {
  outline: none;
  border-color: #00D4FF;
  box-shadow: 0 0 0 3px rgba(0,212,255,0.1);
}

/* Log Row */
.log-row {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  padding: 3px 16px;
  font-family: var(--font-mono);
  font-size: 12px;
  line-height: 1.7;
  border-bottom: 1px solid #21262D;
  cursor: pointer;
}
.log-row:hover { background: #161B22; }
.log-row__timestamp { color: #484F58; flex-shrink: 0; }
.log-row__level--error { color: #F85149; }
.log-row__level--warn { color: #D29922; }
.log-row__level--info { color: #00D4FF; }
.log-row__message { color: #E6EDF3; }

/* Metric Card */
.metric-card {
  background: #161B22;
  border: 1px solid #30363D;
  border-radius: 8px;
  padding: 16px 20px;
}
.metric-card__value {
  font-size: 28px;
  font-weight: 600;
  color: #00D4FF;
  font-family: var(--font-mono);
}
.metric-card__label {
  font-size: 12px;
  color: #8B949E;
  margin-top: 4px;
}

/* Dataset Badge */
.dataset-badge {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  padding: 2px 8px;
  border-radius: 4px;
  font-size: 11px;
  font-weight: 600;
  font-family: var(--font-mono);
  background: rgba(0,212,255,0.12);
  color: #00D4FF;
  border: 1px solid rgba(0,212,255,0.25);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Icon padding |
| `--spacing-sm` | `8px` | Inline gaps |
| `--spacing-md` | `12px` | Card inner spacing |
| `--spacing-lg` | `16px` | Panel padding |
| `--spacing-xl` | `24px` | Section gaps |
| `--radius-sm` | `4px` | Badges, small chips |
| `--radius-md` | `6px` | Buttons, inputs |
| `--radius-lg` | `8px` | Cards, panels |
| `--sidebar-width` | `220px` | Left navigation |
| `--log-row-height` | `24px` | Default log line height |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.6); }
.shadow-tooltip { box-shadow: 0 4px 12px rgba(0,0,0,0.7); }
```

## 7. Do's and Don'ts
**Do:**
- Use monospace font for ALL log output, timestamps, and query fields
- Color-code log levels consistently: cyan=info, green=debug, yellow=warn, red=error
- Surface key metrics in large monospace numbers with cyan color
- Show query syntax highlighting in the query editor

**Don't:**
- Don't use light backgrounds — they break focus on data
- Don't overload chart colors — stick to the defined 3-color data palette
- Don't truncate log lines by default — let them wrap or scroll
- Don't use the cyan accent for non-interactive decorative purposes

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Query and log views only; charts collapse |
| Tablet | 768px | Sidebar collapses to icon rail |
| Desktop | 1024px | Full layout: sidebar + query + visualizations |
| Wide | 1440px | Expanded chart panels and log density |

## 9. Agent Prompt Guide
```
You are designing for Axiom — an observability and log analytics platform.
Use a deep dark background (#0D1117 page, #161B22 cards) inspired by GitHub's dark theme.
Primary accent is bright cyan (#00D4FF) — use for CTAs, active states, and key metrics.
Log lines use monospace 12px with color-coded level indicators (cyan info, yellow warn, red error).
Metric cards display large cyan monospace numbers with small muted labels below.
Charts use a 3-color data palette: cyan, green, coral.
Tone is engineering-dense, data-first, and terminal-adjacent.
```
