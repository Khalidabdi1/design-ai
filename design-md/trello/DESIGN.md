# Trello Design System

> Visual task management with playful productivity and board-first clarity. Trello's public site uses a bright, approachable design language rooted in white, pale blue, bold blue gradients, rounded cards, and simple productivity metaphors like boards, cards, inboxes, and planners.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Trello feels like **work management simplified into a colorful, visual, low-friction system**. It is more playful than most B2B tools, but still clear and useful.

### Mood & Feeling
- Light and productive
- Friendly, not intimidating
- Visual and easy to understand
- Organized but not corporate-heavy
- Optimistic and motion-ready

### Design Density
**Medium density.** There are lots of feature blocks and examples, but the interface remains approachable because of bold cards, simple metaphors, and generous spacing.

### Visual Character
- Blue-led brand framing
- Rounded cards and illustrated boards
- High-contrast white content shells
- Friendly productivity explanations
- Simple, legible feature modules

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--trello-blue` | `#0C66E4` | Primary action and brand blue |
| `--trello-blue-bright` | `#579DFF` | Brighter support accent |
| `--trello-white` | `#FFFFFF` | Main surface and cards |
| `--trello-surface` | `#F4F5F7` | Soft background fill |
| `--trello-ink` | `#172B4D` | Primary text |

### Support and Utility

| Token | Hex | Role |
|-------|-----|------|
| `--trello-muted` | `#44546F` | Secondary copy |
| `--trello-border` | `#DFE1E6` | Card and divider edges |
| `--trello-purple` | `#8777D9` | Playful support accent |
| `--trello-green` | `#36B37E` | Positive state |
| `--trello-blue-soft` | `#DEEBFF` | Soft background tint |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Charlie Display", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Charlie Text", "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 56px | 700 | 1.04 | -0.02em | `#172B4D` |
| Page Title | 40px | 700 | 1.08 | -0.02em | `#172B4D` |
| Section Title | 30px | 700 | 1.14 | -0.01em | `#172B4D` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#172B4D` |
| Body Large | 18px | 400 | 1.6 | 0 | `#172B4D` |
| Body | 16px | 400 | 1.6 | 0 | `#172B4D` |
| Small Body | 14px | 400 | 1.5 | 0 | `#44546F` |
| Label | 12px | 700 | 1.35 | 0.04em | `#44546F` |

### Typography Philosophy
Trello typography should feel **clear, upbeat, and highly understandable**. It should make productivity features feel accessible rather than dense.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #0c66e4;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #0055cc;
}

.button-secondary {
  background: #ffffff;
  color: #172b4d;
  border: 1px solid #dfe1e6;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Boards and Feature Cards

```css
.board-card {
  background: #ffffff;
  border: 1px solid #dfe1e6;
  border-radius: 20px;
  box-shadow: 0 12px 24px rgba(23, 43, 77, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #172b4d;
  border: 1px solid #dfe1e6;
  border-radius: 12px;
  min-height: 44px;
  padding: 12px 14px;
}
```

### Component Notes
- Board metaphors should stay visually obvious
- Friendly illustrations and bright blues fit naturally
- Cards should feel tactile and approachable rather than severe

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight visual rhythm |
| `--space-3` | `8px` | Small gaps |
| `--space-4` | `12px` | Compact spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card spacing |
| `--space-7` | `32px` | Module separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and product demo spacing |

### Layout Behavior
- Use board-style demos and visual productivity stories
- Keep feature modules easy to browse in sequence
- Support both simple onboarding and more powerful capability discovery
- Use blue and illustration to add energy without losing clarity

### Whitespace Philosophy
Whitespace should feel **supportive and lightweight**, making Trello’s visual productivity model easy to absorb quickly.

---

## 6. Depth & Elevation

### Elevation Strategy
Trello uses **soft card elevation** with friendly, rounded content shells and approachable contrast.

```css
--shadow-soft: 0 8px 18px rgba(23, 43, 77, 0.05);
--shadow-card: 0 16px 28px rgba(23, 43, 77, 0.08);
```

### Surface Hierarchy
- White base
- Soft blue and gray support sections
- Elevated cards and board demos
- Bright blue CTA emphasis

---

## 7. Do's and Don'ts

### Do
- Keep the system visual, simple, and upbeat
- Use boards, cards, and lists as obvious metaphors
- Let blue energy support productivity rather than overwhelm it
- Preserve easy onboarding and approachability

### Don't
- Do not make Trello look like heavy enterprise project software
- Do not overcomplicate feature demos with dense UI noise
- Do not flatten the board metaphor into generic cards
- Do not remove the sense of play and momentum

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked board demos and simplified feature rows |
| Tablet | `768px - 1023px` | Two-column sections and compact board previews |
| Desktop | `1024px+` | Full visual productivity storytelling with wide demo blocks |

### Responsive Rules
- Preserve the board metaphor on small screens
- Keep signup and tour actions obvious
- Prefer swipeable demos over tiny compressed layouts
- Maintain generous card radii and visual simplicity

---

## 9. Agent Prompt Guide

### Quick Reference
- Blue-led, rounded, board-first productivity UI
- Friendly Charlie-style type and approachable feature blocks
- White cards, soft blue tints, and obvious task-management metaphors
- Lightweight but still capable work-management feel

### Prompt Template
```text
Design this like Trello's current public website:
- bright Trello-blue productivity foundation with white rounded cards
- visual board, list, and card metaphors that feel instantly understandable
- friendly, upbeat typography and approachable work-management demos
- soft blue and gray support sections with light card elevation
- simple, visual productivity energy instead of heavy enterprise complexity
```
