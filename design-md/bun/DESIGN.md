# Bun Design System
> Fast JavaScript runtime with a warm, minimal dark aesthetic — dark charcoal surfaces, amber-gold brand accent, and developer-documentation-first UI.

---

## 1. Visual Theme & Atmosphere
Bun is an all-in-one JavaScript runtime focused on speed. The website and docs are minimal, dark, and confident — reflecting a tool built for developers who care about performance. The brand's warm amber-gold accent (inspired by the "bun" emoji) gives the otherwise dark interface a distinctive warmth. The documentation is the primary interface: clean prose, syntax-highlighted code blocks, and a sidebar navigator. The aesthetic says: fast, modern, no-nonsense.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FBBC05` | Brand amber, CTAs, highlights |
| `--color-primary-dark` | `#E0A800` | Hover/active |
| `--color-primary-dim` | `rgba(251,188,5,0.12)` | Subtle highlights |
| `--color-bg-base` | `#18181B` | App/page background |
| `--color-bg-sidebar` | `#111113` | Left doc sidebar |
| `--color-bg-card` | `#1E1E22` | Card, elevated surfaces |
| `--color-bg-code` | `#0F0F11` | Code blocks |
| `--color-bg-elevated` | `#27272A` | Dropdowns, tooltips |
| `--color-border` | `#2E2E35` | Default borders |
| `--color-border-subtle` | `#232328` | Subtle dividers |
| `--color-text-primary` | `#FAFAFA` | Headings, body text |
| `--color-text-secondary` | `#A1A1AA` | Labels, meta |
| `--color-text-muted` | `#52525B` | Placeholders, disabled |
| `--color-code-string` | `#98C379` | String literals |
| `--color-code-keyword` | `#C678DD` | Keywords |
| `--color-code-function` | `#61AFEF` | Functions |
| `--color-success` | `#4ADE80` | Pass, success |
| `--color-error` | `#F87171` | Fail, error |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 15px;
--font-size-md: 17px;
--font-size-h4: 18px;
--font-size-h3: 20px;
--font-size-h2: 24px;
--font-size-h1: 32px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.3;
--line-height-base: 1.6;
--line-height-body: 1.75;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| H1 / Hero | 32px | 700 | 1.25 |
| H2 | 24px | 700 | 1.3 |
| H3 | 20px | 600 | 1.35 |
| Body / Docs | 15px | 400 | 1.75 |
| Sidebar Label | 13px | 400 | 1.5 |
| Code | 13px | 400 | 1.65 |

## 4. Component Stylings
```css
/* CTA Button */
.button-primary {
  background: #FBBC05;
  color: #18181B;
  border: none;
  border-radius: 8px;
  padding: 10px 22px;
  font-size: 14px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #E0A800; }

/* Install Command Bar */
.install-bar {
  background: #0F0F11;
  border: 1px solid #2E2E35;
  border-radius: 8px;
  padding: 14px 20px;
  display: flex;
  align-items: center;
  gap: 10px;
  font-family: var(--font-mono);
  font-size: 14px;
}
.install-bar__prompt { color: #FBBC05; user-select: none; }
.install-bar__command { color: #FAFAFA; }
.install-bar__copy {
  margin-left: auto;
  background: #27272A;
  border: 1px solid #2E2E35;
  border-radius: 6px;
  padding: 4px 10px;
  font-size: 12px;
  color: #A1A1AA;
  cursor: pointer;
  transition: background 0.12s;
}
.install-bar__copy:hover { background: #3F3F46; color: #FAFAFA; }

/* Code Block */
.code-block {
  background: #0F0F11;
  border: 1px solid #2E2E35;
  border-radius: 10px;
  overflow: hidden;
  margin: 20px 0;
}
.code-block__header {
  background: #1E1E22;
  padding: 8px 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid #2E2E35;
}
.code-block__lang {
  font-size: 11px;
  font-weight: 600;
  color: #A1A1AA;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-family: var(--font-mono);
}
.code-block__body {
  padding: 20px;
  font-family: var(--font-mono);
  font-size: 13px;
  line-height: 1.65;
  color: #FAFAFA;
  overflow-x: auto;
}

/* Benchmark Card */
.benchmark-card {
  background: #1E1E22;
  border: 1px solid #2E2E35;
  border-radius: 10px;
  padding: 20px;
}
.benchmark-label {
  font-size: 12px;
  font-weight: 600;
  color: #A1A1AA;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  margin-bottom: 12px;
}
.benchmark-bar-row {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 8px;
}
.benchmark-name { font-size: 13px; color: #FAFAFA; width: 80px; flex-shrink: 0; }
.benchmark-bar-track { flex: 1; background: #2E2E35; border-radius: 100px; height: 6px; }
.benchmark-bar-fill { height: 100%; border-radius: 100px; background: #FBBC05; }
.benchmark-bar-fill--other { background: #3F3F46; }
.benchmark-value { font-size: 12px; color: #A1A1AA; font-family: var(--font-mono); width: 80px; text-align: right; }

/* Sidebar Item */
.sidebar-item {
  display: flex;
  align-items: center;
  gap: 6px;
  padding: 5px 12px;
  border-radius: 6px;
  cursor: pointer;
  font-size: 13px;
  color: #A1A1AA;
  transition: background 0.08s, color 0.08s;
  text-decoration: none;
}
.sidebar-item:hover { color: #FAFAFA; background: #1E1E22; }
.sidebar-item--active { color: #FBBC05; background: rgba(251,188,5,0.08); }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--docs-max-width` | `720px` | Documentation content |
| `--sidebar-width` | `260px` | Left documentation nav |
| `--spacing-xs` | `4px` | Inline gaps |
| `--spacing-sm` | `8px` | Sidebar item spacing |
| `--spacing-md` | `16px` | Section padding |
| `--spacing-lg` | `24px` | Block spacing |
| `--spacing-xl` | `40px` | Page gutter |
| `--radius-sm` | `4px` | Inline elements |
| `--radius-md` | `8px` | Buttons, bars |
| `--radius-lg` | `10px` | Code blocks, cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.7); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Show install command in a styled terminal bar with an amber prompt character
- Benchmark cards use amber bars for Bun, gray for competitors
- Active sidebar item has amber text and subtle amber background tint
- Code blocks have a language label in the header

**Don't:**
- Don't use amber for error states — use red (#F87171)
- Don't show documentation in a sans-serif body font — use 15px with 1.75 line height
- Don't add heavy UI chrome around code blocks — the code should be the focus

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Full-width docs; sidebar hidden |
| Tablet | 768px | Collapsible sidebar + docs |
| Desktop | 1024px | Sidebar + content area |
| Wide | 1440px | Sidebar + wide content + TOC |

## 9. Agent Prompt Guide
```
You are designing for Bun — fast JavaScript runtime documentation site.
Use a dark charcoal background (#18181B) with darker code surfaces (#0F0F11).
Amber (#FBBC05) is the brand color — install prompt character, active sidebar item, CTA button, benchmark bars.
The install command bar is a styled terminal block with an amber "$" prompt and a copy button.
Code blocks have a dark background with a language label header; syntax highlighting uses green strings, purple keywords, blue functions.
Benchmark cards compare Bun (amber bar) vs competitors (gray bars) with a small label and value.
Tone is developer-fast, minimal-dark, performance-forward, and documentation-first.
```
