# Beehiiv Design System
> Newsletter publishing platform with a creator-first aesthetic — warm neutrals, editorial typography, and growth-focused metrics UI.

---

## 1. Visual Theme & Atmosphere
Beehiiv feels like a premium editorial tool that grew up on the internet. The aesthetic combines the warmth of print publishing with the precision of modern SaaS. Muted honey-gold accents punctuate a clean neutral palette. The interface celebrates writing: typography is expressive, whitespace is generous, and data surfaces support creators without overwhelming them.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#F5A623` | Brand gold, CTAs, highlights |
| `--color-primary-dark` | `#D4881A` | Hover/active primary states |
| `--color-primary-light` | `#FEF3DC` | Subtle backgrounds, callouts |
| `--color-neutral-950` | `#0D0D0D` | Headings, primary text |
| `--color-neutral-700` | `#3D3D3D` | Body text |
| `--color-neutral-500` | `#737373` | Secondary labels, metadata |
| `--color-neutral-200` | `#E8E8E8` | Borders, dividers |
| `--color-neutral-50` | `#FAFAFA` | Page background |
| `--color-white` | `#FFFFFF` | Card surfaces |
| `--color-success` | `#22C55E` | Growth indicators, subscriber milestones |
| `--color-error` | `#EF4444` | Errors, churn alerts |

## 3. Typography Rules
```css
--font-display: 'Cal Sans', 'DM Sans', sans-serif;
--font-body: 'Inter', 'DM Sans', sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 12px;
--font-size-sm: 13px;
--font-size-base: 15px;
--font-size-md: 17px;
--font-size-lg: 22px;
--font-size-xl: 28px;
--font-size-2xl: 36px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.2;
--line-height-base: 1.6;
--line-height-loose: 1.8;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Display Heading | 36px | 700 | 1.2 |
| Page Title | 28px | 700 | 1.25 |
| Section Header | 22px | 600 | 1.3 |
| Card Title | 17px | 600 | 1.4 |
| Body | 15px | 400 | 1.6 |
| Meta / Label | 13px | 500 | 1.4 |
| Caption | 12px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #F5A623;
  color: #0D0D0D;
  border: none;
  border-radius: 8px;
  padding: 10px 20px;
  font-size: 15px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s ease;
}
.button-primary:hover { background: #D4881A; }

/* Secondary Button */
.button-secondary {
  background: transparent;
  color: #0D0D0D;
  border: 1.5px solid #E8E8E8;
  border-radius: 8px;
  padding: 10px 20px;
  font-size: 15px;
  font-weight: 500;
}
.button-secondary:hover { border-color: #0D0D0D; }

/* Metric Card */
.metric-card {
  background: #FFFFFF;
  border: 1px solid #E8E8E8;
  border-radius: 12px;
  padding: 20px 24px;
}
.metric-card__value {
  font-size: 32px;
  font-weight: 700;
  color: #0D0D0D;
}
.metric-card__label {
  font-size: 13px;
  font-weight: 500;
  color: #737373;
  margin-top: 4px;
}

/* Post Preview Card */
.post-card {
  background: #FFFFFF;
  border: 1px solid #E8E8E8;
  border-radius: 12px;
  padding: 20px;
  transition: box-shadow 0.15s ease;
  cursor: pointer;
}
.post-card:hover { box-shadow: 0 4px 16px rgba(0,0,0,0.08); }

/* Input */
.input {
  border: 1.5px solid #E8E8E8;
  border-radius: 8px;
  padding: 10px 14px;
  font-size: 15px;
  font-family: var(--font-body);
  color: #0D0D0D;
  background: #FFFFFF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #F5A623;
  box-shadow: 0 0 0 3px rgba(245,166,35,0.15);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Inline gaps |
| `--spacing-sm` | `8px` | Compact padding |
| `--spacing-md` | `16px` | Card inner spacing |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Page gutter |
| `--spacing-2xl` | `64px` | Section separators |
| `--max-content` | `720px` | Editor/reading column width |
| `--radius-sm` | `6px` | Badges, chips |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `12px` | Cards, modals |

## 6. Depth & Elevation
```css
.shadow-sm { box-shadow: 0 1px 3px rgba(0,0,0,0.06); }
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.08); }
.shadow-hover { box-shadow: 0 4px 16px rgba(0,0,0,0.10); }
.shadow-modal { box-shadow: 0 12px 40px rgba(0,0,0,0.14); }
```

## 7. Do's and Don'ts
**Do:**
- Use generous line heights for editorial content (1.6–1.8)
- Surface subscriber growth metrics prominently with large number displays
- Keep the writing editor clean and distraction-free
- Use warm gold as an accent, not a dominant color

**Don't:**
- Don't use gold for error or warning states — reserve it for positive/primary actions
- Don't crowd the editor area with controls or sidebars
- Don't use more than 2 typefaces in a single context

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single column, bottom navigation, metric cards stack |
| Tablet | 768px | Sidebar collapses to icon rail, two-column cards |
| Desktop | 1024px | Full sidebar, analytics dashboard, inline previews |
| Wide | 1440px | Centered layout with wider content columns |

## 9. Agent Prompt Guide
```
You are designing for Beehiiv — a creator-first newsletter platform.
Primary accent is warm gold (#F5A623) on white or near-white backgrounds.
Typography uses Cal Sans or DM Sans for headings, Inter for body, with generous line heights.
Cards are white with 1px borders and 12px radius; hover adds a subtle shadow.
Metric displays use large bold numbers with small muted labels beneath.
The editor is wide, clean, and distraction-free — always centered at max ~720px.
Tone is editorial, warm, and growth-oriented.
```
