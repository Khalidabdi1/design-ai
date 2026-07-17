# BambooHR Design System
> HR software platform with a warm, people-first aesthetic — clean white surfaces, sage green brand, and employee-centered UI.

---

## 1. Visual Theme & Atmosphere
BambooHR is the friendly face of HR software. Where most enterprise tools feel corporate and cold, BambooHR leans into warmth — bright whites, a calm sage-green brand, and illustrations of real people. The interface centers on employee records, org charts, and time-off requests, all wrapped in a professional but approachable aesthetic. It feels like a well-designed HR office: organized, welcoming, and human.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#73AC39` | Brand sage green, CTAs, active nav |
| `--color-primary-dark` | `#5A8F28` | Hover/active |
| `--color-primary-light` | `#EFF6E6` | Green tint backgrounds |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-surface` | `#F7F8FA` | Table rows, panel backgrounds |
| `--color-bg-card` | `#FFFFFF` | Cards, modals |
| `--color-border` | `#E0E4EA` | Default borders |
| `--color-border-strong` | `#C5CDD9` | Table headers, dividers |
| `--color-text-primary` | `#1F2D3D` | Headings, primary text |
| `--color-text-secondary` | `#6B7A8D` | Labels, meta text |
| `--color-text-muted` | `#A0AABB` | Placeholders, disabled |
| `--color-success` | `#73AC39` | Active employees, approved |
| `--color-error` | `#E53E3E` | Errors, terminated |
| `--color-warning` | `#F6AD55` | Pending, review needed |
| `--color-info` | `#4299E1` | Info banners |

## 3. Typography Rules
```css
--font-sans: 'Proxima Nova', 'Inter', -apple-system, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 18px;
--font-size-xl: 24px;
--font-size-2xl: 30px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.3;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 24px | 700 | 1.3 |
| Section Header | 16px | 600 | 1.4 |
| Card Title | 14px | 600 | 1.4 |
| Body / Labels | 14px | 400 | 1.5 |
| Table Text | 13px | 400 | 1.4 |
| Caption / Meta | 12px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #73AC39;
  color: #FFFFFF;
  border: none;
  border-radius: 4px;
  padding: 9px 20px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #5A8F28; }

/* Secondary Button */
.button-secondary {
  background: #FFFFFF;
  color: #1F2D3D;
  border: 1px solid #C5CDD9;
  border-radius: 4px;
  padding: 8px 20px;
  font-size: 14px;
  font-weight: 500;
  cursor: pointer;
  transition: background 0.15s, border-color 0.15s;
}
.button-secondary:hover { background: #F7F8FA; border-color: #A0AABB; }

/* Employee Card */
.employee-card {
  background: #FFFFFF;
  border: 1px solid #E0E4EA;
  border-radius: 8px;
  padding: 20px;
  display: flex;
  align-items: center;
  gap: 16px;
  transition: box-shadow 0.15s;
}
.employee-card:hover { box-shadow: 0 4px 12px rgba(0,0,0,0.08); }
.employee-card__avatar {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  background: #EFF6E6;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 18px;
  font-weight: 600;
  color: #73AC39;
  flex-shrink: 0;
}
.employee-card__name {
  font-size: 15px;
  font-weight: 600;
  color: #1F2D3D;
}
.employee-card__role {
  font-size: 12px;
  color: #6B7A8D;
  margin-top: 2px;
}

/* Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  padding: 3px 8px;
  border-radius: 12px;
  font-size: 11px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.04em;
}
.status-badge--active { background: #EFF6E6; color: #5A8F28; }
.status-badge--pending { background: #FFFBEB; color: #B7791F; }
.status-badge--inactive { background: #FEF2F2; color: #C53030; }

/* Data Table */
.data-table { width: 100%; border-collapse: collapse; }
.data-table th {
  background: #F7F8FA;
  border-bottom: 2px solid #C5CDD9;
  padding: 10px 16px;
  font-size: 12px;
  font-weight: 600;
  color: #6B7A8D;
  text-align: left;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
.data-table td {
  padding: 12px 16px;
  font-size: 14px;
  color: #1F2D3D;
  border-bottom: 1px solid #E0E4EA;
}
.data-table tr:hover td { background: #F7F8FA; }

/* Input */
.input {
  background: #FFFFFF;
  border: 1px solid #C5CDD9;
  border-radius: 4px;
  padding: 9px 12px;
  font-size: 14px;
  color: #1F2D3D;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #73AC39;
  box-shadow: 0 0 0 3px rgba(115,172,57,0.12);
}
.input::placeholder { color: #A0AABB; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Badge gaps, tight pairs |
| `--spacing-sm` | `8px` | Card inner spacing |
| `--spacing-md` | `16px` | Section padding |
| `--spacing-lg` | `24px` | Card padding |
| `--spacing-xl` | `40px` | Page gutter |
| `--sidebar-width` | `220px` | Left navigation |
| `--radius-sm` | `4px` | Buttons, inputs |
| `--radius-md` | `8px` | Cards |
| `--radius-pill` | `12px` | Status badges |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 6px rgba(0,0,0,0.06); }
.shadow-hover { box-shadow: 0 4px 12px rgba(0,0,0,0.10); }
.shadow-modal { box-shadow: 0 12px 40px rgba(0,0,0,0.15); }
.shadow-dropdown { box-shadow: 0 4px 16px rgba(0,0,0,0.10); }
```

## 7. Do's and Don'ts
**Do:**
- Use sage green (#73AC39) as the primary action color — buttons, active nav, focus rings
- Show employee avatars with initials and green background as fallback
- Use status badges (active/pending/inactive) with color-coded pill styles
- Keep tables clean with alternating hover states, not row striping

**Don't:**
- Don't use dark backgrounds — BambooHR is a light, open UI
- Don't omit the employee avatar in employee records
- Don't use red for anything other than errors or terminated status

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single column; sidebar hidden |
| Tablet | 768px | Collapsible sidebar + content |
| Desktop | 1024px | Full sidebar + main content |
| Wide | 1440px | Sidebar + content + detail panel |

## 9. Agent Prompt Guide
```
You are designing for BambooHR — HR software platform.
Use a clean white background (#FFFFFF) with light gray surfaces (#F7F8FA) for tables and panels.
Sage green (#73AC39) is the primary brand color — CTAs, active states, focus rings, and status badges.
Employee cards show circular avatar with initials, name, and role label.
Status badges are pill-shaped: green for active, amber for pending, red for inactive.
Data tables have a gray header row with uppercase labels and clean row hover states.
Tone is warm, professional, people-first, and approachable for HR teams.
```
