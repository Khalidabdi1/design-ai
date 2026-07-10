# Novu Design System
> Open-source notification infrastructure with a dark developer aesthetic — deep surfaces, electric indigo accents, and workflow-driven UI.

---

## 1. Visual Theme & Atmosphere
Novu's design language is built for engineers. Dark backgrounds dominate, keeping focus on the notification workflow graph and code-adjacent content. Indigo and electric blue accents energize the interface and guide users through complex notification pipelines. The aesthetic is precise, technical, and modern — a tool that developers trust because it looks like it was built by developers.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#7C3AED` | Brand violet, CTAs |
| `--color-primary-hover` | `#6D28D9` | Hover/active CTA |
| `--color-primary-light` | `#EDE9FE` | Light badges, backgrounds |
| `--color-accent` | `#60A5FA` | Workflow edges, info highlights |
| `--color-success` | `#34D399` | Delivered, active channels |
| `--color-warning` | `#FBBF24` | Pending, degraded |
| `--color-error` | `#F87171` | Failed, error states |
| `--color-bg-base` | `#0F0F12` | Page background |
| `--color-bg-card` | `#1A1A24` | Card surfaces |
| `--color-bg-elevated` | `#24243A` | Elevated panels, dropdowns |
| `--color-border` | `#2D2D45` | Borders, dividers |
| `--color-text-primary` | `#F4F4F8` | Headings, primary text |
| `--color-text-secondary` | `#9090B0` | Body text, labels |
| `--color-text-muted` | `#5A5A7A` | Placeholders, hints |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 24px;
--font-size-2xl: 32px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 32px | 700 | 1.2 |
| Section Header | 20px | 600 | 1.3 |
| Card Title | 16px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label / Meta | 13px | 500 | 1.4 |
| Code / Caption | 11px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #7C3AED;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 9px 18px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s ease;
}
.button-primary:hover { background: #6D28D9; }

/* Workflow Node */
.workflow-node {
  background: #1A1A24;
  border: 1.5px solid #2D2D45;
  border-radius: 10px;
  padding: 12px 16px;
  min-width: 160px;
  cursor: pointer;
  transition: border-color 0.15s ease;
}
.workflow-node:hover { border-color: #7C3AED; }
.workflow-node--active { border-color: #7C3AED; }
.workflow-node__icon {
  width: 32px;
  height: 32px;
  border-radius: 8px;
  background: rgba(124,58,237,0.2);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 8px;
}

/* Channel Badge */
.channel-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 10px;
  border-radius: 100px;
  font-size: 12px;
  font-weight: 600;
  border: 1px solid #2D2D45;
  background: #24243A;
  color: #9090B0;
}
.channel-badge--active {
  border-color: #34D399;
  color: #34D399;
  background: rgba(52,211,153,0.1);
}

/* Code Block */
.code-block {
  background: #0F0F12;
  border: 1px solid #2D2D45;
  border-radius: 8px;
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #F4F4F8;
  overflow-x: auto;
}

/* Input */
.input {
  background: #1A1A24;
  border: 1.5px solid #2D2D45;
  border-radius: 8px;
  padding: 9px 14px;
  font-size: 14px;
  color: #F4F4F8;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #7C3AED;
  box-shadow: 0 0 0 3px rgba(124,58,237,0.2);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Icon padding |
| `--spacing-sm` | `8px` | Inline gaps |
| `--spacing-md` | `12px` | Card inner spacing |
| `--spacing-lg` | `20px` | Section gaps |
| `--spacing-xl` | `32px` | Page padding |
| `--spacing-2xl` | `48px` | Section separation |
| `--radius-sm` | `6px` | Badges |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `10px` | Cards, nodes |
| `--sidebar-width` | `240px` | Fixed navigation rail |

## 6. Depth & Elevation
```css
.shadow-sm { box-shadow: 0 1px 4px rgba(0,0,0,0.5); }
.shadow-card { box-shadow: 0 4px 12px rgba(0,0,0,0.6); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.7); }
.shadow-node-active { box-shadow: 0 0 0 2px #7C3AED, 0 4px 12px rgba(124,58,237,0.3); }
```

## 7. Do's and Don'ts
**Do:**
- Keep the workflow canvas dark and uncluttered — let edges and nodes carry the hierarchy
- Use channel-specific icons (email, SMS, push, in-app) consistently in workflow nodes
- Surface delivery status with semantic colors: green=delivered, yellow=pending, red=failed
- Monospace font for all code snippets, API keys, and template variables

**Don't:**
- Don't use light backgrounds in the workflow canvas — it breaks the developer aesthetic
- Don't label workflow edges with more than 3 words
- Don't mix rounded and square elements in the same context

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Settings and logs view only; workflow canvas collapses |
| Tablet | 768px | Sidebar hidden, workflow canvas scrollable |
| Desktop | 1024px | Full sidebar + workflow canvas + properties panel |
| Wide | 1440px | Expanded canvas with larger node spacing |

## 9. Agent Prompt Guide
```
You are designing for Novu — open-source notification infrastructure.
Use a deep dark background (#0F0F12) with card surfaces at #1A1A24.
Primary brand color is violet (#7C3AED); use for CTAs, active nodes, and focus rings.
Workflow nodes are rounded rectangles with icon blocks and subtle hover borders.
Channel status badges use semantic colors: green for active, yellow for pending, red for failed.
Typography is Inter at 14px, monospace for code and template content.
Tone is technical, dark, and workflow-first.
```
