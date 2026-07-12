# Basecamp Design System
> Project management and team communication platform with a warm, opinionated aesthetic — cream and forest green surfaces, readable typography, and task-list-first UI.

---

## 1. Visual Theme & Atmosphere
Basecamp has an aesthetic unlike any other project tool — warm, calm, and almost nostalgic in its simplicity. Cream off-white backgrounds, a forest green brand, and a rejection of the anxiety-inducing complexity of newer tools. Everything is a list or a message board. The design is intentionally un-flashy: wide readable text, comfortable spacing, and a confidence that less really is more.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#1D7544` | Brand forest green, CTAs |
| `--color-primary-dark` | `#145C34` | Hover/active primary |
| `--color-primary-light` | `#E8F5EE` | Light backgrounds, badges |
| `--color-bg-base` | `#FFFCF5` | Warm cream page background |
| `--color-bg-card` | `#FFFFFF` | Card surfaces |
| `--color-bg-sidebar` | `#F5F0E8` | Warm sidebar background |
| `--color-text-primary` | `#1A1A18` | Headings, primary text |
| `--color-text-secondary` | `#5C5648` | Body text, labels |
| `--color-text-muted` | `#9C9080` | Timestamps, secondary meta |
| `--color-text-link` | `#1D7544` | Links |
| `--color-border` | `#E0D8C8` | Default borders |
| `--color-border-subtle` | `#EDE8DC` | Dividers |
| `--color-todo-done` | `#1D7544` | Completed todo checkmark |
| `--color-success` | `#1D7544` | Completed, done |
| `--color-error` | `#CC2C2C` | Errors, overdue |
| `--color-overdue` | `#D44D2D` | Past-due dates |

## 3. Typography Rules
```css
--font-sans: 'Calibre', 'Helvetica Neue', Arial, sans-serif;
--font-serif: 'Sentinel', 'Georgia', serif;
--font-size-xs: 12px;
--font-size-sm: 14px;
--font-size-base: 16px;
--font-size-md: 18px;
--font-size-lg: 22px;
--font-size-xl: 28px;
--font-size-2xl: 36px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.3;
--line-height-base: 1.65;
--line-height-reading: 1.8;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 28px | 700 | 1.3 |
| Project Name | 22px | 700 | 1.3 |
| Section Header | 18px | 600 | 1.4 |
| Message Body | 16px | 400 | 1.65 |
| To-do Item | 16px | 400 | 1.5 |
| Timestamp / Meta | 13px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #1D7544;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 11px 22px;
  font-size: 16px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #145C34; }

/* To-do Item */
.todo-item {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  padding: 12px 0;
  border-bottom: 1px solid #EDE8DC;
}
.todo-checkbox {
  width: 22px;
  height: 22px;
  border-radius: 50%;
  border: 2px solid #C0B8A8;
  flex-shrink: 0;
  margin-top: 1px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: border-color 0.12s, background 0.12s;
}
.todo-checkbox:hover { border-color: #1D7544; }
.todo-checkbox--checked {
  background: #1D7544;
  border-color: #1D7544;
  color: #FFFFFF;
}
.todo-text {
  font-size: 16px;
  color: #1A1A18;
  line-height: 1.5;
  flex: 1;
}
.todo-text--done {
  text-decoration: line-through;
  color: #9C9080;
}

/* Message Board Post */
.message-post {
  background: #FFFFFF;
  border: 1px solid #E0D8C8;
  border-radius: 8px;
  padding: 24px;
  margin-bottom: 16px;
}
.message-post__title {
  font-size: 20px;
  font-weight: 700;
  color: #1A1A18;
  margin-bottom: 8px;
}
.message-post__meta {
  font-size: 13px;
  color: #9C9080;
  margin-bottom: 16px;
}
.message-post__body {
  font-size: 16px;
  line-height: 1.65;
  color: #5C5648;
}

/* Project Card */
.project-card {
  background: #FFFFFF;
  border: 1px solid #E0D8C8;
  border-radius: 8px;
  padding: 20px;
  cursor: pointer;
  transition: border-color 0.15s, box-shadow 0.15s;
}
.project-card:hover {
  border-color: #1D7544;
  box-shadow: 0 4px 16px rgba(0,0,0,0.06);
}
.project-card__name {
  font-size: 18px;
  font-weight: 700;
  color: #1A1A18;
}
.project-card__desc {
  font-size: 14px;
  color: #9C9080;
  margin-top: 4px;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Checkbox gaps |
| `--spacing-sm` | `8px` | List item gaps |
| `--spacing-md` | `16px` | Card padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Page-level padding |
| `--content-max-width` | `720px` | Reading column max width |
| `--sidebar-width` | `260px` | Left project sidebar |
| `--radius-sm` | `4px` | Badges |
| `--radius-md` | `6px` | Buttons |
| `--radius-lg` | `8px` | Cards, message posts |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 6px rgba(0,0,0,0.05); }
.shadow-hover { box-shadow: 0 4px 16px rgba(0,0,0,0.06); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.10); }
```

## 7. Do's and Don'ts
**Do:**
- Use circular checkboxes for to-do items — they're more inviting than squares
- Keep message bodies wide and readable at 720px max
- The warm cream background is non-negotiable — it's core to the Basecamp feel
- Show completed todos with strikethrough text in muted color

**Don't:**
- Don't add complex kanban views or timelines — Basecamp is list-first
- Don't use cold blue or aggressive modern palettes — this is a warm brand
- Don't add unnecessary notification badges or urgency indicators
- Don't exceed 2 heading levels in a message post body

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single column; sidebar as drawer |
| Tablet | 768px | Two-panel: project list + content |
| Desktop | 1024px | Sidebar + main content + optional detail |
| Wide | 1440px | Wider content column with side margin |

## 9. Agent Prompt Guide
```
You are designing for Basecamp — project management and team communication.
Use a warm cream background (#FFFCF5) — never pure white.
Forest green (#1D7544) is the only accent: CTAs, checkmarks, active links.
To-do items use circular checkboxes that fill green when complete; text gets strikethrough.
Message board posts are white cards with warm borders and generous line height (1.65).
Typography is large and readable: 16px body, 28px headings, no tight leading.
Tone is warm, calm, opinionated, and anti-complexity.
```
