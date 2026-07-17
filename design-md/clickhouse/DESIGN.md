# ClickHouse Design System
> Open-source columnar OLAP database with a bold yellow brand, dark developer console aesthetic, and analytics-query-first UI.

---

## 1. Visual Theme & Atmosphere
ClickHouse is one of the fastest analytical databases in the world. The brand is assertive — a vivid yellow against dark surfaces that commands attention and signals performance. The UI is built for data engineers and analysts: SQL editors, query result tables, cluster monitoring dashboards, and schema explorers. The design aesthetic is modern and technical, balancing the depth of an enterprise database tool with a startup-polished interface.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FACC15` | Brand yellow, CTAs, highlights |
| `--color-primary-dark` | `#D4A800` | Hover/active |
| `--color-primary-dim` | `rgba(250,204,21,0.12)` | Subtle highlight backgrounds |
| `--color-bg-base` | `#0F1117` | Console background |
| `--color-bg-sidebar` | `#0A0C12` | Left nav |
| `--color-bg-card` | `#171B26` | Cards, panels |
| `--color-bg-elevated` | `#1E2333` | Dropdowns, modals |
| `--color-bg-code` | `#0A0C12` | SQL editor background |
| `--color-border` | `#252A3A` | Default borders |
| `--color-border-subtle` | `#1A1F2E` | Subtle dividers |
| `--color-text-primary` | `#E8EDF4` | Headings, primary text |
| `--color-text-secondary` | `#7D8FAB` | Labels, meta |
| `--color-text-muted` | `#3D4F6A` | Placeholders, disabled |
| `--color-success` | `#22C55E` | Query success, healthy |
| `--color-error` | `#F87171` | Query error, failed |
| `--color-warning` | `#F59E0B` | Warning, degraded |
| `--color-perf-fast` | `#22C55E` | Fast query indicator |
| `--color-perf-slow` | `#F87171` | Slow query indicator |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 13px;
--font-size-md: 15px;
--font-size-lg: 18px;
--font-size-xl: 22px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--line-height-tight: 1.3;
--line-height-base: 1.5;
--line-height-code: 1.65;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Console Title | 22px | 600 | 1.3 |
| Section Header | 15px | 600 | 1.4 |
| Table Header | 12px | 600 | 1.4 |
| Body / Labels | 13px | 400 | 1.5 |
| SQL Code | 12px | 400 | 1.65 |
| Metric Value | 24px | 700 | 1.2 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #FACC15;
  color: #0F1117;
  border: none;
  border-radius: 6px;
  padding: 8px 18px;
  font-size: 13px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #D4A800; }

/* SQL Editor */
.sql-editor {
  background: #0A0C12;
  border: 1px solid #252A3A;
  border-radius: 8px;
  overflow: hidden;
}
.sql-editor__header {
  background: #171B26;
  padding: 8px 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid #252A3A;
}
.sql-editor__label {
  font-size: 11px;
  font-weight: 600;
  color: #FACC15;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-family: var(--font-mono);
}
.sql-editor__body {
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 12px;
  color: #E8EDF4;
  line-height: 1.65;
  min-height: 120px;
}
/* SQL Syntax */
.sql-keyword { color: #FACC15; font-weight: 600; }
.sql-table { color: #61AFEF; }
.sql-string { color: #98C379; }
.sql-number { color: #E5C07B; }
.sql-comment { color: #3D4F6A; font-style: italic; }

/* Query Result Table */
.result-table { width: 100%; border-collapse: collapse; font-size: 12px; }
.result-table th {
  background: #1E2333;
  border-bottom: 1px solid #252A3A;
  padding: 8px 14px;
  font-size: 11px;
  font-weight: 600;
  color: #7D8FAB;
  text-align: left;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  font-family: var(--font-mono);
  white-space: nowrap;
}
.result-table td {
  padding: 7px 14px;
  color: #E8EDF4;
  border-bottom: 1px solid #1A1F2E;
  font-family: var(--font-mono);
  white-space: nowrap;
}
.result-table tr:hover td { background: #1E2333; }

/* Query Stats Bar */
.query-stats {
  display: flex;
  align-items: center;
  gap: 20px;
  padding: 6px 16px;
  background: #171B26;
  border-top: 1px solid #252A3A;
  font-size: 11px;
  font-family: var(--font-mono);
}
.query-stat { color: #7D8FAB; }
.query-stat span { color: #FACC15; font-weight: 600; }
.query-stat--time span { color: #22C55E; }
.query-stat--rows span { color: #E8EDF4; }

/* Metric Card */
.metric-card {
  background: #171B26;
  border: 1px solid #252A3A;
  border-radius: 8px;
  padding: 20px;
}
.metric-card__label {
  font-size: 11px;
  font-weight: 600;
  color: #7D8FAB;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  margin-bottom: 8px;
}
.metric-card__value {
  font-size: 28px;
  font-weight: 700;
  color: #E8EDF4;
  font-family: var(--font-mono);
}
.metric-card__unit { font-size: 14px; color: #7D8FAB; margin-left: 4px; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Tight element gaps |
| `--spacing-sm` | `8px` | Card compact spacing |
| `--spacing-md` | `12px` | Panel inner spacing |
| `--spacing-lg` | `20px` | Card padding |
| `--spacing-xl` | `32px` | Page gutter |
| `--sidebar-width` | `240px` | Left navigation |
| `--radius-sm` | `4px` | Small elements |
| `--radius-md` | `6px` | Buttons |
| `--radius-lg` | `8px` | Editor, cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.7); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Use yellow (#FACC15) for SQL keywords, CTA buttons, and query editor headers
- SQL keywords are bold yellow; table names are blue; strings are green
- Query stats bar shows execution time in green, row count in white, bytes scanned in secondary
- Result tables use monospace font — this is raw data output

**Don't:**
- Don't use yellow for error states — use red (#F87171)
- Don't truncate column values in result tables — add horizontal scroll instead
- Don't omit query execution time — it's the central metric of a performance database

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Read-only query results; editor hidden |
| Tablet | 768px | Compact editor + scrollable results |
| Desktop | 1024px | Full editor + result table |
| Wide | 1440px | Schema sidebar + editor + results |

## 9. Agent Prompt Guide
```
You are designing for ClickHouse — high-performance OLAP database console.
Use a deep dark background (#0F1117) with card surfaces at #171B26.
Brand yellow (#FACC15) drives SQL keywords, CTA buttons, and editor header labels.
The SQL editor has a dark background (#0A0C12) with a yellow "SQL" header label; syntax highlighting: yellow keywords, blue table names, green strings, amber numbers.
Query result tables use monospace font with a dark header row; execution stats appear below in a stats bar (time in green, rows in white).
Metric cards display large monospace numbers with a muted label and unit.
Tone is developer-precise, analytics-forward, performance-obsessed, and database-native.
```
