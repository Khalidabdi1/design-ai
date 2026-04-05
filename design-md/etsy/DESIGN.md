# Etsy Design System

## Overview

Etsy's design system embodies a warm, handcrafted aesthetic that celebrates creativity, artisanship, and human connection. The platform connects millions of buyers with independent sellers offering unique, often handmade or vintage items. The design language emphasizes authenticity, warmth, and discoverability while maintaining trust through clear seller information and social proof.

**Design Philosophy:** Warm, inviting, and craft-focused - celebrating the human touch behind every item while enabling seamless discovery and secure transactions in a global creative marketplace.

---

## 1. Color Palette

### Brand Colors

| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Etsy Orange (Primary) | `#F56400` | `rgb(245, 100, 0)` | Primary brand, CTAs, accents |
| Etsy Coral | `#F1641E` | `rgb(241, 100, 30)` | Secondary brand, hover states |
| Etsy Orange Dark | `#D35400` | `rgb(211, 84, 0)` | Active/pressed states |
| Etsy Orange Light | `#FF7B29` | `rgb(255, 123, 41)` | Highlights, badges |
| Etsy Black | `#222222` | `rgb(34, 34, 34)` | Logo, primary text |

### Background Colors

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-bg-primary` | `#FFFFFF` | Primary page background |
| `--etsy-bg-cream` | `#FDEBD2` | Warm accent backgrounds |
| `--etsy-bg-light-cream` | `#FDF6EC` | Subtle warm backgrounds |
| `--etsy-bg-warm-white` | `#FAF9F7` | Card backgrounds, sections |
| `--etsy-bg-gray-light` | `#F5F5F5` | Secondary backgrounds |
| `--etsy-bg-gray-lighter` | `#FAFAFA` | Subtle separation |
| `--etsy-bg-overlay` | `rgba(34, 34, 34, 0.6)` | Modal overlays |
| `--etsy-bg-hover` | `#F1F1F1` | Interactive hover states |
| `--etsy-bg-selected` | `#FFF4E6` | Selected/active items |

### Semantic Colors

| Category | Token | Value | Usage |
|----------|-------|-------|-------|
| **Success** | `--etsy-success` | `#2E7D32` | Order confirmed, in stock |
| **Success Light** | `--etsy-success-light` | `#E8F5E9` | Success backgrounds |
| **Error** | `--etsy-error` | `#D32F2F` | Validation errors, out of stock |
| **Error Light** | `--etsy-error-light` | `#FFEBEE` | Error backgrounds |
| **Warning** | `--etsy-warning` | `#F57C00` | Low stock, limited time |
| **Warning Light** | `--etsy-warning-light` | `#FFF3E0` | Warning backgrounds |
| **Info** | `--etsy-info` | `#1976D2` | Informational messages |
| **Info Light** | `--etsy-info-light` | `#E3F2FD` | Info backgrounds |
| **Favorite Red** | `--etsy-favorite` | `#E53935` | Heart/favorites icon filled |
| **Star Gold** | `--etsy-star` | `#FBBF24` | Review stars |
| **Star Empty** | `--etsy-star-empty` | `#D1D5DB` | Empty review stars |

### Text Colors

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-text-primary` | `#222222` | Primary headings, important text |
| `--etsy-text-body` | `#333333` | Body text, descriptions |
| `--etsy-text-secondary` | `#595959` | Secondary text, metadata |
| `--etsy-text-tertiary` | `#757575` | Helper text, placeholders |
| `--etsy-text-disabled` | `#9E9E9E` | Disabled states |
| `--etsy-text-inverse` | `#FFFFFF` | Text on dark backgrounds |
| `--etsy-text-link` | `#222222` | Standard links (underlined) |
| `--etsy-text-link-hover` | `#F56400` | Link hover state |
| `--etsy-text-price` | `#222222` | Product prices |
| `--etsy-text-sale` | `#2E7D32` | Sale prices |
| `--etsy-text-original-price` | `#757575` | Strikethrough original price |

### Border Colors

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-border-default` | `#E0E0E0` | Default borders |
| `--etsy-border-light` | `#EEEEEE` | Subtle borders |
| `--etsy-border-dark` | `#BDBDBD` | Emphasized borders |
| `--etsy-border-focus` | `#222222` | Focus ring color |
| `--etsy-border-error` | `#D32F2F` | Error state borders |
| `--etsy-border-input` | `#BDBDBD` | Form input borders |
| `--etsy-border-input-hover` | `#757575` | Input hover state |
| `--etsy-border-input-focus` | `#222222` | Input focus state |

### Icon Colors

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-icon-primary` | `#222222` | Primary icons |
| `--etsy-icon-secondary` | `#595959` | Secondary icons |
| `--etsy-icon-tertiary` | `#757575` | Tertiary/muted icons |
| `--etsy-icon-disabled` | `#BDBDBD` | Disabled icons |
| `--etsy-icon-inverse` | `#FFFFFF` | Icons on dark backgrounds |
| `--etsy-icon-favorite` | `#E53935` | Filled heart |
| `--etsy-icon-favorite-outline` | `#222222` | Unfilled heart outline |

---

## 2. Typography

### Font Families

```css
/* Primary Sans-Serif - Graphik Web */
--etsy-font-primary: 'Graphik Webfont', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;

/* Display/Decorative - Guardian Egyptian */
--etsy-font-display: 'Guardian Egyptian Web', Georgia, 'Times New Roman', serif;

/* System Fallback Stack */
--etsy-font-system: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;

/* Monospace */
--etsy-font-mono: 'SF Mono', SFMono-Regular, Consolas, 'Liberation Mono', Menlo, monospace;
```

### Font Sizes

| Token | Size | Usage |
|-------|------|-------|
| `--etsy-font-size-xs` | 11px | Fine print, legal text |
| `--etsy-font-size-sm` | 12px | Captions, metadata |
| `--etsy-font-size-base` | 13px | Default body text |
| `--etsy-font-size-md` | 14px | Larger body text |
| `--etsy-font-size-lg` | 16px | Emphasized text, subheadings |
| `--etsy-font-size-xl` | 18px | Section headings |
| `--etsy-font-size-2xl` | 20px | Card titles |
| `--etsy-font-size-3xl` | 24px | Page section titles |
| `--etsy-font-size-4xl` | 28px | Page headings |
| `--etsy-font-size-5xl` | 32px | Hero text |
| `--etsy-font-size-6xl` | 40px | Display headings |
| `--etsy-font-size-7xl` | 48px | Large display |

### Font Weights

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-font-weight-light` | 300 | Decorative text |
| `--etsy-font-weight-regular` | 400 | Body text, default |
| `--etsy-font-weight-medium` | 500 | Emphasized text, navigation |
| `--etsy-font-weight-semibold` | 600 | Subheadings, labels |
| `--etsy-font-weight-bold` | 700 | Headings, buttons, prices |

### Line Heights

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-line-height-tight` | 1.2 | Headings, display text |
| `--etsy-line-height-snug` | 1.3 | Compact text |
| `--etsy-line-height-normal` | 1.4 | Default body text |
| `--etsy-line-height-relaxed` | 1.5 | Readable body text |
| `--etsy-line-height-loose` | 1.6 | Long-form content |

### Letter Spacing

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-letter-spacing-tight` | -0.02em | Display headings |
| `--etsy-letter-spacing-normal` | 0 | Body text |
| `--etsy-letter-spacing-wide` | 0.02em | Uppercase labels |
| `--etsy-letter-spacing-wider` | 0.05em | Small caps, badges |

### Typography Hierarchy

| Level | Font | Size | Weight | Line Height | Usage |
|-------|------|------|--------|-------------|-------|
| Display | Guardian Egyptian | 40px | 700 | 1.2 | Hero headlines |
| Heading 1 | Graphik | 28px | 700 | 1.2 | Page titles |
| Heading 2 | Graphik | 24px | 700 | 1.3 | Section titles |
| Heading 3 | Graphik | 20px | 600 | 1.3 | Card headings |
| Heading 4 | Graphik | 16px | 600 | 1.4 | Subsection titles |
| Body Large | Graphik | 14px | 400 | 1.5 | Featured descriptions |
| Body | Graphik | 13px | 400 | 1.4 | Default body |
| Body Small | Graphik | 12px | 400 | 1.4 | Metadata, captions |
| Caption | Graphik | 11px | 400 | 1.3 | Fine print |
| Price | Graphik | 16-20px | 700 | 1.2 | Product prices |

---

## 3. Spacing System

### Base Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-space-0` | 0px | No spacing |
| `--etsy-space-1` | 4px | Minimal spacing |
| `--etsy-space-2` | 8px | Tight spacing |
| `--etsy-space-3` | 12px | Default internal spacing |
| `--etsy-space-4` | 16px | Standard spacing |
| `--etsy-space-5` | 20px | Comfortable spacing |
| `--etsy-space-6` | 24px | Section spacing |
| `--etsy-space-8` | 32px | Large spacing |
| `--etsy-space-10` | 40px | Extra large spacing |
| `--etsy-space-12` | 48px | Page section gaps |
| `--etsy-space-16` | 64px | Major section spacing |
| `--etsy-space-20` | 80px | Hero spacing |
| `--etsy-space-24` | 96px | Maximum spacing |

### Component-Specific Spacing

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-card-padding` | 16px | Product card internal padding |
| `--etsy-card-gap` | 12px | Gap between card elements |
| `--etsy-grid-gap` | 24px | Grid gap between product cards |
| `--etsy-grid-gap-mobile` | 12px | Mobile grid gap |
| `--etsy-section-padding` | 32px | Page section padding |
| `--etsy-nav-height` | 56px | Main navigation height |
| `--etsy-nav-height-mobile` | 48px | Mobile navigation height |
| `--etsy-search-height` | 44px | Search bar height |

### Layout Guidelines

- **Product card padding:** 12-16px on all sides
- **Section spacing:** 32-48px between major sections
- **Grid gap (desktop):** 24px between cards
- **Grid gap (mobile):** 12px between cards
- **Form field spacing:** 16px between fields
- **Button groups:** 8-12px gap between buttons
- **Icon-to-text spacing:** 8px
- **List items:** 8-12px vertical spacing

---

## 4. Border & Radius

### Border Radius

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-radius-none` | 0px | No rounding |
| `--etsy-radius-sm` | 4px | Small elements, badges |
| `--etsy-radius-md` | 8px | Buttons, inputs |
| `--etsy-radius-lg` | 12px | Cards, containers |
| `--etsy-radius-xl` | 16px | Large cards, modals |
| `--etsy-radius-2xl` | 24px | Featured sections |
| `--etsy-radius-full` | 9999px | Pills, avatars, circles |

### Border Width

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-border-width-0` | 0px | No border |
| `--etsy-border-width-1` | 1px | Default borders |
| `--etsy-border-width-2` | 2px | Emphasized borders, focus |
| `--etsy-border-width-3` | 3px | Strong emphasis |

### Common Border Patterns

```css
/* Product card border */
.product-card {
  border: var(--etsy-border-width-1) solid var(--etsy-border-light);
  border-radius: var(--etsy-radius-lg);
}

/* Input field border */
.input {
  border: var(--etsy-border-width-1) solid var(--etsy-border-input);
  border-radius: var(--etsy-radius-md);
}

/* Focus ring */
:focus-visible {
  outline: var(--etsy-border-width-2) solid var(--etsy-border-focus);
  outline-offset: 2px;
}

/* Button border (secondary) */
.button-secondary {
  border: var(--etsy-border-width-1) solid var(--etsy-border-dark);
  border-radius: var(--etsy-radius-full);
}

/* Favorite heart container */
.favorite-button {
  border: none;
  border-radius: var(--etsy-radius-full);
}
```

---

## 5. Shadows & Elevation

### Shadow Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-shadow-none` | none | No shadow |
| `--etsy-shadow-sm` | `0 1px 2px rgba(34, 34, 34, 0.08)` | Subtle lift |
| `--etsy-shadow-md` | `0 2px 8px rgba(34, 34, 34, 0.1)` | Cards at rest |
| `--etsy-shadow-lg` | `0 4px 16px rgba(34, 34, 34, 0.12)` | Hovered cards, dropdowns |
| `--etsy-shadow-xl` | `0 8px 24px rgba(34, 34, 34, 0.15)` | Modals, popovers |
| `--etsy-shadow-2xl` | `0 16px 48px rgba(34, 34, 34, 0.2)` | Large dialogs |

### Card Shadows

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-card-shadow` | `0 2px 4px rgba(34, 34, 34, 0.06)` | Product card default |
| `--etsy-card-shadow-hover` | `0 4px 12px rgba(34, 34, 34, 0.12)` | Product card hover |

### Elevation Hierarchy

| Level | Shadow | Use Case |
|-------|--------|----------|
| Level 0 | `--etsy-shadow-none` | Flat content, inline elements |
| Level 1 | `--etsy-shadow-sm` | Subtle depth |
| Level 2 | `--etsy-shadow-md` | Cards, buttons at rest |
| Level 3 | `--etsy-shadow-lg` | Hovered cards, dropdowns |
| Level 4 | `--etsy-shadow-xl` | Modals, overlays |
| Level 5 | `--etsy-shadow-2xl` | Maximum elevation |

### Z-Index Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-z-base` | 0 | Default stacking |
| `--etsy-z-raised` | 10 | Raised elements |
| `--etsy-z-dropdown` | 100 | Dropdown menus |
| `--etsy-z-sticky` | 200 | Sticky navigation |
| `--etsy-z-overlay` | 300 | Overlay backgrounds |
| `--etsy-z-modal` | 400 | Modal dialogs |
| `--etsy-z-popover` | 500 | Popovers, tooltips |
| `--etsy-z-toast` | 600 | Toast notifications |
| `--etsy-z-maximum` | 9999 | Critical overlays |

---

## 6. Component Specifications

### Buttons

#### Button Types

| Type | Background | Text | Border | Usage |
|------|------------|------|--------|-------|
| Primary | `#222222` | White | None | Main CTAs (Add to cart, Buy now) |
| Primary Orange | `#F56400` | White | None | Brand CTAs, special actions |
| Secondary | White | `#222222` | 1px `#222222` | Secondary actions |
| Tertiary | Transparent | `#222222` | None | Low emphasis actions |
| Outline | Transparent | `#222222` | 2px `#222222` | Filter toggles |
| Favorite | Transparent | Red/Black | None | Heart/favorite button |

#### Button Sizes

| Size | Height | Padding | Font Size | Border Radius |
|------|--------|---------|-----------|---------------|
| Small | 32px | 12px 16px | 13px | 24px (pill) |
| Medium | 40px | 12px 24px | 14px | 24px (pill) |
| Large | 48px | 16px 32px | 16px | 28px (pill) |
| Icon | 40px | 8px | - | 50% (circle) |

#### Button States

```css
/* Primary Button */
.button-primary {
  background: var(--etsy-text-primary);
  color: var(--etsy-text-inverse);
  border: none;
  border-radius: var(--etsy-radius-full);
  padding: 12px 24px;
  font-weight: var(--etsy-font-weight-medium);
  font-size: 14px;
  cursor: pointer;
  transition: all 0.15s ease;
}

.button-primary:hover {
  background: #000000;
  transform: translateY(-1px);
}

.button-primary:active {
  transform: translateY(0);
}

.button-primary:disabled {
  background: var(--etsy-text-disabled);
  cursor: not-allowed;
}

/* Secondary Button */
.button-secondary {
  background: var(--etsy-bg-primary);
  color: var(--etsy-text-primary);
  border: 1px solid var(--etsy-text-primary);
  border-radius: var(--etsy-radius-full);
}

.button-secondary:hover {
  background: var(--etsy-bg-hover);
}

/* Favorite Button */
.button-favorite {
  background: rgba(255, 255, 255, 0.9);
  border: none;
  border-radius: 50%;
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.button-favorite:hover {
  background: rgba(255, 255, 255, 1);
}

.button-favorite.active svg {
  fill: var(--etsy-icon-favorite);
  color: var(--etsy-icon-favorite);
}
```

### Product Cards

```css
.product-card {
  background: var(--etsy-bg-primary);
  border-radius: var(--etsy-radius-lg);
  overflow: hidden;
  transition: box-shadow 0.2s ease, transform 0.2s ease;
  position: relative;
}

.product-card:hover {
  box-shadow: var(--etsy-card-shadow-hover);
  transform: translateY(-2px);
}

.product-card-image {
  aspect-ratio: 1;
  object-fit: cover;
  width: 100%;
}

.product-card-content {
  padding: var(--etsy-space-3);
}

.product-card-shop {
  font-size: var(--etsy-font-size-sm);
  color: var(--etsy-text-secondary);
  margin-bottom: var(--etsy-space-1);
}

.product-card-title {
  font-size: var(--etsy-font-size-base);
  font-weight: var(--etsy-font-weight-regular);
  color: var(--etsy-text-body);
  line-height: var(--etsy-line-height-snug);
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
  margin-bottom: var(--etsy-space-2);
}

.product-card-price {
  font-size: var(--etsy-font-size-lg);
  font-weight: var(--etsy-font-weight-bold);
  color: var(--etsy-text-price);
}

.product-card-price-original {
  font-size: var(--etsy-font-size-sm);
  color: var(--etsy-text-original-price);
  text-decoration: line-through;
  margin-left: var(--etsy-space-2);
}

.product-card-favorite {
  position: absolute;
  top: var(--etsy-space-3);
  right: var(--etsy-space-3);
  z-index: var(--etsy-z-raised);
}
```

### Review Stars

```css
.star-rating {
  display: inline-flex;
  align-items: center;
  gap: 2px;
}

.star {
  width: 14px;
  height: 14px;
  color: var(--etsy-star);
  fill: var(--etsy-star);
}

.star-empty {
  color: var(--etsy-star-empty);
  fill: var(--etsy-star-empty);
}

.star-half {
  position: relative;
}

.star-half::before {
  content: '';
  position: absolute;
  width: 50%;
  height: 100%;
  overflow: hidden;
  color: var(--etsy-star);
}

.review-count {
  font-size: var(--etsy-font-size-sm);
  color: var(--etsy-text-secondary);
  margin-left: var(--etsy-space-1);
}
```

### Shop Badges

```css
/* Star Seller Badge */
.badge-star-seller {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  background: var(--etsy-bg-cream);
  color: var(--etsy-text-primary);
  padding: 4px 8px;
  border-radius: var(--etsy-radius-sm);
  font-size: var(--etsy-font-size-xs);
  font-weight: var(--etsy-font-weight-medium);
}

.badge-star-seller svg {
  color: var(--etsy-star);
  width: 12px;
  height: 12px;
}

/* Free Shipping Badge */
.badge-free-shipping {
  display: inline-flex;
  background: var(--etsy-success-light);
  color: var(--etsy-success);
  padding: 4px 8px;
  border-radius: var(--etsy-radius-sm);
  font-size: var(--etsy-font-size-xs);
  font-weight: var(--etsy-font-weight-medium);
}

/* Sale Badge */
.badge-sale {
  display: inline-flex;
  background: var(--etsy-success);
  color: white;
  padding: 4px 8px;
  border-radius: var(--etsy-radius-sm);
  font-size: var(--etsy-font-size-xs);
  font-weight: var(--etsy-font-weight-bold);
}

/* Bestseller Badge */
.badge-bestseller {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  background: var(--etsy-bg-warm-white);
  border: 1px solid var(--etsy-border-default);
  color: var(--etsy-text-primary);
  padding: 4px 8px;
  border-radius: var(--etsy-radius-sm);
  font-size: var(--etsy-font-size-xs);
  font-weight: var(--etsy-font-weight-medium);
}
```

### Form Inputs

```css
/* Text Input */
.input {
  width: 100%;
  height: 44px;
  padding: 12px 16px;
  background: var(--etsy-bg-primary);
  border: 1px solid var(--etsy-border-input);
  border-radius: var(--etsy-radius-md);
  font-size: var(--etsy-font-size-md);
  color: var(--etsy-text-body);
  transition: border-color 0.15s ease, box-shadow 0.15s ease;
}

.input:hover {
  border-color: var(--etsy-border-input-hover);
}

.input:focus {
  border-color: var(--etsy-border-input-focus);
  outline: none;
  box-shadow: 0 0 0 1px var(--etsy-border-input-focus);
}

.input::placeholder {
  color: var(--etsy-text-tertiary);
}

.input:disabled {
  background: var(--etsy-bg-gray-light);
  color: var(--etsy-text-disabled);
  cursor: not-allowed;
}

.input-error {
  border-color: var(--etsy-error);
}

.input-error:focus {
  box-shadow: 0 0 0 1px var(--etsy-error);
}

/* Search Input */
.search-input {
  height: var(--etsy-search-height);
  padding-left: 44px;
  padding-right: 16px;
  border-radius: var(--etsy-radius-full);
  background-image: url('search-icon.svg');
  background-repeat: no-repeat;
  background-position: 16px center;
  background-size: 20px;
}

/* Select */
.select {
  appearance: none;
  background-image: url('chevron-down.svg');
  background-repeat: no-repeat;
  background-position: right 12px center;
  background-size: 16px;
  padding-right: 40px;
}

/* Checkbox */
.checkbox {
  width: 18px;
  height: 18px;
  border: 1px solid var(--etsy-border-input);
  border-radius: var(--etsy-radius-sm);
  appearance: none;
  cursor: pointer;
  transition: all 0.15s ease;
}

.checkbox:checked {
  background: var(--etsy-text-primary);
  border-color: var(--etsy-text-primary);
  background-image: url('check.svg');
  background-repeat: no-repeat;
  background-position: center;
  background-size: 12px;
}
```

### Navigation

```css
/* Main Navigation Bar */
.nav-main {
  height: var(--etsy-nav-height);
  background: var(--etsy-bg-primary);
  border-bottom: 1px solid var(--etsy-border-light);
  display: flex;
  align-items: center;
  padding: 0 var(--etsy-space-6);
}

/* Logo */
.nav-logo {
  color: var(--etsy-brand-orange);
  font-size: 28px;
  font-weight: var(--etsy-font-weight-bold);
  text-decoration: none;
}

/* Category Navigation */
.nav-categories {
  display: flex;
  gap: var(--etsy-space-4);
  padding: var(--etsy-space-3) var(--etsy-space-6);
  background: var(--etsy-bg-primary);
  border-bottom: 1px solid var(--etsy-border-light);
  overflow-x: auto;
}

.nav-category-item {
  font-size: var(--etsy-font-size-base);
  color: var(--etsy-text-body);
  text-decoration: none;
  white-space: nowrap;
  padding: var(--etsy-space-2) 0;
  border-bottom: 2px solid transparent;
  transition: all 0.15s ease;
}

.nav-category-item:hover {
  color: var(--etsy-text-primary);
}

.nav-category-item.active {
  font-weight: var(--etsy-font-weight-medium);
  border-bottom-color: var(--etsy-text-primary);
}

/* Icon Navigation */
.nav-icon-button {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background: transparent;
  border: none;
  cursor: pointer;
  transition: background 0.15s ease;
}

.nav-icon-button:hover {
  background: var(--etsy-bg-hover);
}

.nav-icon-button svg {
  width: 24px;
  height: 24px;
  color: var(--etsy-icon-primary);
}
```

### Filters

```css
/* Filter Container */
.filter-container {
  display: flex;
  flex-wrap: wrap;
  gap: var(--etsy-space-2);
  padding: var(--etsy-space-4) 0;
  border-bottom: 1px solid var(--etsy-border-light);
}

/* Filter Button */
.filter-button {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 8px 16px;
  background: var(--etsy-bg-primary);
  border: 1px solid var(--etsy-border-dark);
  border-radius: var(--etsy-radius-full);
  font-size: var(--etsy-font-size-base);
  color: var(--etsy-text-body);
  cursor: pointer;
  transition: all 0.15s ease;
}

.filter-button:hover {
  background: var(--etsy-bg-hover);
}

.filter-button.active {
  background: var(--etsy-text-primary);
  color: var(--etsy-text-inverse);
  border-color: var(--etsy-text-primary);
}

/* Filter Chip */
.filter-chip {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 6px 12px;
  background: var(--etsy-bg-selected);
  border: 1px solid var(--etsy-border-default);
  border-radius: var(--etsy-radius-full);
  font-size: var(--etsy-font-size-sm);
}

.filter-chip-remove {
  width: 16px;
  height: 16px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}
```

### Seller Information

```css
/* Shop Info Card */
.shop-info {
  display: flex;
  align-items: center;
  gap: var(--etsy-space-3);
  padding: var(--etsy-space-4);
  background: var(--etsy-bg-warm-white);
  border-radius: var(--etsy-radius-lg);
}

.shop-avatar {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  object-fit: cover;
}

.shop-name {
  font-size: var(--etsy-font-size-md);
  font-weight: var(--etsy-font-weight-medium);
  color: var(--etsy-text-primary);
}

.shop-meta {
  font-size: var(--etsy-font-size-sm);
  color: var(--etsy-text-secondary);
  display: flex;
  align-items: center;
  gap: var(--etsy-space-2);
}

/* Shop Stats */
.shop-stats {
  display: flex;
  gap: var(--etsy-space-6);
  margin-top: var(--etsy-space-3);
}

.shop-stat {
  text-align: center;
}

.shop-stat-value {
  font-size: var(--etsy-font-size-xl);
  font-weight: var(--etsy-font-weight-bold);
  color: var(--etsy-text-primary);
}

.shop-stat-label {
  font-size: var(--etsy-font-size-sm);
  color: var(--etsy-text-secondary);
}
```

---

## 7. Motion & Animation

### Timing Functions

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-ease-default` | `cubic-bezier(0.4, 0, 0.2, 1)` | Standard transitions |
| `--etsy-ease-in` | `cubic-bezier(0.4, 0, 1, 1)` | Enter animations |
| `--etsy-ease-out` | `cubic-bezier(0, 0, 0.2, 1)` | Exit animations |
| `--etsy-ease-in-out` | `cubic-bezier(0.4, 0, 0.2, 1)` | Symmetrical animations |
| `--etsy-ease-bounce` | `cubic-bezier(0.34, 1.56, 0.64, 1)` | Playful bounce |

### Duration Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-duration-instant` | 0ms | No animation |
| `--etsy-duration-fast` | 100ms | Micro-interactions |
| `--etsy-duration-normal` | 150ms | Standard transitions |
| `--etsy-duration-moderate` | 200ms | Medium transitions |
| `--etsy-duration-slow` | 300ms | Complex animations |
| `--etsy-duration-slower` | 400ms | Page transitions |
| `--etsy-duration-slowest` | 500ms | Large element animations |

### Animation Keyframes

```css
/* Fade In */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

/* Fade In Up */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(8px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Scale In */
@keyframes scaleIn {
  from {
    opacity: 0;
    transform: scale(0.95);
  }
  to {
    opacity: 1;
    transform: scale(1);
  }
}

/* Heart Pop */
@keyframes heartPop {
  0% { transform: scale(1); }
  25% { transform: scale(1.2); }
  50% { transform: scale(0.95); }
  100% { transform: scale(1); }
}

/* Slide Down */
@keyframes slideDown {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Shimmer (Loading) */
@keyframes shimmer {
  0% { background-position: -200% 0; }
  100% { background-position: 200% 0; }
}

/* Spin */
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
```

### Common Animation Patterns

```css
/* Card hover lift */
.product-card {
  transition: transform var(--etsy-duration-normal) var(--etsy-ease-out),
              box-shadow var(--etsy-duration-normal) var(--etsy-ease-out);
}

.product-card:hover {
  transform: translateY(-4px);
  box-shadow: var(--etsy-card-shadow-hover);
}

/* Favorite heart animation */
.favorite-button svg {
  transition: transform var(--etsy-duration-fast) var(--etsy-ease-bounce);
}

.favorite-button:active svg {
  animation: heartPop var(--etsy-duration-slow) var(--etsy-ease-out);
}

/* Button hover */
.button {
  transition: background var(--etsy-duration-fast) var(--etsy-ease-default),
              transform var(--etsy-duration-fast) var(--etsy-ease-default);
}

.button:hover {
  transform: translateY(-1px);
}

.button:active {
  transform: translateY(0);
}

/* Dropdown appearance */
.dropdown {
  animation: slideDown var(--etsy-duration-moderate) var(--etsy-ease-out);
}

/* Modal appearance */
.modal {
  animation: scaleIn var(--etsy-duration-slow) var(--etsy-ease-out);
}

/* Loading skeleton */
.skeleton {
  background: linear-gradient(
    90deg,
    var(--etsy-bg-gray-light) 25%,
    var(--etsy-bg-gray-lighter) 50%,
    var(--etsy-bg-gray-light) 75%
  );
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite linear;
}

/* Spinner */
.spinner {
  animation: spin 1s linear infinite;
}
```

---

## 8. Responsive Breakpoints

### Breakpoint Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `--etsy-breakpoint-xs` | 0px | Mobile (extra small) |
| `--etsy-breakpoint-sm` | 480px | Mobile landscape |
| `--etsy-breakpoint-md` | 768px | Tablet |
| `--etsy-breakpoint-lg` | 1024px | Desktop |
| `--etsy-breakpoint-xl` | 1280px | Large desktop |
| `--etsy-breakpoint-2xl` | 1440px | Extra large desktop |

### Media Query Patterns

```scss
// Mobile first (recommended)
$breakpoint-sm: 480px;
$breakpoint-md: 768px;
$breakpoint-lg: 1024px;
$breakpoint-xl: 1280px;
$breakpoint-2xl: 1440px;

// Media query mixins
@mixin sm-up { @media (min-width: $breakpoint-sm) { @content; } }
@mixin md-up { @media (min-width: $breakpoint-md) { @content; } }
@mixin lg-up { @media (min-width: $breakpoint-lg) { @content; } }
@mixin xl-up { @media (min-width: $breakpoint-xl) { @content; } }
@mixin 2xl-up { @media (min-width: $breakpoint-2xl) { @content; } }

// Desktop first
@mixin sm-down { @media (max-width: $breakpoint-sm - 1) { @content; } }
@mixin md-down { @media (max-width: $breakpoint-md - 1) { @content; } }
@mixin lg-down { @media (max-width: $breakpoint-lg - 1) { @content; } }
@mixin xl-down { @media (max-width: $breakpoint-xl - 1) { @content; } }
```

### Product Grid Columns

| Breakpoint | Grid Columns | Card Min Width | Gap |
|------------|--------------|----------------|-----|
| xs (0-479px) | 2 | 140px | 12px |
| sm (480-767px) | 2-3 | 160px | 16px |
| md (768-1023px) | 3-4 | 180px | 20px |
| lg (1024-1279px) | 4-5 | 200px | 24px |
| xl (1280-1439px) | 5-6 | 220px | 24px |
| 2xl (1440px+) | 6+ | 240px | 24px |

### Responsive Layout Guidelines

```css
/* Product Grid */
.product-grid {
  display: grid;
  gap: var(--etsy-grid-gap-mobile);
  grid-template-columns: repeat(2, 1fr);
}

@media (min-width: 480px) {
  .product-grid {
    grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
    gap: 16px;
  }
}

@media (min-width: 768px) {
  .product-grid {
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 20px;
  }
}

@media (min-width: 1024px) {
  .product-grid {
    grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
    gap: var(--etsy-grid-gap);
  }
}

/* Container */
.container {
  width: 100%;
  max-width: 1440px;
  margin: 0 auto;
  padding: 0 16px;
}

@media (min-width: 768px) {
  .container {
    padding: 0 24px;
  }
}

@media (min-width: 1024px) {
  .container {
    padding: 0 32px;
  }
}

/* Navigation - Mobile */
@media (max-width: 767px) {
  .nav-main {
    height: var(--etsy-nav-height-mobile);
    padding: 0 var(--etsy-space-4);
  }
  
  .nav-categories {
    display: none;
  }
  
  .nav-mobile-menu {
    display: flex;
  }
}

@media (min-width: 768px) {
  .nav-mobile-menu {
    display: none;
  }
}
```

### Content Width Guidelines

| Container Type | Max Width | Padding |
|----------------|-----------|---------|
| Full width | 100% | 16px (mobile), 24-32px (desktop) |
| Standard | 1440px | 16px (mobile), 32px (desktop) |
| Narrow | 1200px | 16px (mobile), 32px (desktop) |
| Content | 900px | 16px (mobile), 24px (desktop) |
| Readable | 680px | 16px (mobile), 24px (desktop) |

---

## 9. Accessibility Guidelines

### Color Contrast Requirements

| Element | Minimum Ratio | WCAG Level |
|---------|---------------|------------|
| Body text | 4.5:1 | AA |
| Large text (18px+ bold, 24px+) | 3:1 | AA |
| UI components, icons | 3:1 | AA |
| Focus indicators | 3:1 | AA |

### Etsy Color Contrast Compliance

| Combination | Ratio | Compliant |
|-------------|-------|-----------|
| `#222222` on `#FFFFFF` | 16.1:1 | AAA |
| `#333333` on `#FFFFFF` | 12.6:1 | AAA |
| `#595959` on `#FFFFFF` | 7.0:1 | AAA |
| `#757575` on `#FFFFFF` | 4.6:1 | AA |
| `#FFFFFF` on `#F56400` | 3.4:1 | AA (large text) |
| `#FFFFFF` on `#222222` | 16.1:1 | AAA |
| `#222222` on `#FDEBD2` | 11.8:1 | AAA |

### Focus States

```css
/* Standard focus ring */
:focus-visible {
  outline: 2px solid var(--etsy-border-focus);
  outline-offset: 2px;
}

/* Button focus */
.button:focus-visible {
  outline: 2px solid var(--etsy-border-focus);
  outline-offset: 2px;
}

/* Card focus */
.product-card:focus-visible {
  outline: 2px solid var(--etsy-border-focus);
  outline-offset: 2px;
}

/* Input focus */
.input:focus {
  border-color: var(--etsy-border-input-focus);
  box-shadow: 0 0 0 1px var(--etsy-border-input-focus);
  outline: none;
}

/* Skip link */
.skip-link {
  position: absolute;
  top: -100%;
  left: 16px;
  padding: 8px 16px;
  background: var(--etsy-bg-primary);
  border: 2px solid var(--etsy-border-focus);
  border-radius: var(--etsy-radius-md);
  z-index: var(--etsy-z-maximum);
}

.skip-link:focus {
  top: 16px;
}
```

### Touch Target Sizes

| Element | Minimum Size | Recommended |
|---------|--------------|-------------|
| Buttons | 44px x 44px | 48px x 48px |
| Icon buttons | 44px x 44px | 48px x 48px |
| Favorite hearts | 44px x 44px | 48px x 48px |
| Links (inline) | N/A | Adequate padding |
| Checkboxes/Radios | 44px x 44px | 48px x 48px |
| Filter chips | 32px height | 36px height minimum |

### Interaction State Signifiers

| State | Visual Treatment |
|-------|------------------|
| **Hover** | Background color change, subtle shadow lift |
| **Focus** | Black outline ring (2px, 2px offset) |
| **Active/Pressed** | Slight scale down, darker background |
| **Selected** | Background highlight, checkmark icon |
| **Disabled** | Reduced opacity (40%), cursor: not-allowed |
| **Loading** | Spinner, skeleton shimmer |
| **Error** | Red border, error message below |
| **Favorited** | Red filled heart icon |

### Keyboard Navigation

- All interactive elements must be keyboard accessible
- Tab order follows logical reading order (left-to-right, top-to-bottom)
- Product cards are tabbable with Enter to open
- Favorite buttons accessible via keyboard
- Escape key closes modals, dropdowns, and popovers
- Arrow keys navigate within dropdown menus
- Space/Enter activates buttons and links
- Skip link to bypass navigation

### Screen Reader Guidelines

```html
<!-- Product Card -->
<article class="product-card" aria-labelledby="product-title-123">
  <img src="product.jpg" alt="Handmade ceramic mug with blue glaze" />
  <button 
    class="favorite-button" 
    aria-label="Add to favorites"
    aria-pressed="false"
  >
    <svg aria-hidden="true"><!-- heart icon --></svg>
  </button>
  <div class="product-card-content">
    <a href="/shop/name" class="shop-name">ShopName</a>
    <h3 id="product-title-123">
      <a href="/listing/123">Handmade Ceramic Mug</a>
    </h3>
    <div class="star-rating" aria-label="4.8 out of 5 stars">
      <!-- star icons -->
      <span aria-hidden="true">(1,234)</span>
      <span class="visually-hidden">1,234 reviews</span>
    </div>
    <span class="price" aria-label="$24.99">$24.99</span>
  </div>
</article>

<!-- Badge -->
<span class="badge-star-seller" role="img" aria-label="Star Seller">
  <svg aria-hidden="true"><!-- star icon --></svg>
  Star Seller
</span>

<!-- Review Stars -->
<div class="star-rating" role="img" aria-label="4.5 out of 5 stars">
  <svg aria-hidden="true"><!-- 4 filled stars --></svg>
  <svg aria-hidden="true"><!-- 1 half star --></svg>
</div>

<!-- Loading State -->
<div aria-live="polite" aria-busy="true">
  <span class="visually-hidden">Loading products...</span>
</div>

<!-- Visually Hidden Class -->
<style>
.visually-hidden {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  border: 0;
}
</style>
```

### Motion Preferences

```css
@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
  
  .product-card:hover {
    transform: none;
  }
  
  .skeleton {
    animation: none;
    background: var(--etsy-bg-gray-light);
  }
}
```

### Image Guidelines

- All product images must have descriptive alt text
- Decorative images use `alt=""`
- Icons use `aria-hidden="true"` with adjacent text labels
- Complex images (infographics) include detailed descriptions
- Lazy-loaded images maintain aspect ratio to prevent layout shift

---

## Quick Reference

### CSS Custom Properties Import

```css
:root {
  /* Brand */
  --etsy-orange: #F56400;
  --etsy-coral: #F1641E;
  --etsy-black: #222222;
  
  /* Backgrounds */
  --bg-primary: #FFFFFF;
  --bg-cream: #FDEBD2;
  --bg-warm: #FAF9F7;
  
  /* Text */
  --text-primary: #222222;
  --text-body: #333333;
  --text-secondary: #595959;
  
  /* Typography */
  --font-primary: 'Graphik Webfont', -apple-system, sans-serif;
  --font-size-base: 13px;
  --font-weight-regular: 400;
  --font-weight-medium: 500;
  --font-weight-bold: 700;
  
  /* Spacing */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-6: 24px;
  --space-8: 32px;
  
  /* Borders */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-full: 9999px;
  
  /* Shadows */
  --shadow-card: 0 2px 4px rgba(34, 34, 34, 0.06);
  --shadow-card-hover: 0 4px 12px rgba(34, 34, 34, 0.12);
  
  /* Animation */
  --duration-fast: 100ms;
  --duration-normal: 150ms;
  --ease-default: cubic-bezier(0.4, 0, 0.2, 1);
}
```

### Component Size Reference

| Component | Height | Min Width |
|-----------|--------|-----------|
| Button (small) | 32px | 64px |
| Button (medium) | 40px | 80px |
| Button (large) | 48px | 100px |
| Input field | 44px | 200px |
| Search bar | 44px | 280px |
| Nav height (desktop) | 56px | - |
| Nav height (mobile) | 48px | - |
| Product card | auto | 140px |
| Avatar (small) | 32px | 32px |
| Avatar (medium) | 48px | 48px |
| Avatar (large) | 72px | 72px |
| Badge | 20px | auto |
| Icon (standard) | 24px | 24px |
| Star (rating) | 14px | 14px |

---

## Resources

- [Etsy](https://www.etsy.com)
- [Etsy Seller Handbook](https://www.etsy.com/seller-handbook)
- [Etsy Brand Guidelines](https://www.etsy.com/brand)
- [Etsy Open API Documentation](https://developers.etsy.com)
- [Etsy Engineering Blog](https://www.etsy.com/codeascraft)
