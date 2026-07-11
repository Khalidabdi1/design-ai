# Gusto Design System
> Payroll and HR platform with a warm, people-first aesthetic — coral-orange brand accents, generous whitespace, and human-centered data UI.

---

## 1. Visual Theme & Atmosphere
Gusto makes payroll feel human. The design rejects the cold blue grids of legacy HR software, instead embracing warmth: a coral-orange brand color, soft shadows, and a conversational, approachable tone. UI surfaces are clean white with subtle structure — nothing feels bureaucratic. Data is displayed with care, not density, ensuring non-technical employees feel as comfortable as payroll admins.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#F45D48` | Brand coral, CTAs, highlights |
| `--color-primary-dark` | `#D44030` | Hover/active primary |
| `--color-primary-light` | `#FEF0EE` | Soft backgrounds, highlights |
| `--color-secondary` | `#5B4FCF` | Accent purple, secondary actions |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F8F8F8` | Section backgrounds, table rows |
| `--color-bg-warm` | `#FFF8F7` | Warm tinted panels |
| `--color-text-primary` | `#1E1E2E` | Headings, primary text |
| `--color-text-secondary` | `#5C5C7A` | Body text, secondary |
| `--color-text-muted` | `#9E9EB8` | Labels, timestamps |
| `--color-border` | `#E2E2EF` | Default borders |
| `--color-border-subtle` | `#F0F0FA` | Dividers |
| `--color-success` | `#28A745` | Paid, approved |
| `--color-warning` | `#F5A623` | Pending, review needed |
| `--color-error` | `#DC3545` | Failed, rejected |

## 3. Typography Rules
```css
--font-sans: 'Tiempos Text', 'Georgia', serif;
--font-ui: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 12px;
--font-size-sm: 14px;
--font-size-base: 15px;
--font-size-md: 17px;
--font-size-lg: 22px;
--font-size-xl: 28px;
--font-size-2xl: 36px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.6;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 28px | 700 | 1.25 |
| Section Header | 22px | 600 | 1.3 |
| Card Title | 17px | 600 | 1.4 |
| Body | 15px | 400 | 1.6 |
| UI Label | 14px | 500 | 1.4 |
| Caption | 12px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #F45D48;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 11px 22px;
  font-size: 15px;
  font-weight: 600;
  font-family: var(--font-ui);
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #D44030; }

/* Employee Card */
.employee-card {
  background: #FFFFFF;
  border: 1px solid #E2E2EF;
  border-radius: 12px;
  padding: 20px;
  display: flex;
  align-items: center;
  gap: 16px;
  transition: box-shadow 0.15s;
}
.employee-card:hover { box-shadow: 0 4px 16px rgba(0,0,0,0.08); }
.employee-avatar {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  background: #FEF0EE;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 18px;
  font-weight: 700;
  color: #F45D48;
  flex-shrink: 0;
}

/* Payroll Summary Card */
.payroll-card {
  background: #FFFFFF;
  border: 1px solid #E2E2EF;
  border-radius: 12px;
  padding: 24px;
}
.payroll-card__amount {
  font-size: 36px;
  font-weight: 700;
  color: #1E1E2E;
  font-family: var(--font-ui);
}
.payroll-card__label {
  font-size: 14px;
  color: #9E9EB8;
  margin-top: 4px;
}
.payroll-card__status {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 10px;
  border-radius: 100px;
  font-size: 12px;
  font-weight: 600;
  font-family: var(--font-ui);
}
.payroll-card__status--paid {
  background: rgba(40,167,69,0.1);
  color: #28A745;
}

/* Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  padding: 3px 9px;
  border-radius: 100px;
  font-size: 12px;
  font-weight: 600;
  font-family: var(--font-ui);
}

/* Input */
.input {
  border: 1.5px solid #E2E2EF;
  border-radius: 8px;
  padding: 11px 14px;
  font-size: 15px;
  font-family: var(--font-ui);
  color: #1E1E2E;
  background: #FFFFFF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #F45D48;
  box-shadow: 0 0 0 3px rgba(244,93,72,0.12);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Tight inline gaps |
| `--spacing-sm` | `8px` | Badge padding |
| `--spacing-md` | `16px` | Card inner spacing |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Page-level padding |
| `--spacing-2xl` | `64px` | Section separators |
| `--max-content` | `960px` | Centered content max-width |
| `--radius-sm` | `6px` | Badges, chips |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `12px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.06); }
.shadow-hover { box-shadow: 0 4px 16px rgba(0,0,0,0.08); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.12); }
```

## 7. Do's and Don'ts
**Do:**
- Use coral orange for all primary CTAs and important highlights
- Keep the layout warm and spacious — HR software users are often non-technical
- Show employee avatars with initials in warm coral when no photo is available
- Use conversational confirmation messages after completing payroll actions

**Don't:**
- Don't use cold blue or gray-heavy palettes — it contradicts the brand warmth
- Don't display raw tax data without context labels or summaries
- Don't use more than 3 status states for any payroll item

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single-column: payroll summary + employee list |
| Tablet | 768px | Two-column layout, collapsible sidebar |
| Desktop | 1024px | Full sidebar + main content + detail panel |
| Wide | 1440px | Centered at 960px max with comfortable side margins |

## 9. Agent Prompt Guide
```
You are designing for Gusto — payroll and HR platform.
Use white backgrounds with coral-orange (#F45D48) as the primary CTA and accent color.
Employee avatars use initial letters on warm coral circular backgrounds.
Payroll cards display large bold dollar amounts with muted labels and pill status badges.
Inputs use coral focus rings; cards have subtle borders and a soft hover shadow.
Typography uses a serif (Tiempos Text) for display, Inter for UI labels.
Tone is warm, human, and reassuring — never cold or bureaucratic.
```
