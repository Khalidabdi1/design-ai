# Pipedrive Design System
> Sales-driven CRM with a pipeline-first visual language — bold greens, clean data tables, and action-oriented UI.

---

## 1. Visual Theme & Atmosphere
Pipedrive projects confidence and momentum. The interface is built around the sales pipeline metaphor: columns, cards, and clear progression. The aesthetic is professional yet approachable, using strong greens to convey growth and forward motion. UI density is moderate — enough data to act on, enough whitespace to breathe.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#25B85D` | Brand green, CTAs, active pipeline stages |
| `--color-primary-dark` | `#1D9148` | Hover states, pressed buttons |
| `--color-primary-light` | `#E6F9EE` | Backgrounds, highlights, badges |
| `--color-neutral-900` | `#1A1A1A` | Headings, primary text |
| `--color-neutral-700` | `#4A4A4A` | Body text, secondary labels |
| `--color-neutral-400` | `#9E9E9E` | Placeholders, disabled states |
| `--color-neutral-100` | `#F5F5F5` | Surface backgrounds |
| `--color-white` | `#FFFFFF` | Cards, panels |
| `--color-danger` | `#E74C3C` | Errors, lost deals |
| `--color-warning` | `#F39C12` | Overdue, attention states |
| `--color-info` | `#2980B9` | Informational badges |

## 3. Typography Rules
```css
--font-sans: 'Inter', 'Helvetica Neue', Arial, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 24px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 24px | 700 | 1.25 |
| Section Header | 20px | 600 | 1.3 |
| Card Title | 16px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label/Meta | 13px | 500 | 1.4 |
| Caption | 11px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary CTA Button */
.button-primary {
  background: #25B85D;
  color: #FFFFFF;
  border: none;
  border-radius: 4px;
  padding: 8px 16px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s ease;
}
.button-primary:hover { background: #1D9148; }

/* Pipeline Stage Card */
.deal-card {
  background: #FFFFFF;
  border: 1px solid #E8E8E8;
  border-radius: 6px;
  padding: 12px;
  margin-bottom: 8px;
  cursor: pointer;
  transition: box-shadow 0.15s ease;
}
.deal-card:hover { box-shadow: 0 2px 8px rgba(0,0,0,0.12); }

/* Stage Column Header */
.pipeline-column-header {
  background: #F5F5F5;
  border-radius: 4px 4px 0 0;
  padding: 10px 12px;
  font-size: 13px;
  font-weight: 600;
  color: #4A4A4A;
  border-bottom: 2px solid #25B85D;
}

/* Badge / Tag */
.badge {
  display: inline-flex;
  align-items: center;
  padding: 2px 8px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
  background: #E6F9EE;
  color: #1D9148;
}

/* Input */
.input {
  border: 1px solid #D0D0D0;
  border-radius: 4px;
  padding: 8px 12px;
  font-size: 14px;
  color: #1A1A1A;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #25B85D;
  box-shadow: 0 0 0 3px rgba(37,184,93,0.15);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Icon padding, tight gaps |
| `--spacing-sm` | `8px` | Card internal spacing |
| `--spacing-md` | `12px` | Component gaps |
| `--spacing-lg` | `16px` | Section padding |
| `--spacing-xl` | `24px` | Page-level gutter |
| `--spacing-2xl` | `32px` | Section separation |
| `--radius-sm` | `4px` | Buttons, inputs |
| `--radius-md` | `6px` | Cards |
| `--radius-lg` | `8px` | Modals, panels |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 1px 3px rgba(0,0,0,0.08); }
.shadow-dropdown { box-shadow: 0 4px 12px rgba(0,0,0,0.12); }
.shadow-modal { box-shadow: 0 8px 32px rgba(0,0,0,0.16); }
```

## 7. Do's and Don'ts
**Do:**
- Use green only for positive pipeline actions and CTAs
- Keep the pipeline view as the primary navigation metaphor
- Show deal value prominently on cards
- Use stage counts and conversion rates in column headers

**Don't:**
- Don't clutter cards with more than 3–4 data points
- Don't use red for anything other than lost/danger states
- Don't break the left-to-right pipeline flow for anything

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single-column list view replaces pipeline board |
| Tablet | 768px | Condensed pipeline, 2–3 columns visible |
| Desktop | 1024px | Full pipeline board with horizontal scroll |
| Wide | 1440px | Full board + sidebar details panel |

## 9. Agent Prompt Guide
```
You are designing for Pipedrive — a CRM built around the sales pipeline.
Use bold green (#25B85D) for all primary CTAs and active states.
Keep the pipeline board metaphor central: columns represent stages, cards represent deals.
Typography is Inter at 14px base, 600 weight for headers.
Cards are white with subtle borders; hover reveals a soft shadow.
Inputs use green focus rings. Badges are pill-shaped with light green fill.
The tone is confident, data-rich, and action-forward.
```
