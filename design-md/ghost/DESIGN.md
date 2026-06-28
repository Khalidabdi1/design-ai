# Ghost Design System

> Independent publishing design with elegant dark identity, minimal editorial surfaces, membership-first UX, and creator-owned content clarity.

---

## 1. Visual Theme & Atmosphere

Ghost should feel editorial, independent, and elegant. The design language communicates newsletter publishing, membership subscriptions, content management, and the freedom of owning your audience without platform dependency.

- Mood: elegant, independent, editorial, clean
- Density: low, with generous whitespace, reading-optimized typography, and minimal UI chrome
- Character: near-black brand, white editorial canvas, yellow membership accent, serif headline moments

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--ghost-black` | `#15171A` | Primary brand, body text, and CTA |
| `--ghost-yellow` | `#FF6D00` | Membership and premium content accent |
| `--ghost-blue` | `#3B82F6` | Links and secondary actions |
| `--ghost-green` | `#22C55E` | Published post and subscriber success |
| `--ghost-amber` | `#F59E0B` | Draft and scheduled post state |
| `--ghost-red` | `#EF4444` | Unpublished and error state |
| `--surface-editor` | `#FFFFFF` | Writing canvas |
| `--surface-bg` | `#F9FAFB` | Dashboard background |
| `--surface-dark` | `#15171A` | Portal and dark membership surfaces |
| `--text-primary` | `#15171A` | Body and heading text |
| `--text-secondary` | `#6B7280` | Bylines, dates, and captions |
| `--border-default` | `#E5E7EB` | Subtle dividers and borders |

Near-black is the signature Ghost identity. The orange accent is reserved for membership and paid content — it signals value. Do not dilute by using orange as a general accent.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-serif: "Georgia", "Palatino Linotype", "Times New Roman", serif;
--font-mono: "JetBrains Mono", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Article Title | 44px | 700 | 1.1 |
| Section Title | 28px | 700 | 1.2 |
| Card Title | 22px | 600 | 1.3 |
| Body (Reading) | 18px | 400 | 1.85 |
| Body (UI) | 15px | 400 | 1.6 |
| Byline | 14px | 500 | 1.4 |
| Label | 12px | 600 | 1.35 |

Reading body text uses 18px at 1.85 line-height — Ghost is built for long-form reading comfort.

## 4. Component Stylings

```css
.button-primary {
  min-height: 44px;
  padding: 0 22px;
  border: none;
  border-radius: 6px;
  background: #15171A;
  color: #FFFFFF;
  font: 600 15px/1 Inter, sans-serif;
}

.post-card {
  border-bottom: 1px solid #E5E7EB;
  padding: 24px 0;
}

.membership-badge {
  display: inline-flex;
  padding: 4px 12px;
  border-radius: 999px;
  background: #FF6D00;
  color: #FFFFFF;
  font: 700 12px/1.4 Inter, sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.post-status {
  display: inline-flex;
  padding: 3px 10px;
  border-radius: 999px;
  font: 600 12px/1.4 Inter, sans-serif;
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-4` | `16px` | UI rhythm |
| `--space-6` | `24px` | Card and section padding |
| `--space-10` | `40px` | Dashboard section gaps |
| `--space-16` | `64px` | Reading content vertical rhythm |

Reading content: max-width 740px, centered. The editor should be distraction-free with no sidebar visible while writing. Post list view uses a simple table layout.

## 6. Depth & Elevation

```css
.shadow-card   { box-shadow: 0 1px 3px rgba(21, 23, 26, 0.06); }
.shadow-panel  { box-shadow: 0 8px 24px rgba(21, 23, 26, 0.10); }
.shadow-modal  { box-shadow: 0 24px 56px rgba(21, 23, 26, 0.18); }
```

Ghost's elegance is built on restraint — shadows are minimal. Typography and whitespace carry the hierarchy.

## 7. Do's and Don'ts

Do make the writing experience distraction-free with no persistent sidebar. Do use orange exclusively for membership and paid-content moments. Do give article body text generous line-height. Do not use colorful UI in the reading or writing surface. Do not show non-essential dashboard elements while writing.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | Reading-optimized article view, basic post list |
| Tablet | `768px` | Full post editor, simplified dashboard |
| Desktop | `1200px` | Complete dashboard: posts, members, analytics, settings |

Reading is a universal experience — the reading surface must be perfect on every screen size.

## 9. Agent Prompt Guide

Design like Ghost: near-black CTAs, white editorial canvas, generous reading typography, orange membership accents, distraction-free writing surface, serif article titles, and independent-publishing hierarchy.
