# Productboard Design System
> Product management and roadmap platform with a clean, structured aesthetic — white surfaces, violet-purple brand accents, and insight-driven UI patterns.

---

## 1. Visual Theme & Atmosphere
Productboard is where product teams synthesize customer insights into prioritized roadmaps. The design is clean and structured, reflecting the systematic nature of product management. White surfaces with a violet-purple accent create a calm, focused environment. The UI is data-rich but organized — insights, features, and roadmap items each have their own visual vocabulary while staying within a coherent system.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#6B4FBB` | Brand violet, CTAs |
| `--color-primary-dark` | `#5540A0` | Hover/active primary |
| `--color-primary-light` | `#F0ECFB` | Light backgrounds |
| `--color-insight` | `#2D9CDB` | Customer insight highlights |
| `--color-feature` | `#27AE60` | Feature/story status |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F7F8FC` | Section backgrounds |
| `--color-text-primary` | `#1A1A2E` | Headings, primary |
| `--color-text-secondary` | `#52546A` | Body text, labels |
| `--color-text-muted` | `#9B9DB8` | Timestamps, meta |
| `--color-border` | `#E2E4F0` | Default borders |
| `--color-border-subtle` | `#EEF0FA` | Dividers |
| `--color-score-high` | `#27AE60` | High priority score |
| `--color-score-mid` | `#F2994A` | Medium priority |
| `--color-score-low` | `#EB5757` | Low score |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 26px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 26px | 700 | 1.25 |
| Section Header | 16px | 600 | 1.4 |
| Feature Name | 14px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label | 12px | 500 | 1.4 |
| Score | 14px | 700 | 1.2 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #6B4FBB;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 9px 18px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #5540A0; }

/* Feature Card */
.feature-card {
  background: #FFFFFF;
  border: 1px solid #E2E4F0;
  border-radius: 8px;
  padding: 16px;
  cursor: pointer;
  transition: box-shadow 0.15s;
}
.feature-card:hover { box-shadow: 0 2px 12px rgba(0,0,0,0.07); }
.feature-card__name {
  font-size: 14px;
  font-weight: 600;
  color: #1A1A2E;
  margin-bottom: 4px;
}
.feature-card__description {
  font-size: 13px;
  color: #52546A;
  line-height: 1.5;
}

/* Priority Score */
.priority-score {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 36px;
  height: 36px;
  border-radius: 6px;
  font-size: 14px;
  font-weight: 700;
}
.priority-score--high { background: rgba(39,174,96,0.1); color: #27AE60; }
.priority-score--mid { background: rgba(242,153,74,0.1); color: #F2994A; }
.priority-score--low { background: rgba(235,87,87,0.1); color: #EB5757; }

/* Insight Card */
.insight-card {
  background: #F0F8FF;
  border-left: 3px solid #2D9CDB;
  border-radius: 0 6px 6px 0;
  padding: 12px 16px;
  font-size: 13px;
  color: #1A1A2E;
  line-height: 1.5;
}
.insight-card__source {
  font-size: 11px;
  color: #9B9DB8;
  margin-top: 6px;
}

/* Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  padding: 2px 8px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
.status-badge--candidate { background: #F0ECFB; color: #6B4FBB; }
.status-badge--planned { background: #E8F5EE; color: #27AE60; }
.status-badge--in-progress { background: #E8F4FF; color: #2D9CDB; }
.status-badge--shipped { background: #E8F5EE; color: #16A34A; }

/* Input */
.input {
  border: 1.5px solid #E2E4F0;
  border-radius: 6px;
  padding: 9px 12px;
  font-size: 14px;
  color: #1A1A2E;
  background: #FFFFFF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #6B4FBB;
  box-shadow: 0 0 0 3px rgba(107,79,187,0.12);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Tight inline gaps |
| `--spacing-sm` | `8px` | Badge/chip gaps |
| `--spacing-md` | `16px` | Card inner padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `32px` | Page gutter |
| `--sidebar-width` | `240px` | Left navigation |
| `--radius-sm` | `4px` | Status badges |
| `--radius-md` | `6px` | Buttons, inputs |
| `--radius-lg` | `8px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 1px 4px rgba(0,0,0,0.05); }
.shadow-hover { box-shadow: 0 2px 12px rgba(0,0,0,0.07); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.12); }
```

## 7. Do's and Don'ts
**Do:**
- Use priority scores as colored number badges (not just labels)
- Insight cards have a blue left border to distinguish them from feature cards
- Status badges are uppercase pill labels with semantic colors
- Link insights to features visually — a connector or badge count

**Don't:**
- Don't use heavy kanban boards as the primary view — list and grid are both needed
- Don't use more than 4 distinct feature status states
- Don't mix the brand purple with insight blue in close visual proximity

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single column list; no roadmap view |
| Tablet | 768px | Two panels: sidebar + feature list |
| Desktop | 1024px | Full: sidebar + list/board + detail pane |
| Wide | 1440px | Roadmap timeline with expanded swimlanes |

## 9. Agent Prompt Guide
```
You are designing for Productboard — product management and roadmapping.
Use white backgrounds with violet (#6B4FBB) for CTAs and focus rings.
Priority scores are colored square badges: green=high, orange=mid, red=low.
Customer insight cards have a blue (#2D9CDB) left border and light blue background.
Feature status badges are uppercase pills: violet=candidate, green=planned, blue=in-progress.
Inputs and cards use 6–8px radius with a clean 1–1.5px border.
Tone is structured, insight-driven, and product-team-focused.
```
