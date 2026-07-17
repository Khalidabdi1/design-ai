# Lemon Squeezy Design System
> Merchant of record and digital commerce platform with a bright, playful yellow brand and clean, conversion-focused UI.

---

## 1. Visual Theme & Atmosphere
Lemon Squeezy makes selling digital products delightfully simple. The brand is warm and playful — vivid lemon yellow pops against clean whites, giving the platform an energetic, friendly personality that stands out from sterile fintech UIs. The interface centers on product listings, checkout flows, and revenue dashboards. The tone is optimistic and creator-friendly, signaling that commerce should be fun.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FCD34D` | Brand lemon yellow, CTAs, highlights |
| `--color-primary-dark` | `#F59E0B` | Hover/active |
| `--color-primary-text` | `#1C1C1C` | Text on yellow backgrounds |
| `--color-accent` | `#6C63FF` | Secondary accent, links |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-surface` | `#FAFAFA` | Card backgrounds, table rows |
| `--color-bg-yellow-tint` | `#FFFBEB` | Yellow highlight backgrounds |
| `--color-border` | `#E5E7EB` | Default borders |
| `--color-text-primary` | `#111827` | Headings, primary text |
| `--color-text-secondary` | `#6B7280` | Labels, meta |
| `--color-text-muted` | `#9CA3AF` | Placeholders, disabled |
| `--color-success` | `#10B981` | Payments success, active |
| `--color-error` | `#EF4444` | Failed payments, error |
| `--color-warning` | `#F59E0B` | Pending, review |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
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
| Dashboard Title | 28px | 700 | 1.25 |
| Section Header | 16px | 600 | 1.4 |
| Card Label | 13px | 500 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Revenue Figure | 36px | 700 | 1.2 |
| Meta / Caption | 12px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary CTA Button */
.button-primary {
  background: #FCD34D;
  color: #1C1C1C;
  border: none;
  border-radius: 8px;
  padding: 10px 22px;
  font-size: 14px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #F59E0B; }

/* Revenue Stat Card */
.stat-card {
  background: #FFFFFF;
  border: 1px solid #E5E7EB;
  border-radius: 12px;
  padding: 24px;
}
.stat-card__label {
  font-size: 13px;
  font-weight: 500;
  color: #6B7280;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  margin-bottom: 8px;
}
.stat-card__value {
  font-size: 32px;
  font-weight: 700;
  color: #111827;
  line-height: 1.2;
}
.stat-card__change {
  font-size: 13px;
  font-weight: 500;
  color: #10B981;
  margin-top: 4px;
}
.stat-card__change--down { color: #EF4444; }

/* Product Card */
.product-card {
  background: #FFFFFF;
  border: 1px solid #E5E7EB;
  border-radius: 12px;
  overflow: hidden;
  cursor: pointer;
  transition: box-shadow 0.15s, border-color 0.15s;
}
.product-card:hover {
  box-shadow: 0 8px 24px rgba(0,0,0,0.08);
  border-color: #FCD34D;
}
.product-card__cover {
  height: 160px;
  background: #FFFBEB;
  display: flex;
  align-items: center;
  justify-content: center;
}
.product-card__body { padding: 16px; }
.product-card__name {
  font-size: 15px;
  font-weight: 600;
  color: #111827;
  margin-bottom: 4px;
}
.product-card__price {
  font-size: 16px;
  font-weight: 700;
  color: #111827;
}

/* Order Status Badge */
.order-badge {
  display: inline-block;
  padding: 3px 10px;
  border-radius: 100px;
  font-size: 12px;
  font-weight: 600;
}
.order-badge--paid { background: #D1FAE5; color: #065F46; }
.order-badge--pending { background: #FFFBEB; color: #92400E; }
.order-badge--refunded { background: #F3F4F6; color: #6B7280; }
.order-badge--failed { background: #FEE2E2; color: #991B1B; }

/* Input */
.input {
  background: #FFFFFF;
  border: 1px solid #E5E7EB;
  border-radius: 8px;
  padding: 10px 14px;
  font-size: 14px;
  color: #111827;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #FCD34D;
  box-shadow: 0 0 0 3px rgba(252,211,77,0.2);
}
.input::placeholder { color: #9CA3AF; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Badge gaps |
| `--spacing-sm` | `8px` | Card compact spacing |
| `--spacing-md` | `16px` | Section padding |
| `--spacing-lg` | `24px` | Card padding |
| `--spacing-xl` | `40px` | Page gutter |
| `--sidebar-width` | `240px` | Left navigation |
| `--radius-sm` | `6px` | Badges |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `12px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.06); }
.shadow-hover { box-shadow: 0 8px 24px rgba(0,0,0,0.08); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.12); }
```

## 7. Do's and Don'ts
**Do:**
- Use lemon yellow (#FCD34D) for the primary CTA — it's the brand's signature pop
- Revenue stats use large, bold type — the number is the hero
- Product cards hover with a yellow border to reinforce the brand
- Order status badges are rounded pills with semantic colors

**Don't:**
- Don't use yellow for error states — use red (#EF4444)
- Don't use all-caps buttons — Lemon Squeezy has a friendly, not corporate, tone
- Don't make the product cover image too dark — the UI leans bright and optimistic

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single column; sidebar hidden |
| Tablet | 768px | Compact sidebar + content |
| Desktop | 1024px | Full sidebar + stats + product grid |
| Wide | 1440px | Wider grid; more stats visible |

## 9. Agent Prompt Guide
```
You are designing for Lemon Squeezy — digital commerce and merchant of record platform.
Use a clean white background (#FFFFFF) with light surfaces (#FAFAFA) for cards.
Lemon yellow (#FCD34D) is the signature brand color — CTA buttons, hover borders, focus rings.
Revenue stat cards feature large bold numbers as the primary visual element.
Product cards are rounded (12px) with a soft yellow cover area; they pop on hover with a yellow border.
Order badges are pill-shaped with semantic colors (green=paid, amber=pending, gray=refunded, red=failed).
Tone is friendly, optimistic, creator-focused, and commerce-forward.
```
