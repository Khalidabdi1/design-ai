# Readwise Design System
> Reading and highlight management platform with a warm, book-inspired aesthetic — warm dark surfaces, amber-gold accents, and reader-first UI.

---

## 1. Visual Theme & Atmosphere
Readwise turns passive reading into an active practice. The interface is warm and focused — dark surfaces reminiscent of e-ink readers and dimly lit libraries, with amber and gold accents that feel bookmarked and highlighted. The product centers on highlights from books, articles, and tweets, resurfaced via spaced repetition. The design honors the reading experience: unhurried, typographically rich, and visually warm.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#F2A635` | Brand amber, highlights, CTAs |
| `--color-primary-dark` | `#D4891E` | Hover/active |
| `--color-primary-dim` | `rgba(242,166,53,0.15)` | Highlight tint backgrounds |
| `--color-bg-base` | `#1C1C1E` | App background |
| `--color-bg-sidebar` | `#141416` | Left sidebar |
| `--color-bg-card` | `#242428` | Card surfaces |
| `--color-bg-elevated` | `#2E2E34` | Modals, dropdowns |
| `--color-border` | `#38383F` | Default borders |
| `--color-text-primary` | `#F0EDEA` | Body text, headings |
| `--color-text-secondary` | `#9490A0` | Meta, labels |
| `--color-text-muted` | `#5C5870` | Placeholders, disabled |
| `--color-highlight-yellow` | `#F2A635` | Amber highlight |
| `--color-highlight-blue` | `#4B9FE1` | Blue highlight |
| `--color-highlight-pink` | `#E1709F` | Pink highlight |
| `--color-highlight-green` | `#4DC26C` | Green highlight |
| `--color-success` | `#4DC26C` | Synced, reviewed |
| `--color-error` | `#E85D75` | Error states |

## 3. Typography Rules
```css
--font-text: 'Lora', 'Georgia', serif;
--font-sans: 'Inter', -apple-system, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 16px;
--font-size-md: 18px;
--font-size-lg: 22px;
--font-size-xl: 28px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.3;
--line-height-base: 1.6;
--line-height-reader: 1.8;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 22px | 600 | 1.3 |
| Section Header | 15px | 600 | 1.4 |
| Highlight Text | 18px | 400 | 1.8 |
| Book Title | 14px | 600 | 1.4 |
| Author / Meta | 13px | 400 | 1.4 |
| Caption | 11px | 400 | 1.3 |

## 4. Component Stylings
```css
/* Highlight Card */
.highlight-card {
  background: #242428;
  border: 1px solid #38383F;
  border-radius: 10px;
  padding: 20px 24px;
  border-left: 3px solid #F2A635;
  margin-bottom: 12px;
}
.highlight-card__text {
  font-family: var(--font-text);
  font-size: 17px;
  color: #F0EDEA;
  line-height: 1.8;
  margin-bottom: 14px;
}
.highlight-card__source {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 12px;
  color: #9490A0;
}
.highlight-card__book { color: #F2A635; font-weight: 500; }

/* Highlight Color Picker */
.highlight-marker {
  display: inline-block;
  padding: 0 2px;
  border-radius: 2px;
}
.highlight-marker--yellow { background: rgba(242,166,53,0.25); }
.highlight-marker--blue { background: rgba(75,159,225,0.25); }
.highlight-marker--pink { background: rgba(225,112,159,0.25); }
.highlight-marker--green { background: rgba(77,194,108,0.25); }

/* Book Card */
.book-card {
  background: #242428;
  border: 1px solid #38383F;
  border-radius: 10px;
  padding: 16px;
  display: flex;
  gap: 14px;
  cursor: pointer;
  transition: border-color 0.15s;
}
.book-card:hover { border-color: #F2A635; }
.book-card__cover {
  width: 44px;
  height: 60px;
  border-radius: 4px;
  background: #38383F;
  flex-shrink: 0;
  object-fit: cover;
}
.book-card__title {
  font-size: 14px;
  font-weight: 600;
  color: #F0EDEA;
  margin-bottom: 4px;
}
.book-card__author { font-size: 12px; color: #9490A0; }
.book-card__count {
  font-size: 11px;
  color: #F2A635;
  margin-top: 6px;
  font-weight: 500;
}

/* Review Card (Daily Review) */
.review-card {
  background: #242428;
  border-radius: 12px;
  padding: 32px 40px;
  max-width: 640px;
  margin: 0 auto;
  text-align: center;
}
.review-card__quote {
  font-family: var(--font-text);
  font-size: 20px;
  color: #F0EDEA;
  line-height: 1.75;
  margin-bottom: 24px;
}
.review-card__source {
  font-size: 13px;
  color: #9490A0;
}
.review-card__source strong { color: #F2A635; }

/* Sidebar Item */
.sidebar-item {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 7px 14px;
  border-radius: 6px;
  cursor: pointer;
  font-size: 13px;
  font-family: var(--font-sans);
  color: #9490A0;
  transition: background 0.08s, color 0.08s;
}
.sidebar-item:hover { background: #242428; color: #F0EDEA; }
.sidebar-item--active { background: rgba(242,166,53,0.1); color: #F2A635; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--review-max-width` | `640px` | Daily review card |
| `--reader-max-width` | `680px` | Article reader |
| `--sidebar-width` | `240px` | Left nav |
| `--spacing-xs` | `4px` | Tight gaps |
| `--spacing-sm` | `8px` | Card elements |
| `--spacing-md` | `16px` | Section padding |
| `--spacing-lg` | `24px` | Card padding |
| `--spacing-xl` | `40px` | Page gutter |
| `--radius-md` | `6px` | Sidebar items |
| `--radius-lg` | `10px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.4); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.6); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.5); }
```

## 7. Do's and Don'ts
**Do:**
- Use amber (#F2A635) as the highlight accent and left-border on highlight cards
- Show highlight color options: yellow, blue, pink, green with tinted backgrounds
- Book cards display a small cover image, title, author, and highlight count
- Daily review quotes should be centered in a large, generous text block

**Don't:**
- Don't use a pure white background — Readwise reads best on warm dark surfaces
- Don't use sans-serif for highlight text — serif font is part of the reading experience
- Don't truncate highlight text — the full passage matters

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Daily review full screen; sidebar hidden |
| Tablet | 768px | Sidebar drawer + highlight list |
| Desktop | 1024px | Sidebar + highlights + detail |
| Wide | 1440px | Sidebar + books + highlights + reader |

## 9. Agent Prompt Guide
```
You are designing for Readwise — reading and highlight management platform.
Use a warm dark background (#1C1C1E) with card surfaces at #242428.
Amber (#F2A635) is the brand accent — left-border on highlight cards, active sidebar, CTA hover.
Highlight text uses a serif font (Lora) at 17–20px with generous line height (1.75+).
Highlight color options are yellow, blue, pink, green — shown as tinted background marks.
Book cards show a small cover, title, author, and highlight count in a row layout.
Tone is warm, bookish, intellectual, and spaced-repetition-first.
```
