# Lattice Design System
> People management platform with a clean, professional aesthetic — white surfaces, teal-green brand, and performance-review-first UI.

---

## 1. Visual Theme & Atmosphere
Lattice is the operating system for people teams — it centralizes performance reviews, OKRs, employee engagement, and career development. The interface is clean and purposeful, balancing the depth of HR workflows with an approachable, modern aesthetic. A teal-green brand accent signals progress and growth, matching the platform's mission to help people and companies thrive. The UI is structured and data-rich but avoids the sterile feel of traditional enterprise HR software.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#00897B` | Brand teal, CTAs, active states |
| `--color-primary-dark` | `#00695C` | Hover/active |
| `--color-primary-light` | `#E0F2F1` | Teal tint backgrounds |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-surface` | `#F7F8FC` | Sidebar, panels, table rows |
| `--color-bg-card` | `#FFFFFF` | Card surfaces |
| `--color-border` | `#DDE3EE` | Default borders |
| `--color-border-strong` | `#C1CBD8` | Table headers, strong dividers |
| `--color-text-primary` | `#1A2332` | Headings, primary text |
| `--color-text-secondary` | `#667085` | Labels, meta |
| `--color-text-muted` | `#98A2B3` | Placeholders, disabled |
| `--color-success` | `#27AE60` | Complete, on track |
| `--color-error` | `#E53935` | At risk, overdue |
| `--color-warning` | `#F9A825` | Behind, needs attention |
| `--color-info` | `#1976D2` | Informational |
| `--color-okr-green` | `#27AE60` | On-track OKR |
| `--color-okr-yellow` | `#F9A825` | At-risk OKR |
| `--color-okr-red` | `#E53935` | Off-track OKR |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 18px;
--font-size-xl: 22px;
--font-size-2xl: 28px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.3;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 22px | 700 | 1.3 |
| Section Header | 16px | 600 | 1.4 |
| Card Title | 14px | 600 | 1.4 |
| Body / Labels | 14px | 400 | 1.5 |
| Table Text | 13px | 400 | 1.4 |
| Caption / Meta | 12px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #00897B;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 9px 20px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #00695C; }

/* OKR Progress Card */
.okr-card {
  background: #FFFFFF;
  border: 1px solid #DDE3EE;
  border-radius: 8px;
  padding: 20px;
}
.okr-card__title {
  font-size: 14px;
  font-weight: 600;
  color: #1A2332;
  margin-bottom: 6px;
}
.okr-card__owner { font-size: 12px; color: #667085; margin-bottom: 14px; }
.okr-progress {
  height: 8px;
  background: #DDE3EE;
  border-radius: 100px;
  overflow: hidden;
  margin-bottom: 6px;
}
.okr-progress__fill {
  height: 100%;
  border-radius: 100px;
  transition: width 0.3s ease;
}
.okr-progress__fill--green { background: #27AE60; }
.okr-progress__fill--yellow { background: #F9A825; }
.okr-progress__fill--red { background: #E53935; }
.okr-card__percentage {
  font-size: 12px;
  font-weight: 600;
  color: #1A2332;
}

/* Review Rating Scale */
.rating-scale {
  display: flex;
  gap: 8px;
  margin: 12px 0;
}
.rating-option {
  flex: 1;
  padding: 10px 6px;
  border: 2px solid #DDE3EE;
  border-radius: 8px;
  text-align: center;
  cursor: pointer;
  font-size: 12px;
  font-weight: 500;
  color: #667085;
  transition: border-color 0.12s, background 0.12s, color 0.12s;
}
.rating-option:hover { border-color: #00897B; color: #00897B; }
.rating-option--selected {
  border-color: #00897B;
  background: #E0F2F1;
  color: #00695C;
  font-weight: 600;
}

/* Employee Row */
.employee-row {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 12px 16px;
  border-bottom: 1px solid #DDE3EE;
  cursor: pointer;
  transition: background 0.08s;
}
.employee-row:hover { background: #F7F8FC; }
.employee-row__avatar {
  width: 36px;
  height: 36px;
  border-radius: 50%;
  background: #E0F2F1;
  color: #00897B;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 13px;
  font-weight: 600;
  flex-shrink: 0;
}
.employee-row__name { font-size: 14px; font-weight: 500; color: #1A2332; }
.employee-row__role { font-size: 12px; color: #667085; }

/* Status Chip */
.status-chip {
  display: inline-block;
  padding: 3px 10px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
}
.status-chip--complete { background: #ECFDF5; color: #065F46; }
.status-chip--in-progress { background: #EFF6FF; color: #1E40AF; }
.status-chip--not-started { background: #F3F4F6; color: #6B7280; }
.status-chip--overdue { background: #FEF2F2; color: #991B1B; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Tight element gaps |
| `--spacing-sm` | `8px` | Rating option gaps |
| `--spacing-md` | `16px` | Card inner spacing |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Page gutter |
| `--sidebar-width` | `240px` | Left navigation |
| `--radius-sm` | `4px` | Tags |
| `--radius-md` | `6px` | Buttons |
| `--radius-lg` | `8px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.06); }
.shadow-modal { box-shadow: 0 12px 40px rgba(0,0,0,0.12); }
.shadow-dropdown { box-shadow: 0 4px 16px rgba(0,0,0,0.08); }
```

## 7. Do's and Don'ts
**Do:**
- Use teal (#00897B) for all active states, progress fills (when on track), and CTAs
- OKR progress bars are color-coded: green (on track), yellow (at risk), red (off track)
- Performance rating options are full-width flex items with border selection
- Employee rows show circular avatar with initials

**Don't:**
- Don't use the teal for off-track or at-risk states — those have their own semantic colors
- Don't condense the rating scale — each option needs enough tap/click area
- Don't use dark backgrounds — Lattice is a bright, professional workspace

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single view; sidebar hidden |
| Tablet | 768px | Compact sidebar + main content |
| Desktop | 1024px | Sidebar + content + detail panel |
| Wide | 1440px | Dashboard with multi-column stats |

## 9. Agent Prompt Guide
```
You are designing for Lattice — people management and performance platform.
Use a white background (#FFFFFF) with light gray surfaces (#F7F8FC) for sidebars and panels.
Teal (#00897B) is the brand color — CTAs, active nav, focus rings, on-track OKR progress.
OKR cards show a title, owner, color-coded progress bar, and completion percentage.
Progress bars are color-coded: green (on track), amber (at risk), red (off track).
Performance review rating scales use full-width bordered options with teal selected state.
Tone is professional, people-focused, growth-oriented, and structured for HR teams.
```
