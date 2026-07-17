# Weaviate Design System
> Open-source vector database with a dark, developer-focused aesthetic — deep navy surfaces, green-teal brand accent, and data-exploration-first UI.

---

## 1. Visual Theme & Atmosphere
Weaviate is an AI-native vector database built for developers building semantic search and generative AI applications. The interface is dark and technical — dense with schema explorers, query consoles, and vector visualization panels. A green-teal accent signals system health and active operations. The design language is precise and data-forward, echoing the terminal aesthetics of developer tooling while remaining navigable for data scientists.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#00D2A0` | Brand teal-green, CTAs, active states |
| `--color-primary-dark` | `#00A880` | Hover/active |
| `--color-primary-dim` | `rgba(0,210,160,0.12)` | Subtle highlights |
| `--color-bg-base` | `#0D1117` | App background |
| `--color-bg-sidebar` | `#141B25` | Left nav |
| `--color-bg-card` | `#1A2230` | Cards, panels |
| `--color-bg-elevated` | `#1F2A3C` | Dropdowns, modals |
| `--color-bg-code` | `#111827` | Code/query areas |
| `--color-border` | `#243047` | Default borders |
| `--color-border-subtle` | `#1A2435` | Subtle dividers |
| `--color-text-primary` | `#E2E8F0` | Headings, primary text |
| `--color-text-secondary` | `#8BA3BE` | Labels, meta |
| `--color-text-muted` | `#4E6680` | Placeholders, disabled |
| `--color-success` | `#00D2A0` | Indexed, healthy |
| `--color-error` | `#F87171` | Error, failed |
| `--color-warning` | `#FBBF24` | Warning, degraded |
| `--color-vector` | `#818CF8` | Vector/embedding accent |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, sans-serif;
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
| Label | 13px | 500 | 1.4 |
| Body | 13px | 400 | 1.5 |
| Code / Query | 12px | 400 | 1.65 |
| Metric Value | 22px | 600 | 1.2 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #00D2A0;
  color: #0D1117;
  border: none;
  border-radius: 6px;
  padding: 8px 18px;
  font-size: 13px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #00A880; }

/* Schema Class Card */
.class-card {
  background: #1A2230;
  border: 1px solid #243047;
  border-radius: 8px;
  padding: 16px;
  cursor: pointer;
  transition: border-color 0.15s;
}
.class-card:hover { border-color: #00D2A0; }
.class-card__name {
  font-size: 14px;
  font-weight: 600;
  color: #E2E8F0;
  margin-bottom: 6px;
}
.class-card__count {
  font-size: 11px;
  color: #8BA3BE;
}
.class-card__count span {
  color: #00D2A0;
  font-weight: 600;
}

/* Query Console */
.query-console {
  background: #111827;
  border: 1px solid #243047;
  border-radius: 8px;
  overflow: hidden;
}
.query-console__header {
  background: #1A2230;
  padding: 8px 16px;
  border-bottom: 1px solid #243047;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.query-console__lang {
  font-size: 11px;
  font-weight: 600;
  color: #00D2A0;
  text-transform: uppercase;
  letter-spacing: 0.08em;
}
.query-console__body {
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 12px;
  color: #E2E8F0;
  line-height: 1.65;
  min-height: 120px;
}

/* Property Row */
.property-row {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 8px 12px;
  border-bottom: 1px solid #1A2435;
  font-size: 12px;
  font-family: var(--font-mono);
}
.property-row__name { color: #E2E8F0; flex: 1; }
.property-row__type { color: #818CF8; }
.property-row__index { color: #00D2A0; font-size: 11px; }

/* Health Badge */
.health-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 10px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
}
.health-badge--healthy { background: rgba(0,210,160,0.12); color: #00D2A0; }
.health-badge--degraded { background: rgba(251,191,36,0.12); color: #FBBF24; }
.health-badge--error { background: rgba(248,113,113,0.12); color: #F87171; }
.health-dot {
  width: 6px; height: 6px;
  border-radius: 50%;
  background: currentColor;
}

/* Input */
.input {
  background: #1A2230;
  border: 1px solid #243047;
  border-radius: 6px;
  padding: 8px 12px;
  font-size: 13px;
  color: #E2E8F0;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #00D2A0;
  box-shadow: 0 0 0 2px rgba(0,210,160,0.15);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Property row gaps |
| `--spacing-sm` | `8px` | Card compact spacing |
| `--spacing-md` | `12px` | Panel inner spacing |
| `--spacing-lg` | `20px` | Card padding |
| `--spacing-xl` | `32px` | Page gutter |
| `--sidebar-width` | `240px` | Left navigation |
| `--radius-sm` | `4px` | Badges |
| `--radius-md` | `6px` | Buttons, inputs |
| `--radius-lg` | `8px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.4); }
.shadow-modal { box-shadow: 0 12px 40px rgba(0,0,0,0.6); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.5); }
```

## 7. Do's and Don'ts
**Do:**
- Use teal-green (#00D2A0) for healthy states, active classes, and primary actions
- Show property types in indigo/purple to distinguish them from property names
- Query console uses monospace font with a dark code background
- Health badges use a dot + label with color-semantic backgrounds

**Don't:**
- Don't use bright colors for non-semantic purposes — this is a technical console
- Don't omit monospace font for schema properties and query results
- Don't show vector embeddings as raw numbers — use dimensionality indicators

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Schema list only; console hidden |
| Tablet | 768px | Schema + compact query panel |
| Desktop | 1024px | Full sidebar + schema + console |
| Wide | 1440px | Multi-panel with vector visualization |

## 9. Agent Prompt Guide
```
You are designing for Weaviate — an open-source vector database platform.
Use a deep dark background (#0D1117) with card surfaces at #1A2230.
Teal-green (#00D2A0) marks healthy states, active schema classes, and primary actions.
Schema classes are shown as cards with class name and object count; vector properties show in indigo (#818CF8).
Query console has a dark code background (#111827) with a monospace font and a teal language label.
Health badges are pill-shaped with a dot indicator and semantic background tinting.
Tone is developer-precise, data-forward, and AI-native.
```
