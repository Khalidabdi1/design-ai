# Weights & Biases (W&B) Design System
> ML experiment tracking and model monitoring platform with a dark research aesthetic — deep navy, golden-yellow run markers, and experiment-first data UI.

---

## 1. Visual Theme & Atmosphere
Weights & Biases is where machine learning experiments live. The design is optimized for researchers and engineers who need to compare runs, track metrics over time, and surface model behavior. The aesthetic is dark and data-dense, with golden-yellow accent lines that trace experiment runs across charts. The UI combines a terminal-adjacent precision with enough visual richness to make model comparisons legible at a glance.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FFBE00` | Brand gold, run traces, CTAs |
| `--color-primary-dark` | `#D9A000` | Hover/active gold |
| `--color-primary-dim` | `rgba(255,190,0,0.12)` | Subtle gold backgrounds |
| `--color-run-1` | `#FF7043` | Run color palette – coral |
| `--color-run-2` | `#42A5F5` | Run color palette – blue |
| `--color-run-3` | `#66BB6A` | Run color palette – green |
| `--color-run-4` | `#AB47BC` | Run color palette – purple |
| `--color-run-5` | `#26C6DA` | Run color palette – cyan |
| `--color-bg-base` | `#0F111A` | Page background |
| `--color-bg-card` | `#1A1D2E` | Card surfaces |
| `--color-bg-elevated` | `#242840` | Elevated panels, dropdowns |
| `--color-border` | `#2E3050` | Default borders |
| `--color-text-primary` | `#E8EBF4` | Headings, primary text |
| `--color-text-secondary` | `#8B90B0` | Labels, secondary info |
| `--color-text-muted` | `#4A5080` | Placeholders, disabled |
| `--color-success` | `#4CAF50` | Best run, improvement |
| `--color-error` | `#F44336` | Failed run, regression |

## 3. Typography Rules
```css
--font-sans: 'Source Sans Pro', 'Inter', -apple-system, sans-serif;
--font-mono: 'Source Code Pro', 'JetBrains Mono', monospace;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 13px;
--font-size-md: 15px;
--font-size-lg: 18px;
--font-size-xl: 24px;
--font-size-2xl: 32px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.2;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Dashboard Title | 24px | 700 | 1.2 |
| Section Header | 15px | 600 | 1.4 |
| Run Name | 13px | 600 | 1.4 |
| Body | 13px | 400 | 1.5 |
| Metric Label | 12px | 500 | 1.3 |
| Monospace/Code | 12px | 400 | 1.6 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #FFBE00;
  color: #0F111A;
  border: none;
  border-radius: 6px;
  padding: 8px 16px;
  font-size: 13px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.12s ease;
}
.button-primary:hover { background: #D9A000; }

/* Run Row */
.run-row {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 8px 12px;
  border-bottom: 1px solid #2E3050;
  cursor: pointer;
  transition: background 0.1s;
}
.run-row:hover { background: #1A1D2E; }
.run-color-dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  flex-shrink: 0;
}
.run-name {
  font-size: 13px;
  font-weight: 600;
  color: #E8EBF4;
  font-family: var(--font-mono);
}

/* Metric Card */
.metric-card {
  background: #1A1D2E;
  border: 1px solid #2E3050;
  border-radius: 8px;
  padding: 16px;
}
.metric-card__value {
  font-size: 28px;
  font-weight: 700;
  color: #FFBE00;
  font-family: var(--font-mono);
}
.metric-card__delta-up {
  font-size: 12px;
  color: #4CAF50;
  font-family: var(--font-mono);
}
.metric-card__delta-down {
  font-size: 12px;
  color: #F44336;
  font-family: var(--font-mono);
}

/* Tag Chip */
.tag-chip {
  display: inline-flex;
  align-items: center;
  padding: 2px 8px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
  font-family: var(--font-mono);
  background: rgba(255,190,0,0.12);
  color: #FFBE00;
  border: 1px solid rgba(255,190,0,0.25);
}

/* Input */
.input {
  background: #0F111A;
  border: 1px solid #2E3050;
  border-radius: 6px;
  padding: 8px 12px;
  font-size: 13px;
  color: #E8EBF4;
  transition: border-color 0.12s;
}
.input:focus {
  outline: none;
  border-color: #FFBE00;
  box-shadow: 0 0 0 2px rgba(255,190,0,0.15);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Color dot gaps |
| `--spacing-sm` | `8px` | Row vertical padding |
| `--spacing-md` | `12px` | Card inner padding |
| `--spacing-lg` | `16px` | Section gaps |
| `--spacing-xl` | `24px` | Panel gutter |
| `--sidebar-width` | `260px` | Run list sidebar |
| `--radius-sm` | `4px` | Badges |
| `--radius-md` | `6px` | Buttons, inputs |
| `--radius-lg` | `8px` | Cards, chart panels |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-chart { box-shadow: 0 4px 16px rgba(0,0,0,0.4); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.65); }
```

## 7. Do's and Don'ts
**Do:**
- Assign a distinct run color to each experiment run from the defined palette
- Show metric deltas with green/red monospace to indicate improvement/regression
- Use monospace for all run names, metric values, and hyperparameter values
- Display run comparisons in a scrollable side-by-side panel

**Don't:**
- Don't reuse run colors within the same comparison group
- Don't use the gold accent for anything other than the primary brand CTA and highlighted metrics
- Don't truncate run names — they're identifiers and must be scannable
- Don't use light mode for chart-heavy dashboards

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single metric view; run list collapses to dropdown |
| Tablet | 768px | Two-panel: run list + selected run metrics |
| Desktop | 1024px | Full layout: sidebar + chart grid + detail panel |
| Wide | 1440px | Expanded chart grid with more metrics per row |

## 9. Agent Prompt Guide
```
You are designing for Weights & Biases (W&B) — ML experiment tracking.
Use a deep navy background (#0F111A) with card surfaces at #1A1D2E.
Primary accent is gold (#FFBE00) — use for CTAs, key metric values, and golden run traces.
Each experiment run gets a distinct color from: coral, blue, green, purple, cyan.
Run names and metric values are always in monospace font.
Metric cards show large gold monospace numbers with small green/red delta indicators.
Tone is research-dense, comparison-focused, and ML-engineer-first.
```
