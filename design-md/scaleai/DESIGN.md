# Scale AI Design System
> AI data platform and model evaluation infrastructure with a clean enterprise aesthetic — white and slate surfaces, vivid purple-indigo accents, and data-labeling-first UI.

---

## 1. Visual Theme & Atmosphere
Scale AI operates at the frontier of AI infrastructure — data annotation, model evaluation, and enterprise AI solutions. The design is clean, authoritative, and enterprise-grade: white and light slate surfaces with a confident indigo accent. The UI conveys technical precision and trust — complex data workflows are presented clearly, with clear status hierarchies and task-management patterns that work at massive scale.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#5C4EE5` | Brand indigo, CTAs, active states |
| `--color-primary-dark` | `#4839C8` | Hover/active primary |
| `--color-primary-light` | `#EEF0FD` | Light backgrounds, badges |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F7F8FC` | Section backgrounds, table rows |
| `--color-bg-dark` | `#0D0E1A` | Dark hero sections |
| `--color-text-primary` | `#0D0E1A` | Headings, primary |
| `--color-text-secondary` | `#4A4F6A` | Body text, labels |
| `--color-text-muted` | `#9298B4` | Meta, timestamps |
| `--color-border` | `#DEE1EF` | Default borders |
| `--color-border-subtle` | `#F0F2FA` | Dividers |
| `--color-success` | `#22C55E` | Completed, approved |
| `--color-warning` | `#F59E0B` | Pending review |
| `--color-error` | `#EF4444` | Rejected, failed |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'IBM Plex Mono', monospace;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 15px;
--font-size-md: 17px;
--font-size-lg: 22px;
--font-size-xl: 30px;
--font-size-2xl: 40px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.2;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Hero Title | 40px | 700 | 1.2 |
| Page Title | 30px | 700 | 1.25 |
| Section Header | 22px | 600 | 1.3 |
| Card Title | 17px | 600 | 1.4 |
| Body | 15px | 400 | 1.5 |
| Label | 13px | 500 | 1.4 |
| Caption / Meta | 11px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #5C4EE5;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 11px 22px;
  font-size: 15px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #4839C8; }

/* Task Card */
.task-card {
  background: #FFFFFF;
  border: 1px solid #DEE1EF;
  border-radius: 10px;
  padding: 20px;
  cursor: pointer;
  transition: box-shadow 0.15s;
}
.task-card:hover { box-shadow: 0 4px 16px rgba(0,0,0,0.07); }
.task-card__type {
  font-size: 11px;
  font-weight: 700;
  color: #5C4EE5;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  margin-bottom: 6px;
}
.task-card__title {
  font-size: 17px;
  font-weight: 600;
  color: #0D0E1A;
}

/* Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  padding: 3px 9px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
}
.status-badge--completed { background: rgba(34,197,94,0.1); color: #16A34A; }
.status-badge--pending { background: rgba(245,158,11,0.1); color: #D97706; }
.status-badge--rejected { background: rgba(239,68,68,0.1); color: #DC2626; }
.status-badge--in-progress { background: rgba(92,78,229,0.1); color: #5C4EE5; }

/* Metric Card */
.metric-card {
  background: #FFFFFF;
  border: 1px solid #DEE1EF;
  border-radius: 10px;
  padding: 24px;
}
.metric-card__value {
  font-size: 40px;
  font-weight: 700;
  color: #0D0E1A;
}
.metric-card__label {
  font-size: 14px;
  color: #9298B4;
  margin-top: 4px;
}

/* Data Table Row */
.table-row {
  display: grid;
  padding: 12px 16px;
  border-bottom: 1px solid #F0F2FA;
  align-items: center;
  font-size: 14px;
  color: #4A4F6A;
  transition: background 0.08s;
}
.table-row:hover { background: #F7F8FC; }

/* Input */
.input {
  border: 1.5px solid #DEE1EF;
  border-radius: 8px;
  padding: 10px 14px;
  font-size: 15px;
  color: #0D0E1A;
  background: #FFFFFF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #5C4EE5;
  box-shadow: 0 0 0 3px rgba(92,78,229,0.12);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Badge padding |
| `--spacing-sm` | `8px` | Row internal gaps |
| `--spacing-md` | `16px` | Card inner spacing |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Page gutter |
| `--spacing-2xl` | `64px` | Hero section padding |
| `--max-content` | `1200px` | Content max-width |
| `--radius-sm` | `6px` | Badges |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `10px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.05); }
.shadow-hover { box-shadow: 0 4px 16px rgba(0,0,0,0.07); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.12); }
```

## 7. Do's and Don'ts
**Do:**
- Use uppercase 11px labels for task type identifiers in indigo
- Show task completion rates as large bold numbers in metric cards
- Semantic status badges are essential — every task needs a visible state
- Data tables should alternate hover state with subtle background for scanability

**Don't:**
- Don't use dark backgrounds in the main product UI (hero sections excepted)
- Don't mix the indigo brand color with the semantic status colors
- Don't show raw model output without human-readable summaries

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Task list with simplified cards |
| Tablet | 768px | Two-column task grid |
| Desktop | 1024px | Sidebar + task grid + detail panel |
| Wide | 1440px | Full width with expanded data tables |

## 9. Agent Prompt Guide
```
You are designing for Scale AI — AI data platform and model evaluation.
Use a white background with light slate surfaces (#F7F8FC for sections).
Primary accent is indigo (#5C4EE5) — for CTAs, task type labels, and active states.
Task type labels are 11px uppercase indigo above card titles.
Metric cards show large bold black numbers with muted labels.
Status badges use semantic colors: green=completed, orange=pending, red=rejected, indigo=in-progress.
Tone is enterprise-grade, precision-focused, and AI-infrastructure-authoritative.
```
