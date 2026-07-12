# Superhuman Design System
> AI-powered email client with a keyboard-first dark aesthetic — obsidian surfaces, gold highlights, and speed-obsessed interaction patterns.

---

## 1. Visual Theme & Atmosphere
Superhuman is designed to make email feel fast, focused, and almost luxurious. The dark interface eliminates distraction while the gold accent signals premium status. Every pixel is intentional — tight typography, minimal chrome, and smooth transitions that reinforce the sense of speed. It reads like a high-end productivity tool used by people who value both aesthetics and efficiency.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#F5A623` | Brand gold, highlights, active states |
| `--color-primary-dark` | `#D4881A` | Hover/active gold |
| `--color-primary-dim` | `rgba(245,166,35,0.12)` | Subtle gold backgrounds |
| `--color-bg-base` | `#141414` | App background |
| `--color-bg-sidebar` | `#1A1A1A` | Sidebar, email list |
| `--color-bg-card` | `#1E1E1E` | Email thread cards |
| `--color-bg-elevated` | `#2A2A2A` | Dropdowns, tooltips |
| `--color-bg-reading` | `#111111` | Reading pane |
| `--color-border` | `#2E2E2E` | Subtle dividers |
| `--color-text-primary` | `#F0F0F0` | Headings, sender names |
| `--color-text-secondary` | `#909090` | Preview text, timestamps |
| `--color-text-muted` | `#505050` | Placeholders, hints |
| `--color-unread` | `#FFFFFF` | Unread message subjects |
| `--color-read` | `#808080` | Read message subjects |
| `--color-success` | `#34D399` | Sent, archived |
| `--color-error` | `#F87171` | Failed, error |

## 3. Typography Rules
```css
--font-sans: -apple-system, 'SF Pro Text', 'Inter', sans-serif;
--font-display: -apple-system, 'SF Pro Display', 'Inter', sans-serif;
--font-serif: 'Georgia', 'Times New Roman', serif;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 15px;
--font-size-lg: 18px;
--font-size-xl: 22px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
--line-height-email: 1.7;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Sender Name (unread) | 14px | 700 | 1.4 |
| Sender Name (read) | 14px | 400 | 1.4 |
| Subject (unread) | 14px | 600 | 1.4 |
| Subject (read) | 14px | 400 | 1.4 |
| Email Preview | 13px | 400 | 1.4 |
| Email Body | 15px | 400 | 1.7 |
| Timestamp | 11px | 400 | 1.3 |

## 4. Component Stylings
```css
/* Email Row */
.email-row {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 20px;
  cursor: pointer;
  border-bottom: 1px solid rgba(255,255,255,0.04);
  transition: background 0.08s;
}
.email-row:hover { background: #1E1E1E; }
.email-row--selected { background: rgba(245,166,35,0.08); border-left: 2px solid #F5A623; }
.email-row--unread .email-row__subject { font-weight: 600; color: #F0F0F0; }
.email-row--read .email-row__subject { font-weight: 400; color: #808080; }

/* Gold Keyboard Hint */
.cmd-hint {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  padding: 2px 6px;
  border-radius: 4px;
  background: rgba(245,166,35,0.12);
  border: 1px solid rgba(245,166,35,0.25);
  font-size: 11px;
  font-weight: 600;
  color: #F5A623;
  font-family: var(--font-sans);
}

/* Split Input (compose "To" field) */
.compose-to {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
  padding: 10px 16px;
  border-bottom: 1px solid #2E2E2E;
  min-height: 44px;
  align-items: center;
}
.recipient-chip {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 3px 10px;
  border-radius: 100px;
  background: #2A2A2A;
  border: 1px solid #383838;
  font-size: 13px;
  font-weight: 500;
  color: #F0F0F0;
}

/* Status Toast */
.status-toast {
  position: fixed;
  bottom: 24px;
  left: 50%;
  transform: translateX(-50%);
  background: #2A2A2A;
  border: 1px solid #383838;
  border-radius: 10px;
  padding: 12px 20px;
  font-size: 14px;
  font-weight: 500;
  color: #F0F0F0;
  display: flex;
  align-items: center;
  gap: 10px;
  box-shadow: 0 8px 32px rgba(0,0,0,0.6);
}
.status-toast .undo-btn {
  color: #F5A623;
  font-weight: 600;
  cursor: pointer;
  background: none;
  border: none;
  padding: 0;
}

/* Avatar */
.avatar {
  width: 36px;
  height: 36px;
  border-radius: 50%;
  flex-shrink: 0;
  background: #2A2A2A;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 13px;
  font-weight: 600;
  color: #F5A623;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--sidebar-width` | `220px` | Mailbox navigation |
| `--list-width` | `360px` | Email list pane |
| `--reading-min` | `480px` | Reading pane minimum |
| `--spacing-xs` | `4px` | Chip gaps |
| `--spacing-sm` | `8px` | Row item gaps |
| `--spacing-md` | `12px` | Section padding |
| `--spacing-lg` | `20px` | Pane padding |
| `--radius-sm` | `4px` | Keyboard hints |
| `--radius-md` | `8px` | Toasts, popovers |
| `--radius-pill` | `100px` | Recipient chips |

## 6. Depth & Elevation
```css
.shadow-toast { box-shadow: 0 8px 32px rgba(0,0,0,0.6); }
.shadow-compose { box-shadow: 0 16px 48px rgba(0,0,0,0.7); }
.shadow-dropdown { box-shadow: 0 4px 16px rgba(0,0,0,0.5); }
```

## 7. Do's and Don'ts
**Do:**
- Use bold weight for unread senders and subjects — it's the primary readability signal
- Show keyboard shortcuts in gold cmd-hint badges throughout the UI
- Animate archive/send actions with a fast upward swipe (150ms)
- Keep the compose window as a floating overlay — never full page

**Don't:**
- Don't use color to mark read/unread — use font weight only
- Don't add heavy toolbar chrome — keyboard is the primary interaction model
- Don't paginate email list — infinite scroll only
- Don't use anything brighter than gold (#F5A623) for highlights

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single pane: list OR reading view |
| Tablet | 768px | Two-pane: list + reading |
| Desktop | 1024px | Three-pane: sidebar + list + reading |
| Wide | 1440px | Expanded reading pane with more whitespace |

## 9. Agent Prompt Guide
```
You are designing for Superhuman — an AI-powered premium email client.
Use a deep dark background (#141414) with dark card surfaces and minimal borders.
The only accent is gold (#F5A623) — used for selected email borders, keyboard hints, and undo actions.
Email rows show avatar, sender, subject, preview, and timestamp in a tight horizontal layout.
Unread emails use bold weight; read emails use regular weight — font weight is the only indicator.
Keyboard hints are small gold-tinted badges showing shortcuts (⌘K, E, R, etc.).
Tone is speed-obsessed, keyboard-first, and premium-dark.
```
