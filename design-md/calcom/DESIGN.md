# Cal.com Design System
> Open-source scheduling infrastructure with a developer-friendly, minimal aesthetic — dark surfaces, crisp whites, and calendar-driven UI patterns.

---

## 1. Visual Theme & Atmosphere
Cal.com combines the precision of a developer tool with the approachability of a consumer scheduling product. The design leans into dark-mode-first thinking with a near-black surface palette, crisp whites for contrast, and a subtle green accent that signals availability and confirmation. The UI is clean and purposeful — every element serves the scheduling flow.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-brand` | `#6366F1` | Primary brand indigo |
| `--color-brand-dark` | `#4F46E5` | Hover/active brand states |
| `--color-brand-light` | `#EEF2FF` | Light brand backgrounds |
| `--color-success` | `#10B981` | Availability, confirmed bookings |
| `--color-neutral-950` | `#09090B` | Darkest surface (dark mode bg) |
| `--color-neutral-900` | `#18181B` | Dark cards, sidebars |
| `--color-neutral-800` | `#27272A` | Elevated dark elements |
| `--color-neutral-600` | `#52525B` | Dark-mode muted text |
| `--color-neutral-400` | `#A1A1AA` | Secondary labels |
| `--color-neutral-200` | `#E4E4E7` | Light borders |
| `--color-neutral-50` | `#FAFAFA` | Light mode backgrounds |
| `--color-white` | `#FFFFFF` | Light mode cards, text on dark |
| `--color-error` | `#EF4444` | Errors, conflicts |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 12px;
--font-size-sm: 14px;
--font-size-base: 15px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 24px;
--font-size-2xl: 30px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 30px | 700 | 1.2 |
| Section Header | 20px | 600 | 1.3 |
| Card Title | 16px | 600 | 1.4 |
| Body | 15px | 400 | 1.5 |
| Label | 14px | 500 | 1.4 |
| Caption / Code | 12px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #6366F1;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 9px 18px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s ease;
}
.button-primary:hover { background: #4F46E5; }

/* Calendar Day Cell */
.calendar-day {
  width: 40px;
  height: 40px;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 14px;
  font-weight: 500;
  cursor: pointer;
  transition: background 0.1s ease;
  color: #FFFFFF;
}
.calendar-day--available:hover { background: rgba(99,102,241,0.2); }
.calendar-day--selected {
  background: #6366F1;
  color: #FFFFFF;
}
.calendar-day--disabled {
  color: #52525B;
  cursor: not-allowed;
}

/* Time Slot */
.time-slot {
  border: 1.5px solid #27272A;
  border-radius: 8px;
  padding: 10px 16px;
  font-size: 14px;
  font-weight: 500;
  color: #FFFFFF;
  cursor: pointer;
  transition: border-color 0.15s, background 0.15s;
}
.time-slot:hover {
  border-color: #6366F1;
  background: rgba(99,102,241,0.1);
}
.time-slot--selected {
  border-color: #6366F1;
  background: #6366F1;
}

/* Booking Confirmation Card */
.booking-card {
  background: #18181B;
  border: 1px solid #27272A;
  border-radius: 12px;
  padding: 24px;
}

/* Input */
.input {
  background: #18181B;
  border: 1.5px solid #27272A;
  border-radius: 8px;
  padding: 10px 14px;
  font-size: 14px;
  color: #FFFFFF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #6366F1;
  box-shadow: 0 0 0 3px rgba(99,102,241,0.2);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Icon gaps |
| `--spacing-sm` | `8px` | Calendar cell gaps |
| `--spacing-md` | `16px` | Card padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Page-level padding |
| `--radius-sm` | `6px` | Chips, badges |
| `--radius-md` | `8px` | Buttons, inputs, day cells |
| `--radius-lg` | `12px` | Cards, panels |
| `--calendar-cell` | `40px` | Fixed day cell size |

## 6. Depth & Elevation
```css
/* Dark mode defaults */
.shadow-sm { box-shadow: 0 1px 3px rgba(0,0,0,0.4); }
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Default to dark surfaces; offer a light-mode toggle
- Use indigo (#6366F1) consistently for selected states, CTAs, and interactive highlights
- Show availability status with green (#10B981) — never with the brand color
- Keep the calendar grid pixel-perfect: equal cell sizes, consistent spacing

**Don't:**
- Don't put more than 2 CTAs on the booking page — one primary, one secondary
- Don't use brand indigo for error states — use red (#EF4444)
- Don't animate calendar transitions excessively

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single column: calendar → time slots → form stacked vertically |
| Tablet | 768px | Calendar and time slots side by side, form below |
| Desktop | 1024px | Three-panel layout: details + calendar + time/form |
| Wide | 1440px | Centered container at 1200px max-width |

## 9. Agent Prompt Guide
```
You are designing for Cal.com — open-source scheduling infrastructure.
Primary brand color is indigo (#6366F1); availability indicators use green (#10B981).
Default to dark surfaces (#18181B cards, #09090B background) with white text.
The calendar grid is the centerpiece: 40px day cells, 8px radius, precise spacing.
Time slots use bordered cards that shift to indigo fill when selected.
Typography is Inter at 15px, 600 weight for interactive labels.
Tone is clean, developer-friendly, and precision-focused.
```
