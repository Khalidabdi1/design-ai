# Appwrite Design System
> Open-source backend platform with a dark developer aesthetic — deep charcoal, vivid pink brand accents, and infrastructure-dashboard UI.

---

## 1. Visual Theme & Atmosphere
Appwrite is an open-source Firebase alternative loved by the developer community. The design is dark and developer-forward, anchored by a vivid pink-magenta brand accent that's unmistakable in the ecosystem. The UI is clean and organized: database collections, auth users, storage buckets, and functions are each presented with clarity and consistency. The tone is technical but approachable — built by and for developers who care about quality.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FD366E` | Brand pink-red, CTAs |
| `--color-primary-dark` | `#D42557` | Hover/active primary |
| `--color-primary-light` | `rgba(253,54,110,0.1)` | Subtle backgrounds |
| `--color-bg-base` | `#19191D` | App background |
| `--color-bg-card` | `#232329` | Card, panel surfaces |
| `--color-bg-elevated` | `#2D2D35` | Dropdowns, elevated panels |
| `--color-bg-input` | `#19191D` | Input backgrounds |
| `--color-border` | `#38383F` | Default borders |
| `--color-border-subtle` | `#2D2D35` | Subtle dividers |
| `--color-text-primary` | `#EDEDF0` | Headings, primary text |
| `--color-text-secondary` | `#97979B` | Labels, secondary |
| `--color-text-muted` | `#56565C` | Placeholders, disabled |
| `--color-success` | `#35D063` | Online, enabled |
| `--color-warning` | `#FDB043` | Degraded, warning |
| `--color-error` | `#FE9567` | Error, critical |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 11px;
--font-size-sm: 12px;
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
| Dashboard Title | 24px | 700 | 1.25 |
| Section Header | 16px | 600 | 1.4 |
| Card Title | 14px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label / Meta | 12px | 500 | 1.4 |
| Code / ID | 12px | 400 | 1.5 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #FD366E;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 9px 18px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #D42557; }

/* Resource Card */
.resource-card {
  background: #232329;
  border: 1px solid #38383F;
  border-radius: 10px;
  padding: 20px;
  cursor: pointer;
  transition: border-color 0.15s;
}
.resource-card:hover { border-color: #FD366E; }
.resource-card__icon {
  width: 40px;
  height: 40px;
  border-radius: 8px;
  background: rgba(253,54,110,0.1);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 12px;
  color: #FD366E;
}
.resource-card__title {
  font-size: 16px;
  font-weight: 600;
  color: #EDEDF0;
}
.resource-card__count {
  font-size: 28px;
  font-weight: 700;
  color: #EDEDF0;
  font-family: var(--font-mono);
  margin-top: 8px;
}

/* Table Row */
.table-row {
  display: grid;
  padding: 12px 16px;
  border-bottom: 1px solid #2D2D35;
  align-items: center;
  font-size: 13px;
  color: #97979B;
  cursor: pointer;
  transition: background 0.08s;
}
.table-row:hover { background: #232329; }
.table-row__id {
  font-family: var(--font-mono);
  font-size: 12px;
  color: #97979B;
}

/* Status Dot */
.status-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  flex-shrink: 0;
}
.status-dot--online { background: #35D063; }
.status-dot--offline { background: #56565C; }
.status-dot--error { background: #FE9567; }

/* Input */
.input {
  background: #19191D;
  border: 1px solid #38383F;
  border-radius: 8px;
  padding: 9px 14px;
  font-size: 14px;
  color: #EDEDF0;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #FD366E;
  box-shadow: 0 0 0 3px rgba(253,54,110,0.12);
}

/* Code Block */
.code-block {
  background: #19191D;
  border: 1px solid #38383F;
  border-radius: 8px;
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 12px;
  color: #EDEDF0;
  line-height: 1.6;
  overflow-x: auto;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Dot + label gaps |
| `--spacing-sm` | `8px` | Row gaps |
| `--spacing-md` | `12px` | Card inner padding |
| `--spacing-lg` | `20px` | Section gaps |
| `--spacing-xl` | `32px` | Page gutter |
| `--sidebar-width` | `240px` | Left navigation |
| `--radius-sm` | `4px` | Badges |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `10px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.4); }
.shadow-card-hover { box-shadow: 0 0 0 1px #FD366E, 0 4px 16px rgba(253,54,110,0.15); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Use the pink accent for hover borders on resource cards — it's the primary interactive signal
- Show resource counts in large monospace numbers
- Resource icons use a pink-tinted background with pink icon color
- Status dots should always accompany status text for accessibility

**Don't:**
- Don't use the pink brand color for error states — use the orange-coral (#FE9567)
- Don't use light backgrounds — Appwrite is always dark
- Don't overload the sidebar with more than 8 navigation items

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Sidebar as bottom tab bar; list views only |
| Tablet | 768px | Sidebar as overlay; condensed cards |
| Desktop | 1024px | Full sidebar + main content area |
| Wide | 1440px | Wider content with multi-column card grids |

## 9. Agent Prompt Guide
```
You are designing for Appwrite — an open-source backend-as-a-service platform.
Use a deep dark background (#19191D) with card surfaces at #232329.
Primary accent is vivid pink (#FD366E) — for CTAs, card hover borders, and icon backgrounds.
Resource cards show a pink-tinted icon, a title, and a large monospace count.
Table rows show document/user IDs in monospace, with status dots for online/offline states.
Code blocks and IDs are always monospace on the darkest background.
Tone is developer-focused, open-source-proud, and precision-dark.
```
