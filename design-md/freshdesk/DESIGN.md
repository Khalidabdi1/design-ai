# Freshdesk Design System
> Customer support platform with a vibrant teal brand, clean white workspace, and ticket-centric UI.

---

## 1. Visual Theme & Atmosphere
Freshdesk is a helpdesk built for support teams who need clarity under pressure. The interface is bright and organized — white surfaces with a bold teal accent that signals action. Ticket lists, conversation threads, and customer timelines are the primary views. The design is functional and direct, prioritizing readability and quick triage over decoration. Freshdesk's personality is energetic and approachable, echoing its "Fresh" brand ethos.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#0E76A8` | Brand teal, CTAs, active states |
| `--color-primary-dark` | `#0A5A80` | Hover/active |
| `--color-primary-light` | `#E6F4FA` | Teal tint, selected rows |
| `--color-accent` | `#25C16F` | Resolved, success |
| `--color-bg-base` | `#FFFFFF` | Page/app background |
| `--color-bg-surface` | `#F5F7FA` | Sidebar, table rows |
| `--color-bg-card` | `#FFFFFF` | Ticket cards |
| `--color-border` | `#E0E6ED` | Default borders |
| `--color-text-primary` | `#1A2B3C` | Headings, primary text |
| `--color-text-secondary` | `#67788A` | Labels, meta |
| `--color-text-muted` | `#A8B5C3` | Placeholders, timestamps |
| `--color-success` | `#25C16F` | Resolved tickets |
| `--color-error` | `#E84040` | Urgent, overdue |
| `--color-warning` | `#F5A623` | Pending, waiting |
| `--color-info` | `#0E76A8` | Info messages |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 18px;
--font-size-xl: 22px;
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
| Ticket Subject | 14px | 600 | 1.4 |
| Body / Labels | 14px | 400 | 1.5 |
| Meta / Timestamps | 12px | 400 | 1.4 |
| Badge Text | 11px | 600 | 1.3 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #0E76A8;
  color: #FFFFFF;
  border: none;
  border-radius: 4px;
  padding: 9px 20px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #0A5A80; }

/* Ticket Row */
.ticket-row {
  display: grid;
  grid-template-columns: 24px 2fr 1fr 120px 100px 80px;
  align-items: center;
  padding: 12px 16px;
  border-bottom: 1px solid #E0E6ED;
  cursor: pointer;
  transition: background 0.08s;
}
.ticket-row:hover { background: #F5F7FA; }
.ticket-row--selected { background: #E6F4FA; }
.ticket-row__subject {
  font-size: 14px;
  font-weight: 500;
  color: #1A2B3C;
}
.ticket-row__meta {
  font-size: 12px;
  color: #67788A;
}

/* Priority Badge */
.priority-badge {
  display: inline-block;
  padding: 2px 8px;
  border-radius: 3px;
  font-size: 11px;
  font-weight: 600;
  text-transform: uppercase;
}
.priority-badge--urgent { background: #FEF0F0; color: #C0392B; }
.priority-badge--high { background: #FFF4E6; color: #D4681A; }
.priority-badge--medium { background: #FFFBE6; color: #B8860B; }
.priority-badge--low { background: #F0FAF5; color: #1E7B4B; }

/* Status Label */
.status-label {
  display: inline-block;
  padding: 3px 10px;
  border-radius: 12px;
  font-size: 12px;
  font-weight: 500;
}
.status-label--open { background: #E6F4FA; color: #0E76A8; }
.status-label--pending { background: #FFF4E6; color: #D4681A; }
.status-label--resolved { background: #EDFAF4; color: #1E7B4B; }
.status-label--closed { background: #F0F4F8; color: #67788A; }

/* Conversation Thread */
.message-bubble {
  background: #F5F7FA;
  border-radius: 8px;
  padding: 14px 16px;
  margin-bottom: 12px;
  max-width: 80%;
}
.message-bubble--agent { background: #E6F4FA; margin-left: auto; }
.message-bubble__sender {
  font-size: 12px;
  font-weight: 600;
  color: #67788A;
  margin-bottom: 6px;
}
.message-bubble__text { font-size: 14px; color: #1A2B3C; line-height: 1.5; }

/* Reply Box */
.reply-box {
  background: #FFFFFF;
  border: 1px solid #E0E6ED;
  border-radius: 6px;
  padding: 12px 16px;
  font-size: 14px;
  color: #1A2B3C;
  min-height: 100px;
  resize: vertical;
  transition: border-color 0.15s;
}
.reply-box:focus {
  outline: none;
  border-color: #0E76A8;
  box-shadow: 0 0 0 3px rgba(14,118,168,0.1);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Badge gaps |
| `--spacing-sm` | `8px` | Row padding |
| `--spacing-md` | `16px` | Card inner spacing |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Page padding |
| `--sidebar-width` | `240px` | Left navigation |
| `--list-width` | `400px` | Ticket list panel |
| `--radius-sm` | `4px` | Buttons, inputs |
| `--radius-md` | `8px` | Message bubbles |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.06); }
.shadow-modal { box-shadow: 0 12px 40px rgba(0,0,0,0.12); }
.shadow-dropdown { box-shadow: 0 4px 16px rgba(0,0,0,0.10); }
```

## 7. Do's and Don'ts
**Do:**
- Use teal (#0E76A8) for all primary actions, selected states, and link colors
- Color-code ticket priority badges (red urgent → amber high → yellow medium → green low)
- Show ticket conversation as a threaded message list with agent/customer sides
- Use status labels with pill-rounded corners for quick visual triage

**Don't:**
- Don't use dark backgrounds — Freshdesk is a bright, functional workspace
- Don't mix priority color with status color — they carry distinct meanings
- Don't abbreviate ticket subjects in the detail view

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single view; list or detail |
| Tablet | 768px | Collapsible sidebar + ticket list |
| Desktop | 1024px | Sidebar + list + detail |
| Wide | 1440px | Sidebar + wider list + expanded detail |

## 9. Agent Prompt Guide
```
You are designing for Freshdesk — customer support helpdesk platform.
Use a white background (#FFFFFF) with light gray surfaces (#F5F7FA) for sidebars and hover states.
Teal (#0E76A8) is the primary brand color — CTAs, active nav, selected rows, focus rings.
Tickets show subject, requester, agent, status, and priority in a grid row layout.
Priority badges are color-coded: red (urgent), amber (high), yellow (medium), green (low).
Status labels use pill shapes: open (teal), pending (amber), resolved (green), closed (gray).
Tone is professional, functional, and energetic — built for support teams at speed.
```
