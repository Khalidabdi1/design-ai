# Canny Design System
> Customer feedback management platform with a clean, upvote-centric aesthetic — white surfaces, blue brand accents, and feedback-board-first UI patterns.

---

## 1. Visual Theme & Atmosphere
Canny is where companies collect, organize, and respond to customer feedback. The design borrows the familiar vocabulary of voting platforms — upvote buttons, status badges, and comment threads — wrapped in a clean, trustworthy interface. Blue accents signal interactivity and the democratic nature of voting. The UI is deliberately simple: a feedback post, a vote count, and a status badge are the three building blocks of everything.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#2D7FF9` | Brand blue, CTAs, vote buttons |
| `--color-primary-dark` | `#1A6AE0` | Hover/active primary |
| `--color-primary-light` | `#EBF3FF` | Voted state, highlights |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F8F9FB` | Board sidebar, row alternates |
| `--color-text-primary` | `#1A1E2E` | Headings, post titles |
| `--color-text-secondary` | `#52566E` | Body, labels |
| `--color-text-muted` | `#9DA3BE` | Timestamps, vote counts |
| `--color-text-link` | `#2D7FF9` | Links |
| `--color-border` | `#E3E6F0` | Default borders |
| `--color-border-subtle` | `#EEF0FA` | Dividers |
| `--color-vote-active` | `#2D7FF9` | Voted upvote button |
| `--color-status-open` | `#2D7FF9` | Open status |
| `--color-status-planned` | `#F5A623` | Planned status |
| `--color-status-progress` | `#8E44AD` | In progress |
| `--color-status-complete` | `#27AE60` | Complete status |
| `--color-status-closed` | `#95A5A6` | Closed/won't do |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 13px;
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
--line-height-body: 1.6;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Post Title | 16px | 600 | 1.4 |
| Post Body | 14px | 400 | 1.6 |
| Vote Count | 14px | 700 | 1.2 |
| Board Name | 14px | 600 | 1.4 |
| Timestamp | 12px | 400 | 1.3 |
| Status Label | 12px | 600 | 1.3 |

## 4. Component Stylings
```css
/* Vote Button */
.vote-button {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2px;
  padding: 8px 12px;
  border-radius: 8px;
  border: 1.5px solid #E3E6F0;
  cursor: pointer;
  min-width: 52px;
  transition: border-color 0.12s, background 0.12s;
  background: #FFFFFF;
}
.vote-button:hover {
  border-color: #2D7FF9;
  background: #EBF3FF;
}
.vote-button--voted {
  border-color: #2D7FF9;
  background: #EBF3FF;
  color: #2D7FF9;
}
.vote-button__arrow {
  font-size: 12px;
  color: inherit;
}
.vote-button__count {
  font-size: 14px;
  font-weight: 700;
  color: inherit;
}

/* Feedback Post Row */
.post-row {
  display: flex;
  gap: 16px;
  padding: 16px;
  border-bottom: 1px solid #EEF0FA;
  cursor: pointer;
  transition: background 0.08s;
}
.post-row:hover { background: #F8F9FB; }
.post-row__content { flex: 1; }
.post-row__title {
  font-size: 15px;
  font-weight: 600;
  color: #1A1E2E;
  margin-bottom: 4px;
}
.post-row__meta {
  font-size: 12px;
  color: #9DA3BE;
  display: flex;
  align-items: center;
  gap: 8px;
}
.post-row__comments {
  font-size: 12px;
  color: #9DA3BE;
  display: flex;
  align-items: center;
  gap: 4px;
}

/* Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  padding: 2px 8px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
}
.status-badge--open { background: #EBF3FF; color: #1A6AE0; }
.status-badge--planned { background: #FEF3DC; color: #B8760A; }
.status-badge--in-progress { background: #F3EEFF; color: #6C3483; }
.status-badge--complete { background: #E8F5EE; color: #1A7F37; }
.status-badge--closed { background: #F0F2F5; color: #6B7280; }

/* Primary Button */
.button-primary {
  background: #2D7FF9;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 9px 18px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #1A6AE0; }

/* Input */
.input {
  border: 1.5px solid #E3E6F0;
  border-radius: 6px;
  padding: 9px 12px;
  font-size: 14px;
  color: #1A1E2E;
  background: #FFFFFF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #2D7FF9;
  box-shadow: 0 0 0 3px rgba(45,127,249,0.12);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--vote-width` | `52px` | Fixed vote button column width |
| `--spacing-xs` | `4px` | Vote button internal gap |
| `--spacing-sm` | `8px` | Post meta gaps |
| `--spacing-md` | `16px` | Post row padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `32px` | Page gutter |
| `--sidebar-width` | `220px` | Board list sidebar |
| `--radius-sm` | `4px` | Status badges |
| `--radius-md` | `6px` | Buttons, inputs |
| `--radius-lg` | `8px` | Vote buttons |

## 6. Depth & Elevation
```css
.shadow-post { box-shadow: 0 1px 3px rgba(0,0,0,0.04); }
.shadow-hover { box-shadow: 0 2px 8px rgba(0,0,0,0.06); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.12); }
```

## 7. Do's and Don'ts
**Do:**
- Place the vote button on the left side of each post row — it's the primary action
- The voted state turns the vote button blue-filled
- Status badges are color-coded pills: each status has a consistent color
- Sort posts by vote count by default

**Don't:**
- Don't hide the vote count — it's the primary social signal
- Don't use the same color for multiple statuses
- Don't add heavy visual weight to comment counts — they're secondary
- Don't reorder feedback boards without user control

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single column; vote button above post title |
| Tablet | 768px | Board sidebar collapses; list view |
| Desktop | 1024px | Sidebar + post list + optional detail panel |
| Wide | 1440px | Wider post list with more meta visible |

## 9. Agent Prompt Guide
```
You are designing for Canny — a customer feedback and voting platform.
Use a white background with blue (#2D7FF9) as the primary accent for votes and CTAs.
Every feedback post row has a vote button on the left (upward arrow + count) that turns blue when voted.
Status badges are color-coded pills on each post: blue=open, orange=planned, purple=in-progress, green=complete.
Post rows hover with a subtle gray background; vote buttons hover with a blue tint.
Keep UI minimal: post title + vote count + status badge is all that's needed per row.
Tone is community-driven, democratic, and feedback-first.
```
