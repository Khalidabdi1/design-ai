# Firebase Design System
> Google's application development platform with a warm amber-orange brand, dark console surfaces, and real-time-data-first UI.

---

## 1. Visual Theme & Atmosphere
Firebase is Google's BaaS platform that powers millions of apps. The console is dark and technical — a professional developer environment where real-time data, auth user lists, and storage buckets are the primary views. The brand's amber-orange flame accent brings warmth and energy to an otherwise precise, structured interface. The UI reflects Google's Material Design DNA, adapted for a developer-centric context.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FFCA28` | Brand amber, key highlights |
| `--color-secondary` | `#F57C00` | Brand orange, CTAs |
| `--color-secondary-dark` | `#E65100` | Hover/active CTA |
| `--color-bg-base` | `#111B27` | Console background |
| `--color-bg-card` | `#1A2535` | Card, panel surfaces |
| `--color-bg-elevated` | `#1F2E42` | Dropdowns, modals |
| `--color-bg-sidebar` | `#0D1520` | Left nav |
| `--color-border` | `#253447` | Default borders |
| `--color-text-primary` | `#E8EDF4` | Headings, primary text |
| `--color-text-secondary` | `#8FA3BE` | Labels, secondary |
| `--color-text-muted` | `#4E6680` | Placeholders, disabled |
| `--color-success` | `#34D399` | Active, healthy |
| `--color-error` | `#F87171` | Error, disabled |
| `--color-warning` | `#FBBF24` | Quota, warning |
| `--color-realtime` | `#34D399` | Realtime data indicator |

## 3. Typography Rules
```css
--font-sans: 'Google Sans', 'Roboto', Inter, sans-serif;
--font-mono: 'Roboto Mono', 'JetBrains Mono', monospace;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 13px;
--font-size-md: 15px;
--font-size-lg: 18px;
--font-size-xl: 22px;
--font-size-2xl: 28px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Console Title | 22px | 600 | 1.3 |
| Section Header | 15px | 600 | 1.4 |
| Card Title | 13px | 600 | 1.4 |
| Body / Labels | 13px | 400 | 1.5 |
| Data Value | 13px | 400 | 1.5 |
| Code / Keys | 12px | 400 | 1.6 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #F57C00;
  color: #FFFFFF;
  border: none;
  border-radius: 4px;
  padding: 8px 18px;
  font-size: 13px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
  text-transform: uppercase;
  letter-spacing: 0.06em;
}
.button-primary:hover { background: #E65100; }

/* Console Card */
.console-card {
  background: #1A2535;
  border: 1px solid #253447;
  border-radius: 8px;
  padding: 20px;
}
.console-card__title {
  font-size: 13px;
  font-weight: 600;
  color: #E8EDF4;
  margin-bottom: 12px;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
.console-card__value {
  font-size: 28px;
  font-weight: 600;
  color: #FFCA28;
  font-family: var(--font-mono);
}

/* Realtime Data Row */
.data-row {
  display: grid;
  grid-template-columns: 1fr 2fr;
  align-items: center;
  padding: 6px 12px;
  border-bottom: 1px solid #1F2E42;
  font-size: 12px;
  font-family: var(--font-mono);
  transition: background 0.08s;
}
.data-row:hover { background: #1F2E42; }
.data-row__key { color: #FFCA28; }
.data-row__value { color: #E8EDF4; }

/* Realtime Indicator */
.realtime-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: #34D399;
  animation: pulse 2s infinite;
}
@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.4; }
}

/* Service Card (Auth, Firestore, etc.) */
.service-card {
  background: #1A2535;
  border: 1px solid #253447;
  border-radius: 8px;
  padding: 20px;
  cursor: pointer;
  transition: border-color 0.15s;
  display: flex;
  align-items: center;
  gap: 14px;
}
.service-card:hover { border-color: #F57C00; }
.service-card__icon {
  width: 40px;
  height: 40px;
  border-radius: 8px;
  background: rgba(245,124,0,0.15);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  color: #F57C00;
}
.service-card__name {
  font-size: 14px;
  font-weight: 600;
  color: #E8EDF4;
}

/* Input */
.input {
  background: #1A2535;
  border: 1px solid #253447;
  border-radius: 4px;
  padding: 8px 12px;
  font-size: 13px;
  color: #E8EDF4;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #F57C00;
  box-shadow: 0 0 0 2px rgba(245,124,0,0.15);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Data row padding |
| `--spacing-sm` | `8px` | Card compact spacing |
| `--spacing-md` | `12px` | Panel inner spacing |
| `--spacing-lg` | `20px` | Card padding |
| `--spacing-xl` | `28px` | Page gutter |
| `--sidebar-width` | `256px` | Left navigation |
| `--radius-sm` | `4px` | Buttons, inputs |
| `--radius-md` | `8px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.4); }
.shadow-modal { box-shadow: 0 12px 40px rgba(0,0,0,0.6); }
.shadow-sidebar { box-shadow: 2px 0 8px rgba(0,0,0,0.4); }
```

## 7. Do's and Don'ts
**Do:**
- Use amber (#FFCA28) for data keys and highlighted metrics — it's the brand's most distinctive color
- Pulse animate the realtime indicator dot to show live data
- Uppercase 13px labels for console card section headers
- Service cards have orange icon containers with hover border change

**Don't:**
- Don't use material-style FABs — the Firebase console uses standard buttons
- Don't use the amber accent for error states
- Don't omit the monospace font for data keys and values

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Service cards list; sidebar hidden |
| Tablet | 768px | Compact sidebar + content |
| Desktop | 1024px | Full sidebar + content area |
| Wide | 1440px | Expanded content with more cards per row |

## 9. Agent Prompt Guide
```
You are designing for Firebase — Google's application development platform.
Use a dark navy-charcoal background (#111B27) with card surfaces at #1A2535.
Brand amber (#FFCA28) marks data keys, metric values, and logo accent.
CTAs use orange (#F57C00) in uppercase Material-style buttons with 4px radius.
Realtime data tables use monospace font with amber keys and light-colored values.
Service cards have orange-tinted icon containers and orange hover borders.
Tone is developer-professional, Google-adjacent, and real-time-data-first.
```
