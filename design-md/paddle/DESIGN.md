# Paddle Design System
> SaaS payment infrastructure with a clean, merchant-confident aesthetic — deep blue brand, green revenue accents, and billing-dashboard-first UI.

---

## 1. Visual Theme & Atmosphere
Paddle handles the entire payment stack for software companies, and its design reflects that responsibility. The UI is clean, trustworthy, and data-oriented — a deep blue brand that communicates financial reliability, paired with green revenue indicators that celebrate growth. Dashboard views surface billing metrics, subscription health, and churn data with clarity. The aesthetic is polished enterprise without being cold.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#0B4FFF` | Brand blue, CTAs |
| `--color-primary-dark` | `#0038CC` | Hover/active primary |
| `--color-primary-light` | `#E8EFFE` | Light highlights |
| `--color-revenue` | `#00B87A` | MRR, revenue, growth |
| `--color-revenue-light` | `#E0F7EF` | Revenue badge backgrounds |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F8FAFF` | Section backgrounds |
| `--color-bg-dark` | `#04133D` | Dark hero, top bar |
| `--color-text-primary` | `#0A0F2C` | Headings, primary text |
| `--color-text-secondary` | `#4C5680` | Body, labels |
| `--color-text-muted` | `#9CA3C5` | Timestamps, meta |
| `--color-border` | `#DEE3F4` | Default borders |
| `--color-border-subtle` | `#EEF1FA` | Dividers |
| `--color-success` | `#00B87A` | Paid, active subscription |
| `--color-warning` | `#F59E0B` | Dunning, past due |
| `--color-error` | `#EF4444` | Failed charge, churned |

## 3. Typography Rules
```css
--font-sans: 'Inter', 'Helvetica Neue', Arial, sans-serif;
--font-mono: 'JetBrains Mono', 'IBM Plex Mono', monospace;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 28px;
--font-size-2xl: 36px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Dashboard Title | 28px | 700 | 1.25 |
| Section Header | 20px | 600 | 1.3 |
| Card Title | 16px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label | 13px | 500 | 1.4 |
| Revenue Value | 36px | 700 | 1.2 |
| Mono / Code | 13px | 400 | 1.5 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #0B4FFF;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 10px 20px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #0038CC; }

/* Revenue Metric Card */
.revenue-card {
  background: #FFFFFF;
  border: 1px solid #DEE3F4;
  border-radius: 10px;
  padding: 24px;
}
.revenue-card__value {
  font-size: 36px;
  font-weight: 700;
  color: #0A0F2C;
}
.revenue-card__delta {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  font-size: 13px;
  font-weight: 600;
  margin-top: 4px;
}
.revenue-card__delta--up { color: #00B87A; }
.revenue-card__delta--down { color: #EF4444; }
.revenue-card__label {
  font-size: 13px;
  color: #9CA3C5;
  margin-top: 4px;
}

/* Subscription Row */
.sub-row {
  display: grid;
  padding: 12px 16px;
  align-items: center;
  border-bottom: 1px solid #EEF1FA;
  font-size: 13px;
  cursor: pointer;
  transition: background 0.08s;
}
.sub-row:hover { background: #F8FAFF; }
.sub-row__id {
  font-family: var(--font-mono);
  font-size: 12px;
  color: #9CA3C5;
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
.status-badge--active { background: #E0F7EF; color: #00915F; }
.status-badge--past-due { background: #FEF3C7; color: #B45309; }
.status-badge--canceled { background: #FEE2E2; color: #B91C1C; }
.status-badge--trialing { background: #E8EFFE; color: #0B4FFF; }

/* Input */
.input {
  border: 1.5px solid #DEE3F4;
  border-radius: 8px;
  padding: 10px 14px;
  font-size: 14px;
  color: #0A0F2C;
  background: #FFFFFF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #0B4FFF;
  box-shadow: 0 0 0 3px rgba(11,79,255,0.12);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Delta indicator gaps |
| `--spacing-sm` | `8px` | Card inner compact |
| `--spacing-md` | `16px` | Section padding |
| `--spacing-lg` | `24px` | Card padding |
| `--spacing-xl` | `32px` | Page gutter |
| `--sidebar-width` | `240px` | Navigation sidebar |
| `--radius-sm` | `6px` | Status badges |
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
- Display MRR/ARR in large bold numbers — revenue is the hero metric
- Show subscription status badges with consistent semantic colors
- Use green delta indicators for positive revenue changes
- Display subscription IDs in monospace

**Don't:**
- Don't mix the blue brand with green revenue accents in the same headline
- Don't use red for anything other than cancellations and failed charges
- Don't paginate subscription tables by default — show enough rows to scan

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Metric cards single-column; table collapses to list |
| Tablet | 768px | Two-column metric grid |
| Desktop | 1024px | Sidebar + four-column metric grid |
| Wide | 1440px | Expanded table with more subscription columns |

## 9. Agent Prompt Guide
```
You are designing for Paddle — SaaS payment infrastructure.
Use a white background with deep blue (#0B4FFF) for CTAs and inputs.
Revenue metrics are the visual hero: large bold numbers with green (+) or red (-) delta indicators.
Subscription tables show ID (monospace), plan, status badge, amount, and date.
Status badges are pill-shaped: green=active, yellow=past-due, red=canceled, blue=trialing.
Dark navy (#04133D) for top navigation and hero sections.
Tone is financially trustworthy, data-driven, and merchant-confident.
```
