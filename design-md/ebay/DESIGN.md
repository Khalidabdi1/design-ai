# eBay Design System Specification

## 1. Brand Identity

### Brand Overview
eBay is a global e-commerce marketplace connecting buyers and sellers worldwide. Founded in 1995, eBay has evolved from an auction-only platform to a comprehensive marketplace featuring fixed-price listings, deals, and a vast range of product categories from electronics to collectibles.

### Brand Personality
- **Empowering**: Enabling buyers to find unique items and sellers to reach global audiences
- **Trustworthy**: Buyer protection, seller ratings, and secure transactions
- **Diverse**: Embracing the wide variety of products and sellers
- **Dynamic**: Real-time auctions, deals, and competitive pricing
- **Community-Driven**: Connecting collectors, enthusiasts, and everyday shoppers

### Logo Specifications
The eBay logo features the distinctive multicolor wordmark with overlapping letters:
- **Logo Colors**: 
  - Red: #E53238 (e)
  - Blue: #0064D2 (b)
  - Yellow/Gold: #F5AF02 (a)
  - Green: #86B817 (y)
- **Logo Style**: Overlapping, playful letterforms representing connection and community
- **Clear Space**: Minimum clear space equal to the height of the lowercase 'e'
- **Minimum Size**: 40px width for digital applications

### Design System
eBay uses the **Evo Design System** (formerly Skin), a comprehensive component library with:
- Pure CSS framework (@ebay/skin)
- Marko components (@ebay/ebayui-core)
- React components (@ebay/ebayui-core-react)
- BEM methodology for CSS naming
- Accessibility-first (WCAG 2.2 AA compliant)

---

## 2. Color Palette

### Primary Colors
```css
/* eBay Blue - Primary Brand/Action Color */
--color-blue-600: #3665F3;        /* Primary buttons, links */
--color-blue-500: #3E73FF;        /* Hover states */
--color-blue-700: #2C54C8;        /* Active/pressed states */
--color-blue-100: #E6EEFF;        /* Light backgrounds */
```

### Brand Logo Colors
```css
/* Multicolor Logo Palette */
--ebay-red: #E53238;              /* Logo red */
--ebay-blue: #0064D2;             /* Logo blue */
--ebay-yellow: #F5AF02;           /* Logo yellow/gold */
--ebay-green: #86B817;            /* Logo green */
```

### Semantic Colors
```css
/* Background Colors */
--color-background-primary: #FFFFFF;
--color-background-secondary: #F7F7F7;
--color-background-tertiary: #E5E5E5;
--color-background-elevated: #FFFFFF;
--color-background-inverse: #111820;
--color-background-disabled: #E5E5E5;

/* Success/Positive */
--color-green-600: #5BA71B;
--color-background-success: #E8F4E1;
--color-foreground-success: #2E7D0D;

/* Attention/Warning */
--color-yellow-500: #F5AF02;
--color-background-attention: #FEF4D9;
--color-foreground-attention: #8B6914;

/* Error/Critical */
--color-red-600: #E0103A;
--color-background-attention: #FDEDED;
--color-foreground-attention: #CC0000;

/* Foreground/Text Colors */
--color-foreground-primary: #111820;
--color-foreground-secondary: #707070;
--color-foreground-disabled: #A6A6A6;
--color-foreground-on-inverse: #FFFFFF;
--color-foreground-link-primary: #3665F3;
--color-foreground-link-visited: #800080;
```

### Border Colors
```css
--color-border-subtle: #E5E5E5;
--color-border-medium: #C7C7C7;
--color-border-strong: #767676;
--color-border-accent: #3665F3;
--color-border-success: #5BA71B;
--color-border-attention: #F5AF02;
--color-border-disabled: #E5E5E5;
```

### State Layer Colors
```css
--color-state-layer-hover: rgba(0, 0, 0, 0.04);
--color-state-layer-pressed: rgba(0, 0, 0, 0.08);
--color-state-layer-focus: rgba(54, 101, 243, 0.12);
--color-state-layer-selected: rgba(54, 101, 243, 0.08);
```

### Dark Mode Support
```css
/* Dark Theme Colors */
--color-background-primary-dark: #121212;
--color-background-secondary-dark: #1F1F1F;
--color-background-elevated-dark: #2A2A2A;
--color-foreground-primary-dark: #F7F7F7;
--color-foreground-secondary-dark: #A6A6A6;
```

---

## 3. Typography

### Font Family
```css
/* Primary Font Stack */
--font-family-primary: "Market Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;

/* System Font Fallback */
--font-family-system: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;

/* Monospace (code/data) */
--font-family-mono: "SF Mono", Monaco, "Cascadia Code", "Roboto Mono", monospace;
```

### Market Sans
Market Sans is eBay's proprietary typeface, designed for clarity and readability across digital platforms:
- Clean, geometric sans-serif design
- Optimized for screen readability
- Available in multiple weights
- Supports extended character sets

### Type Scale
```css
/* Display/Hero Text */
--font-size-giant: 32px;          /* Hero headings */
--font-size-large-1: 24px;        /* Large display */
--font-size-large-2: 20px;        /* Section headings */

/* Body Text */
--font-size-medium: 16px;         /* Primary body */
--font-size-regular: 14px;        /* Standard body */
--font-size-small: 12px;          /* Secondary text */

/* Detail Text */
--font-size-tiny: 11px;           /* Captions, labels */
```

### Font Weights
```css
--font-weight-regular: 400;
--font-weight-medium: 500;        /* Emphasis */
--font-weight-semibold: 600;      /* Subheadings */
--font-weight-bold: 700;          /* Headings, CTAs */
```

### Line Heights
```css
--line-height-tight: 1.2;         /* Headings */
--line-height-normal: 1.4;        /* Body text */
--line-height-relaxed: 1.6;       /* Long-form content */
```

### Typography Classes
```css
/* Giant Text (always bold) */
.typography-giant { font-size: 32px; font-weight: 700; line-height: 1.2; }

/* Large Text (always bold) */
.typography-large-1 { font-size: 24px; font-weight: 700; line-height: 1.25; }
.typography-large-2 { font-size: 20px; font-weight: 700; line-height: 1.3; }

/* Medium Text */
.typography-medium { font-size: 16px; font-weight: 400; line-height: 1.4; }
.typography-medium.bold-text { font-weight: 700; }
.typography-medium.secondary-text { color: var(--color-foreground-secondary); }

/* Regular Text */
.typography-regular { font-size: 14px; font-weight: 400; line-height: 1.4; }

/* Small Text */
.typography-small { font-size: 12px; font-weight: 400; line-height: 1.4; }
```

---

## 4. Spacing & Layout

### Spacing Scale
```css
/* Base Unit: 4px */
--spacing-50: 2px;
--spacing-100: 4px;
--spacing-200: 8px;
--spacing-300: 12px;
--spacing-400: 16px;
--spacing-500: 20px;
--spacing-600: 24px;
--spacing-800: 32px;
--spacing-1000: 40px;
--spacing-1200: 48px;
--spacing-1600: 64px;
--spacing-2000: 80px;
```

### Page Grid System
eBay uses a responsive page grid system:
```css
/* Mobile (< 601px) */
--page-margin: 16px;
--column-gap: 16px;
--columns: 4;

/* Tablet (601px - 960px) */
--page-margin: 24px;
--column-gap: 24px;
--columns: 8;

/* Desktop (961px - 1280px) */
--page-margin: 48px;
--column-gap: 24px;
--columns: 12;

/* Large Desktop (> 1280px) */
--max-width: 1280px;
--page-margin: auto;
--column-gap: 24px;
--columns: 12;
```

### Layout Grid Classes
```css
/* Container */
.page-grid { max-width: 1280px; margin: 0 auto; padding: 0 var(--page-margin); }

/* Responsive Columns */
.layout-grid { display: grid; gap: var(--column-gap); }
.layout-grid--2-columns { grid-template-columns: repeat(2, 1fr); }
.layout-grid--3-columns { grid-template-columns: repeat(3, 1fr); }
.layout-grid--4-columns { grid-template-columns: repeat(4, 1fr); }
```

### Item Tile Grid
```css
/* Product listing grid configurations */
.item-tile-group { display: grid; gap: 16px; }
.item-tile-group--2-up { grid-template-columns: repeat(2, 1fr); }
.item-tile-group--3-up { grid-template-columns: repeat(3, 1fr); }
.item-tile-group--4-up { grid-template-columns: repeat(4, 1fr); }
.item-tile-group--5-up { grid-template-columns: repeat(5, 1fr); }
.item-tile-group--6-up { grid-template-columns: repeat(6, 1fr); }
```

---

## 5. Component Specifications

### Buttons

#### Primary Button (Buy It Now, Add to Cart)
```css
.btn--primary {
  background-color: #3665F3;
  color: #FFFFFF;
  border: none;
  border-radius: 24px;
  padding: 12px 24px;
  font-size: 14px;
  font-weight: 700;
  min-height: 40px;
  cursor: pointer;
  transition: background-color 150ms ease;
}
.btn--primary:hover { background-color: #2C54C8; }
.btn--primary:active { background-color: #1F3D9E; }
.btn--primary:disabled { background-color: #C7C7C7; color: #767676; }
```

#### Secondary Button
```css
.btn--secondary {
  background-color: transparent;
  color: #3665F3;
  border: 1px solid #3665F3;
  border-radius: 24px;
  padding: 11px 23px;
  font-size: 14px;
  font-weight: 700;
  min-height: 40px;
}
.btn--secondary:hover { background-color: rgba(54, 101, 243, 0.04); }
```

#### Tertiary Button (Text-only)
```css
.btn--tertiary {
  background-color: transparent;
  color: #3665F3;
  border: none;
  padding: 12px 16px;
  font-size: 14px;
  font-weight: 700;
  text-decoration: underline;
}
```

#### Destructive Button
```css
.btn--destructive {
  background-color: #E0103A;
  color: #FFFFFF;
  border: none;
  border-radius: 24px;
  padding: 12px 24px;
  font-weight: 700;
}
```

#### Button Sizes
```css
.btn--small { padding: 8px 16px; min-height: 32px; font-size: 12px; }
.btn--regular { padding: 12px 24px; min-height: 40px; font-size: 14px; }
.btn--large { padding: 16px 32px; min-height: 48px; font-size: 16px; }
```

### Form Elements

#### Text Input
```css
.textbox {
  width: 100%;
  padding: 12px 16px;
  border: 1px solid #767676;
  border-radius: 8px;
  font-size: 14px;
  background-color: #FFFFFF;
  transition: border-color 150ms ease, box-shadow 150ms ease;
}
.textbox:hover { border-color: #111820; }
.textbox:focus {
  border-color: #3665F3;
  box-shadow: 0 0 0 2px rgba(54, 101, 243, 0.2);
  outline: none;
}
.textbox--invalid { border-color: #E0103A; }
.textbox:disabled { background-color: #F7F7F7; border-color: #E5E5E5; }
```

#### Floating Label Input
```css
.floating-label {
  position: relative;
}
.floating-label__input {
  padding: 20px 16px 8px;
  border: 1px solid #767676;
  border-radius: 8px;
}
.floating-label__label {
  position: absolute;
  top: 50%;
  left: 16px;
  transform: translateY(-50%);
  transition: all 150ms ease;
  color: #707070;
}
.floating-label__input:focus + .floating-label__label,
.floating-label__input:not(:placeholder-shown) + .floating-label__label {
  top: 8px;
  transform: translateY(0);
  font-size: 11px;
}
```

#### Select Dropdown
```css
.select {
  appearance: none;
  padding: 12px 40px 12px 16px;
  border: 1px solid #767676;
  border-radius: 8px;
  background-color: #FFFFFF;
  background-image: url("chevron-down.svg");
  background-repeat: no-repeat;
  background-position: right 16px center;
  cursor: pointer;
}
```

#### Checkbox
```css
.checkbox__control {
  width: 18px;
  height: 18px;
  border: 1px solid #767676;
  border-radius: 4px;
  background-color: #FFFFFF;
}
.checkbox__control:checked {
  background-color: #3665F3;
  border-color: #3665F3;
  background-image: url("checkmark.svg");
}
```

#### Radio Button
```css
.radio__control {
  width: 18px;
  height: 18px;
  border: 1px solid #767676;
  border-radius: 50%;
  background-color: #FFFFFF;
}
.radio__control:checked {
  border-color: #3665F3;
  border-width: 5px;
}
```

### Cards & Tiles

#### Item Tile (Product Card)
```css
.item-tile {
  display: flex;
  flex-direction: column;
  background-color: #FFFFFF;
  border-radius: 8px;
  overflow: hidden;
  transition: box-shadow 200ms ease;
}
.item-tile:hover {
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.12);
}
.item-tile__image {
  aspect-ratio: 1;
  width: 100%;
  object-fit: cover;
}
.item-tile__body {
  padding: 12px;
}
.item-tile__title {
  font-size: 14px;
  font-weight: 400;
  line-height: 1.4;
  color: #111820;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
}
.item-tile__price {
  font-size: 16px;
  font-weight: 700;
  color: #111820;
  margin-top: 4px;
}
.item-tile__shipping {
  font-size: 12px;
  color: #5BA71B;
  margin-top: 4px;
}
```

#### Card Component
```css
.card {
  background-color: #FFFFFF;
  border: 1px solid #E5E5E5;
  border-radius: 12px;
  padding: 16px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05);
}
.card--elevated {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  border: none;
}
```

### Navigation

#### Tabs
```css
.tabs__items {
  display: flex;
  border-bottom: 1px solid #E5E5E5;
  gap: 24px;
}
.tabs__item {
  padding: 12px 0;
  font-size: 14px;
  font-weight: 400;
  color: #707070;
  border-bottom: 2px solid transparent;
  cursor: pointer;
}
.tabs__item--selected {
  color: #111820;
  border-bottom-color: #3665F3;
  font-weight: 700;
}
.tabs__item:hover { color: #111820; }
```

#### Breadcrumbs
```css
.breadcrumbs {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  font-size: 12px;
}
.breadcrumbs__item {
  color: #3665F3;
  text-decoration: none;
}
.breadcrumbs__item:hover { text-decoration: underline; }
.breadcrumbs__separator {
  margin: 0 8px;
  color: #707070;
}
.breadcrumbs__item--current {
  color: #111820;
  pointer-events: none;
}
```

#### Pagination
```css
.pagination {
  display: flex;
  align-items: center;
  gap: 4px;
}
.pagination__item {
  min-width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  font-size: 14px;
  color: #111820;
}
.pagination__item:hover { background-color: #F7F7F7; }
.pagination__item--selected {
  background-color: #3665F3;
  color: #FFFFFF;
}
```

---

## 6. Iconography

### Icon System
eBay uses a comprehensive SVG icon system with consistent sizing and styling:

```css
/* Icon Sizes */
--icon-size-small: 16px;
--icon-size-regular: 24px;
--icon-size-large: 32px;
--icon-size-xlarge: 48px;

/* Icon Button */
.icon-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background: transparent;
  border: none;
  cursor: pointer;
}
.icon-btn:hover { background-color: #F7F7F7; }
.icon-btn:active { background-color: #E5E5E5; }
```

### Common Icons
| Icon | Use Case |
|------|----------|
| `icon-search` | Search functionality |
| `icon-cart` | Shopping cart |
| `icon-heart` | Watchlist/favorites |
| `icon-notification` | Alerts and notifications |
| `icon-user` | Account/profile |
| `icon-chevron-down` | Dropdowns, expandable |
| `icon-chevron-right` | Navigation, links |
| `icon-close` | Close/dismiss |
| `icon-menu` | Mobile menu |
| `icon-star` | Ratings |
| `icon-star-filled` | Filled ratings |
| `icon-check` | Success, confirmation |
| `icon-info` | Information |
| `icon-warning` | Warnings |
| `icon-error` | Errors |

### Star Rating
```css
.star-rating {
  display: inline-flex;
  gap: 2px;
}
.star-rating__icon {
  width: 16px;
  height: 16px;
  color: #F5AF02;  /* Gold/yellow for filled stars */
}
.star-rating__icon--empty {
  color: #C7C7C7;  /* Gray for empty stars */
}
```

---

## 7. Motion & Animation

### Timing Functions
```css
/* Standard Easings */
--ease-out: cubic-bezier(0.0, 0.0, 0.2, 1);
--ease-in: cubic-bezier(0.4, 0.0, 1, 1);
--ease-in-out: cubic-bezier(0.4, 0.0, 0.2, 1);
--ease-bounce: cubic-bezier(0.34, 1.56, 0.64, 1);
```

### Duration Tokens
```css
--duration-instant: 0ms;
--duration-fast: 100ms;
--duration-normal: 200ms;
--duration-slow: 300ms;
--duration-slower: 400ms;
--duration-slowest: 500ms;
```

### Common Animations

#### Fade In/Out
```css
@keyframes fade-in {
  from { opacity: 0; }
  to { opacity: 1; }
}
.animate-fade-in {
  animation: fade-in var(--duration-normal) var(--ease-out);
}
```

#### Slide Up
```css
@keyframes slide-up {
  from { transform: translateY(16px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}
.animate-slide-up {
  animation: slide-up var(--duration-slow) var(--ease-out);
}
```

#### Loading Spinner
```css
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
.progress-spinner {
  width: 24px;
  height: 24px;
  border: 2px solid #E5E5E5;
  border-top-color: #3665F3;
  border-radius: 50%;
  animation: spin 800ms linear infinite;
}
```

#### Skeleton Loading
```css
@keyframes shimmer {
  0% { background-position: -200% 0; }
  100% { background-position: 200% 0; }
}
.skeleton {
  background: linear-gradient(
    90deg,
    #F7F7F7 25%,
    #E5E5E5 50%,
    #F7F7F7 75%
  );
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite;
}
```

#### Auction Countdown Animation
```css
@keyframes pulse-urgent {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.7; }
}
.countdown--urgent {
  color: #E0103A;
  animation: pulse-urgent 1s ease-in-out infinite;
}
```

### Transition Standards
```css
/* Interactive Element Transitions */
.btn { transition: background-color 150ms var(--ease-out), transform 100ms var(--ease-out); }
.btn:active { transform: scale(0.98); }

/* Link Hover */
.link { transition: color 100ms var(--ease-out); }

/* Card Hover */
.card { transition: box-shadow 200ms var(--ease-out), transform 200ms var(--ease-out); }
.card:hover { transform: translateY(-2px); }
```

---

## 8. Accessibility

### Focus States
```css
/* Focus Ring - Visible for keyboard navigation */
*:focus-visible {
  outline: 2px solid #3665F3;
  outline-offset: 2px;
}

/* Focus within containers */
.btn:focus-visible {
  box-shadow: 0 0 0 4px rgba(54, 101, 243, 0.3);
  outline: none;
}

/* High contrast focus */
@media (prefers-contrast: high) {
  *:focus-visible {
    outline: 3px solid currentColor;
    outline-offset: 3px;
  }
}
```

### Color Contrast
- Normal text (< 18px): Minimum 4.5:1 contrast ratio
- Large text (>= 18px or 14px bold): Minimum 3:1 contrast ratio
- UI components: Minimum 3:1 contrast ratio
- All eBay design tokens are WCAG 2.2 AA compliant

### Screen Reader Support
```html
<!-- Visually Hidden Text -->
<span class="clipped">Accessible label</span>

<style>
.clipped {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
</style>
```

### ARIA Patterns
```html
<!-- Product Card with Price Announcement -->
<article aria-label="Apple iPhone 14, $599">
  <img src="..." alt="Apple iPhone 14 front and back view">
  <h3>Apple iPhone 14</h3>
  <p aria-label="Price: $599">$599.00</p>
  <p aria-label="Free shipping">Free shipping</p>
</article>

<!-- Auction Countdown -->
<time datetime="PT2H30M" aria-live="polite" aria-label="2 hours and 30 minutes remaining">
  2h 30m
</time>

<!-- Star Rating -->
<div role="img" aria-label="4.5 out of 5 stars rating">
  <!-- Star SVGs -->
</div>

<!-- Add to Watchlist -->
<button aria-pressed="false" aria-label="Add to watchlist">
  <svg aria-hidden="true"><!-- heart icon --></svg>
</button>
```

### Keyboard Navigation
- All interactive elements are focusable via Tab
- Arrow keys navigate within composite widgets (menus, tabs, carousels)
- Enter/Space activate buttons and links
- Escape closes modals and dropdowns
- Skip links provided for navigation bypass

### Touch Targets
```css
/* Minimum touch target: 44x44px (WCAG) */
.touch-target {
  min-width: 44px;
  min-height: 44px;
}

/* eBay standard: 40px minimum with 8px spacing */
.btn { min-height: 40px; }
.icon-btn { min-width: 40px; min-height: 40px; }
```

### Reduced Motion
```css
@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

---

## 9. Platform-Specific Guidelines

### Web Application
- **Framework**: Marko.js for server-side rendering, React for interactive components
- **Responsive Design**: Mobile-first approach with breakpoints at 601px, 961px, 1280px
- **Performance**: Critical CSS inlined, lazy-load images, progressive enhancement
- **Browser Support**: Last 2 versions of major browsers (Chrome, Firefox, Safari, Edge)

### Mobile Web
```css
/* Mobile Viewport */
@media (max-width: 600px) {
  /* Full-width buttons */
  .btn--fluid { width: 100%; }
  
  /* Stacked navigation */
  .header__nav { display: none; }
  .header__menu-btn { display: flex; }
  
  /* 2-column product grid */
  .item-tile-group { grid-template-columns: repeat(2, 1fr); }
  
  /* Larger touch targets */
  .btn { min-height: 48px; }
}
```

### iOS App Guidelines
- Follow Apple Human Interface Guidelines where applicable
- Use native iOS components for system-level interactions
- Maintain eBay brand colors and typography
- Support Dynamic Type for accessibility
- Integrate with Apple Pay using eBay styling

### Android App Guidelines
- Follow Material Design 3 principles adapted for eBay brand
- Use eBay color palette for Material components
- Support system dark mode
- Implement Android-specific navigation patterns
- Integrate Google Pay with eBay styling

### Search Interface
```css
.search-bar {
  display: flex;
  align-items: center;
  height: 48px;
  border: 1px solid #767676;
  border-radius: 24px;
  background-color: #FFFFFF;
  overflow: hidden;
}
.search-bar:focus-within {
  border-color: #3665F3;
  box-shadow: 0 0 0 2px rgba(54, 101, 243, 0.2);
}
.search-bar__input {
  flex: 1;
  border: none;
  padding: 0 16px;
  font-size: 14px;
}
.search-bar__button {
  width: 48px;
  height: 48px;
  background-color: #3665F3;
  border: none;
  display: flex;
  align-items: center;
  justify-content: center;
}
```

### Auction-Specific Components
```css
/* Bid Button */
.btn--bid {
  background-color: #3665F3;
  color: #FFFFFF;
  border-radius: 24px;
  padding: 12px 32px;
  font-weight: 700;
}

/* Current Bid Display */
.bid-display {
  background-color: #E6EEFF;
  padding: 16px;
  border-radius: 8px;
}
.bid-display__label {
  font-size: 12px;
  color: #707070;
}
.bid-display__amount {
  font-size: 24px;
  font-weight: 700;
  color: #111820;
}

/* Countdown Timer */
.countdown {
  font-size: 14px;
  font-weight: 700;
}
.countdown--warning { color: #8B6914; }  /* < 1 hour */
.countdown--urgent { color: #E0103A; }   /* < 10 minutes */

/* Bid History */
.bid-history__item {
  display: flex;
  justify-content: space-between;
  padding: 8px 0;
  border-bottom: 1px solid #E5E5E5;
}
```

### Seller Rating Component
```css
.seller-rating {
  display: flex;
  align-items: center;
  gap: 8px;
}
.seller-rating__percentage {
  font-size: 14px;
  font-weight: 700;
  color: #111820;
}
.seller-rating__feedback {
  font-size: 12px;
  color: #707070;
}
.seller-rating--positive { color: #5BA71B; }
.seller-rating--neutral { color: #707070; }
.seller-rating--negative { color: #E0103A; }
```

### Category Navigation
```css
.category-nav {
  display: flex;
  gap: 16px;
  overflow-x: auto;
  padding: 16px 0;
  -webkit-overflow-scrolling: touch;
}
.category-nav__item {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
  min-width: 80px;
  text-decoration: none;
}
.category-nav__icon {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  background-color: #F7F7F7;
}
.category-nav__label {
  font-size: 12px;
  color: #111820;
  text-align: center;
}
```

### Watch/Save Functionality
```css
.watch-btn {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  padding: 8px 12px;
  border: 1px solid #E5E5E5;
  border-radius: 20px;
  background: #FFFFFF;
  font-size: 12px;
  color: #707070;
  cursor: pointer;
}
.watch-btn:hover {
  background: #F7F7F7;
  border-color: #C7C7C7;
}
.watch-btn--active {
  color: #E0103A;
  border-color: #E0103A;
}
.watch-btn__icon {
  width: 16px;
  height: 16px;
}
```

---

## Additional Resources

### Official Documentation
- **Evo Web Components**: https://opensource.ebay.com/evo-web/
- **GitHub Repository**: https://github.com/eBay/evo-web
- **eBay Design Playbook**: https://playbook.ebay.com/design-system/

### NPM Packages
- `@ebay/skin` - CSS framework
- `@ebay/ebayui-core` - Marko components
- `@ebay/ebayui-core-react` - React components

### Design Principles
1. **Accessibility First**: WCAG 2.2 AA compliance is mandatory
2. **Mobile-First**: Design for smallest screens, enhance for larger
3. **Performance**: Optimize for fast load times and smooth interactions
4. **Consistency**: Use design tokens and components for brand cohesion
5. **Trust**: Clear pricing, shipping info, and seller ratings build confidence
