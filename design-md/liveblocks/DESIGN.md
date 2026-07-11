# Liveblocks Design System
> Real-time collaboration infrastructure with a clean developer aesthetic — dark surfaces, electric blue presence indicators, and multiplayer-first UI patterns.

---

## 1. Visual Theme & Atmosphere
Liveblocks is the invisible layer that makes apps collaborative. Its design system reflects this: clean, precise, and unobtrusive — documentation and dashboards that help developers understand and integrate real-time features without friction. The palette is dark with electric blue presence indicators that evoke live cursors, active connections, and simultaneous users. The UI is minimal but energetic.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#5C6BC0` | Brand indigo-blue |
| `--color-primary-bright` | `#6366F1` | CTA buttons, active states |
| `--color-presence-1` | `#3B82F6` | User presence color 1 |
| `--color-presence-2` | `#8B5CF6` | User presence color 2 |
| `--color-presence-3` | `#EC4899` | User presence color 3 |
| `--color-presence-4` | `#10B981` | User presence color 4 |
| `--color-bg-base` | `#0A0A0B` | App background |
| `--color-bg-card` | `#141415` | Card surfaces |
| `--color-bg-elevated` | `#1E1E20` | Elevated panels |
| `--color-border` | `#2A2A2E` | Default borders |
| `--color-text-primary` | `#FAFAFA` | Headings, primary |
| `--color-text-secondary` | `#A1A1AA` | Body text, labels |
| `--color-text-muted` | `#52525B` | Placeholders, disabled |
| `--color-success` | `#22C55E` | Connected, online |
| `--color-error` | `#EF4444` | Disconnected, error |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 28px;
--font-size-2xl: 36px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 36px | 700 | 1.2 |
| Section Header | 20px | 600 | 1.3 |
| Card Title | 16px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label | 13px | 500 | 1.4 |
| Code | 13px | 400 | 1.6 |
| Caption | 11px | 400 | 1.4 |

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

/* Presence Avatar */
.presence-avatar {
  width: 28px;
  height: 28px;
  border-radius: 50%;
  border: 2px solid var(--color-presence-1);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 11px;
  font-weight: 700;
  color: #FFFFFF;
  background: var(--color-presence-1);
}
.presence-avatar--overlap {
  margin-left: -8px;
}

/* Live Cursor Indicator */
.live-cursor {
  position: absolute;
  pointer-events: none;
  display: flex;
  align-items: flex-start;
  gap: 6px;
}
.live-cursor__label {
  padding: 3px 8px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
  color: #FFFFFF;
  background: var(--color-presence-1);
  white-space: nowrap;
  margin-top: 16px;
}

/* Connection Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 10px;
  border-radius: 100px;
  font-size: 12px;
  font-weight: 600;
  background: #141415;
  border: 1px solid #2A2A2E;
  color: #A1A1AA;
}
.status-badge::before {
  content: '';
  width: 6px;
  height: 6px;
  border-radius: 50%;
  background: currentColor;
}
.status-badge--connected { color: #22C55E; border-color: rgba(34,197,94,0.2); }
.status-badge--disconnected { color: #EF4444; border-color: rgba(239,68,68,0.2); }

/* Code Snippet Card */
.code-card {
  background: #0A0A0B;
  border: 1px solid #2A2A2E;
  border-radius: 10px;
  overflow: hidden;
}
.code-card__header {
  padding: 10px 16px;
  background: #141415;
  border-bottom: 1px solid #2A2A2E;
  font-size: 12px;
  font-weight: 600;
  color: #A1A1AA;
}
.code-card__body {
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #FAFAFA;
  line-height: 1.6;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Presence avatar overlap |
| `--spacing-sm` | `8px` | Compact component gaps |
| `--spacing-md` | `16px` | Card inner padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Page-level gutter |
| `--spacing-2xl` | `64px` | Section separators |
| `--radius-sm` | `4px` | Status dots |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `10px` | Cards |
| `--sidebar-width` | `240px` | Docs navigation |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.6); }
.shadow-cursor { filter: drop-shadow(0 2px 4px rgba(0,0,0,0.4)); }
```

## 7. Do's and Don'ts
**Do:**
- Use distinct colors for each concurrent user's presence indicator
- Show live connection status prominently in multiplayer UI contexts
- Overlap presence avatars with a negative left margin (−8px) for a stack effect
- Use monospace for all integration code and API keys

**Don't:**
- Don't use more than 5–6 simultaneous presence colors
- Don't animate presence indicators excessively — subtle pulse is enough
- Don't use the same color for multiple active users in the same room
- Don't show presence outside of collaborative contexts

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Dashboard and settings; collaborative canvas disabled |
| Tablet | 768px | Sidebar collapses; avatar stack shrinks to 3 |
| Desktop | 1024px | Full layout with sidebar nav and canvas |
| Wide | 1440px | Expanded layout with inline code docs panel |

## 9. Agent Prompt Guide
```
You are designing for Liveblocks — real-time collaboration infrastructure.
Use a near-black background (#0A0A0B) with card surfaces at #141415.
Primary brand is indigo (#6366F1) for CTAs; presence indicators use a rotating palette of blue, purple, pink, and green.
User avatars are circular with a colored border matching their presence color.
Live cursors show a color-matched pointer with a pill label showing the user's name.
Connection status badges use dot + label pattern with semantic color.
Typography is Inter at 14px; monospace for all code integration snippets.
Tone is technical, collaborative, and multiplayer-forward.
```
