# Walmart Design System

## 1. Brand Overview

### Brand Identity
Walmart is the world's largest retailer, founded in 1962 by Sam Walton with a mission to help people save money and live better. The brand represents accessibility, value, and everyday low prices for millions of customers worldwide.

### Core Values
- **Save Money. Live Better.** - The iconic tagline encapsulating Walmart's promise
- **Everyday Low Prices (EDLP)** - Consistent value without gimmicks
- **Customer-First** - Making shopping easy, affordable, and convenient
- **Community** - Serving local communities across America and beyond
- **Accessibility** - Products and services for everyone

### Brand Personality
- Approachable and friendly
- Trustworthy and reliable
- Value-conscious and practical
- Helpful and service-oriented
- Inclusive and welcoming

### Design Philosophy
Walmart's design system emphasizes clarity, utility, and value communication. Every design decision supports the core mission of helping customers save money while providing a seamless shopping experience across all channels—from superstores to mobile apps.

---

## 2. Color Palette

### Primary Colors

#### Walmart Blue
```
Primary Blue: #0071DC
RGB: 0, 113, 220
HSL: 209°, 100%, 43%
```
The signature Walmart Blue represents trust, reliability, and the brand's heritage. Used for primary actions, headers, and key brand moments.

#### Walmart Yellow (Spark Yellow)
```
Spark Yellow: #FFC220
RGB: 255, 194, 32
HSL: 44°, 100%, 56%
```
The vibrant yellow from the Spark logo, representing optimism, savings, and value. Used for highlights, promotions, and the iconic Spark element.

### Secondary Colors

#### Action Blue
```
Action Blue: #004F9A
RGB: 0, 79, 154
HSL: 209°, 100%, 30%
```
A deeper blue for hover states, active elements, and text links.

#### Success Green
```
Success Green: #2E7D32
RGB: 46, 125, 50
HSL: 123°, 46%, 34%
```
Used for positive actions, confirmations, and availability indicators.

#### Rollback Red
```
Rollback Red: #DE1C24
RGB: 222, 28, 36
HSL: 357°, 80%, 49%
```
The iconic rollback color for price reductions and urgent promotions.

### Neutral Colors

#### Text Dark
```
Primary Text: #2E2F32
RGB: 46, 47, 50
HSL: 225°, 4%, 19%
```

#### Text Secondary
```
Secondary Text: #46474A
RGB: 70, 71, 74
HSL: 225°, 3%, 28%
```

#### Text Muted
```
Muted Text: #74767C
RGB: 116, 118, 124
HSL: 225°, 3%, 47%
```

#### Backgrounds
```
White: #FFFFFF
Light Gray: #F5F5F5
Card Gray: #F8F8F8
Border Gray: #E6E6E6
Divider: #CCCCCC
```

### Functional Colors

| Purpose | Color | Hex Code |
|---------|-------|----------|
| Primary Action | Walmart Blue | #0071DC |
| Savings/Value | Spark Yellow | #FFC220 |
| Rollback | Rollback Red | #DE1C24 |
| Success | Success Green | #2E7D32 |
| Warning | Orange | #F57C00 |
| Error | Error Red | #B00020 |
| Info | Info Blue | #0288D1 |
| Pickup Today | Green | #1E8900 |
| Delivery | Blue | #0071DC |

### Color Usage Guidelines

1. **Blue dominates** - Use Walmart Blue for primary CTAs, headers, and navigation
2. **Yellow accents** - Reserve Spark Yellow for the logo and special promotions
3. **Red for savings** - Rollback Red exclusively for price reductions
4. **Green for availability** - Use green to indicate in-stock, pickup ready, or success states
5. **Maintain contrast** - Ensure WCAG AA compliance (4.5:1 for text)

---

## 3. Typography

### Primary Typeface: Bogle

Bogle is Walmart's custom typeface, designed specifically for the brand. It's friendly, approachable, and highly legible across all platforms.

#### Bogle Font Family
```css
font-family: 'Bogle', 'Helvetica Neue', Helvetica, Arial, sans-serif;
```

#### Font Weights
| Weight | Value | Usage |
|--------|-------|-------|
| Regular | 400 | Body text, descriptions |
| Medium | 500 | Subheadings, emphasis |
| Bold | 700 | Headlines, prices, CTAs |
| Black | 900 | Hero headlines, major promotions |

### Type Scale

#### Display Headlines
```css
/* Hero Display */
font-size: 48px;
line-height: 56px;
font-weight: 900;
letter-spacing: -0.5px;

/* Display Large */
font-size: 40px;
line-height: 48px;
font-weight: 700;

/* Display Medium */
font-size: 32px;
line-height: 40px;
font-weight: 700;
```

#### Headlines
```css
/* H1 */
font-size: 28px;
line-height: 36px;
font-weight: 700;

/* H2 */
font-size: 24px;
line-height: 32px;
font-weight: 700;

/* H3 */
font-size: 20px;
line-height: 28px;
font-weight: 700;

/* H4 */
font-size: 18px;
line-height: 24px;
font-weight: 700;
```

#### Body Text
```css
/* Body Large */
font-size: 16px;
line-height: 24px;
font-weight: 400;

/* Body Regular */
font-size: 14px;
line-height: 20px;
font-weight: 400;

/* Body Small */
font-size: 12px;
line-height: 16px;
font-weight: 400;

/* Caption */
font-size: 11px;
line-height: 14px;
font-weight: 400;
```

### Price Typography

Prices are a critical element in Walmart's design and require special treatment:

```css
/* Large Price (Hero) */
.price-hero {
  font-size: 48px;
  font-weight: 700;
  color: #2E2F32;
}

.price-hero .cents {
  font-size: 24px;
  vertical-align: super;
}

/* Standard Price */
.price-standard {
  font-size: 24px;
  font-weight: 700;
  color: #2E2F32;
}

/* Rollback Price */
.price-rollback {
  font-size: 24px;
  font-weight: 700;
  color: #DE1C24;
}

/* Was Price (Strikethrough) */
.price-was {
  font-size: 14px;
  font-weight: 400;
  color: #74767C;
  text-decoration: line-through;
}
```

### Typography Best Practices

1. **Left-align** most text for optimal readability
2. **Bold prices** to make them instantly scannable
3. **Use sentence case** for most content (not ALL CAPS)
4. **Limit line length** to 60-80 characters for readability
5. **Maintain hierarchy** with consistent size jumps

---

## 4. Spacing & Layout

### Spacing Scale

Walmart uses an 8px base unit for consistent spacing:

| Token | Value | Usage |
|-------|-------|-------|
| spacing-0 | 0px | Reset |
| spacing-1 | 4px | Tight spacing, icon gaps |
| spacing-2 | 8px | Base unit, small gaps |
| spacing-3 | 12px | Compact padding |
| spacing-4 | 16px | Standard padding |
| spacing-5 | 24px | Section padding |
| spacing-6 | 32px | Large gaps |
| spacing-7 | 48px | Section breaks |
| spacing-8 | 64px | Major sections |
| spacing-9 | 96px | Page sections |

### Grid System

#### Desktop Grid (1280px+)
```css
.container {
  max-width: 1440px;
  padding: 0 64px;
  margin: 0 auto;
}

.grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 24px;
}
```

#### Tablet Grid (768px - 1279px)
```css
.container {
  padding: 0 32px;
}

.grid {
  grid-template-columns: repeat(8, 1fr);
  gap: 16px;
}
```

#### Mobile Grid (< 768px)
```css
.container {
  padding: 0 16px;
}

.grid {
  grid-template-columns: repeat(4, 1fr);
  gap: 12px;
}
```

### Product Grid Layouts

```css
/* Desktop: 4-5 products per row */
.product-grid-desktop {
  grid-template-columns: repeat(5, 1fr);
  gap: 16px;
}

/* Tablet: 3-4 products per row */
.product-grid-tablet {
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
}

/* Mobile: 2 products per row */
.product-grid-mobile {
  grid-template-columns: repeat(2, 1fr);
  gap: 8px;
}
```

### Breakpoints

| Breakpoint | Value | Device |
|------------|-------|--------|
| xs | 0-479px | Small phones |
| sm | 480-767px | Large phones |
| md | 768-1023px | Tablets |
| lg | 1024-1279px | Small desktop |
| xl | 1280-1439px | Desktop |
| xxl | 1440px+ | Large desktop |

---

## 5. Components

### Buttons

#### Primary Button
```css
.btn-primary {
  background-color: #0071DC;
  color: #FFFFFF;
  font-family: 'Bogle', sans-serif;
  font-size: 16px;
  font-weight: 700;
  padding: 12px 24px;
  border-radius: 24px;
  border: none;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

.btn-primary:hover {
  background-color: #004F9A;
}

.btn-primary:disabled {
  background-color: #CCCCCC;
  cursor: not-allowed;
}
```

#### Secondary Button
```css
.btn-secondary {
  background-color: transparent;
  color: #0071DC;
  font-weight: 700;
  padding: 12px 24px;
  border-radius: 24px;
  border: 2px solid #0071DC;
}

.btn-secondary:hover {
  background-color: #F0F8FF;
}
```

#### Add to Cart Button
```css
.btn-add-to-cart {
  background-color: #0071DC;
  color: #FFFFFF;
  font-weight: 700;
  padding: 12px 20px;
  border-radius: 24px;
  display: flex;
  align-items: center;
  gap: 8px;
}

.btn-add-to-cart .icon {
  width: 20px;
  height: 20px;
}
```

### Product Card

```css
.product-card {
  background: #FFFFFF;
  border-radius: 8px;
  padding: 16px;
  display: flex;
  flex-direction: column;
  gap: 12px;
  transition: box-shadow 0.2s ease;
}

.product-card:hover {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.product-card__image {
  aspect-ratio: 1;
  object-fit: contain;
  width: 100%;
}

.product-card__title {
  font-size: 14px;
  font-weight: 400;
  color: #2E2F32;
  line-height: 20px;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  overflow: hidden;
}

.product-card__price {
  font-size: 24px;
  font-weight: 700;
  color: #2E2F32;
}

.product-card__price .cents {
  font-size: 14px;
  vertical-align: super;
}
```

### Rollback Badge

```css
.rollback-badge {
  background-color: #DE1C24;
  color: #FFFFFF;
  font-size: 12px;
  font-weight: 700;
  padding: 4px 8px;
  border-radius: 4px;
  text-transform: uppercase;
  display: inline-flex;
  align-items: center;
  gap: 4px;
}

.rollback-badge::before {
  content: '';
  width: 16px;
  height: 16px;
  background: url('rollback-arrow.svg') no-repeat center;
}
```

### Fulfillment Options

```css
.fulfillment-options {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.fulfillment-option {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 12px;
  color: #46474A;
}

.fulfillment-option--pickup {
  color: #1E8900;
}

.fulfillment-option--delivery {
  color: #0071DC;
}

.fulfillment-option .icon {
  width: 16px;
  height: 16px;
}
```

### Search Bar

```css
.search-bar {
  display: flex;
  align-items: center;
  background: #FFFFFF;
  border-radius: 24px;
  padding: 8px 16px;
  width: 100%;
  max-width: 600px;
}

.search-bar__input {
  flex: 1;
  border: none;
  font-size: 16px;
  font-family: 'Bogle', sans-serif;
  outline: none;
}

.search-bar__button {
  background: #0071DC;
  border: none;
  border-radius: 50%;
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}
```

### Navigation Header

```css
.header {
  background: #0071DC;
  color: #FFFFFF;
  padding: 12px 0;
}

.header__top {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 24px;
}

.header__logo {
  height: 32px;
}

.header__nav {
  background: #004F9A;
  padding: 8px 0;
}

.header__nav-link {
  color: #FFFFFF;
  font-size: 14px;
  font-weight: 500;
  padding: 8px 16px;
  text-decoration: none;
}

.header__nav-link:hover {
  text-decoration: underline;
}
```

### Rating Stars

```css
.rating {
  display: flex;
  align-items: center;
  gap: 4px;
}

.rating__stars {
  display: flex;
  gap: 2px;
}

.rating__star {
  width: 16px;
  height: 16px;
  fill: #FFC220;
}

.rating__star--empty {
  fill: #E6E6E6;
}

.rating__count {
  font-size: 12px;
  color: #74767C;
}
```

---

## 6. Iconography

### Icon Style Guidelines

Walmart icons are simple, functional, and universally recognizable:

- **Style**: Outlined with 2px stroke weight
- **Size**: 24px standard, 16px small, 32px large
- **Color**: Inherit from parent or use functional colors
- **Corner radius**: 2px rounded corners

### Core Icons

| Icon | Usage | Size |
|------|-------|------|
| Spark | Logo element, rewards | 24-48px |
| Cart | Shopping cart | 24px |
| Search | Search functionality | 24px |
| Store | Store locator, pickup | 24px |
| Delivery | Delivery options | 24px |
| Heart | Favorites/wishlist | 24px |
| User | Account | 24px |
| Menu | Mobile navigation | 24px |
| Filter | Sort/filter options | 24px |
| Check | Success, selection | 20px |

### The Spark

The Walmart Spark is the most recognizable brand element:

```css
.spark {
  width: 48px;
  height: 48px;
}

.spark-yellow {
  fill: #FFC220;
}

/* Spark usage rules:
   - Always use official Spark asset
   - Maintain clear space equal to spark height
   - Never rotate or distort
   - Yellow Spark on blue or dark backgrounds
   - Blue Spark on white or light backgrounds
*/
```

### Icon Sizes

```css
/* Small Icons */
.icon-sm {
  width: 16px;
  height: 16px;
}

/* Standard Icons */
.icon-md {
  width: 24px;
  height: 24px;
}

/* Large Icons */
.icon-lg {
  width: 32px;
  height: 32px;
}

/* Extra Large (feature icons) */
.icon-xl {
  width: 48px;
  height: 48px;
}
```

---

## 7. Imagery & Media

### Photography Style

#### Product Photography
- **Clean white backgrounds** for primary product images
- **Consistent lighting** - soft, even illumination
- **Multiple angles** - front, back, detail shots
- **Scale reference** where appropriate
- **High resolution** - minimum 1000x1000px

#### Lifestyle Photography
- **Real people** in authentic settings
- **Diverse representation** across all demographics
- **Bright, optimistic lighting**
- **Natural, unposed moments**
- **Family and community focus**

### Image Specifications

| Type | Aspect Ratio | Min Resolution |
|------|--------------|----------------|
| Product (Square) | 1:1 | 1000x1000px |
| Product (Detail) | 1:1 | 1500x1500px |
| Hero Banner | 16:9 | 1920x1080px |
| Category Tile | 4:3 | 800x600px |
| Thumbnail | 1:1 | 200x200px |
| Mobile Banner | 2:1 | 750x375px |

### Image Treatment

```css
/* Product Image Container */
.product-image {
  background: #FFFFFF;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 16px;
}

.product-image img {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
}

/* Lazy Loading */
.product-image img {
  opacity: 0;
  transition: opacity 0.3s ease;
}

.product-image img.loaded {
  opacity: 1;
}
```

### Video Guidelines

- **Auto-play** product videos on hover (muted)
- **Captions** required for accessibility
- **Max length** 30 seconds for product demos
- **Mobile optimized** with vertical variants

---

## 8. Motion & Animation

### Animation Principles

1. **Purposeful** - Every animation should serve a function
2. **Fast** - Customers want efficiency, not entertainment
3. **Subtle** - Support the experience, don't distract
4. **Consistent** - Use standard timing across the platform

### Timing Tokens

```css
/* Duration */
--duration-instant: 100ms;
--duration-fast: 200ms;
--duration-normal: 300ms;
--duration-slow: 500ms;

/* Easing */
--ease-default: cubic-bezier(0.4, 0, 0.2, 1);
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
```

### Common Animations

#### Button Interactions
```css
.btn {
  transition: background-color 200ms var(--ease-default),
              transform 100ms var(--ease-default);
}

.btn:hover {
  transform: translateY(-1px);
}

.btn:active {
  transform: translateY(0);
}
```

#### Add to Cart Animation
```css
@keyframes addToCart {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.1);
  }
  100% {
    transform: scale(1);
  }
}

.btn-add-to-cart.added {
  animation: addToCart 300ms var(--ease-bounce);
}
```

#### Loading States
```css
@keyframes pulse {
  0%, 100% {
    opacity: 1;
  }
  50% {
    opacity: 0.5;
  }
}

.skeleton {
  background: linear-gradient(90deg, #F5F5F5 25%, #E6E6E6 50%, #F5F5F5 75%);
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite;
}

@keyframes shimmer {
  0% {
    background-position: 200% 0;
  }
  100% {
    background-position: -200% 0;
  }
}
```

#### Page Transitions
```css
.page-enter {
  opacity: 0;
  transform: translateY(8px);
}

.page-enter-active {
  opacity: 1;
  transform: translateY(0);
  transition: opacity 300ms var(--ease-out),
              transform 300ms var(--ease-out);
}
```

### Cart Badge Animation
```css
@keyframes cartBounce {
  0%, 100% {
    transform: scale(1);
  }
  25% {
    transform: scale(1.2);
  }
  50% {
    transform: scale(0.95);
  }
  75% {
    transform: scale(1.05);
  }
}

.cart-badge.updated {
  animation: cartBounce 400ms var(--ease-bounce);
}
```

---

## 9. Accessibility

### Accessibility Standards

Walmart is committed to WCAG 2.1 AA compliance across all digital properties.

### Color Contrast

| Text Type | Minimum Ratio | Walmart Implementation |
|-----------|---------------|----------------------|
| Normal Text | 4.5:1 | #2E2F32 on #FFFFFF = 13.9:1 |
| Large Text | 3:1 | #0071DC on #FFFFFF = 5.2:1 |
| UI Components | 3:1 | All interactive elements |

### Focus States

```css
/* Global Focus Style */
*:focus-visible {
  outline: 2px solid #0071DC;
  outline-offset: 2px;
}

/* Button Focus */
.btn:focus-visible {
  outline: 2px solid #FFFFFF;
  outline-offset: 2px;
  box-shadow: 0 0 0 4px #0071DC;
}

/* Link Focus */
a:focus-visible {
  outline: 2px solid #0071DC;
  outline-offset: 2px;
  border-radius: 2px;
}
```

### Keyboard Navigation

```css
/* Skip Link */
.skip-link {
  position: absolute;
  top: -100%;
  left: 16px;
  background: #0071DC;
  color: #FFFFFF;
  padding: 12px 24px;
  border-radius: 4px;
  z-index: 9999;
}

.skip-link:focus {
  top: 16px;
}
```

### Screen Reader Support

```html
<!-- Product Card Example -->
<article class="product-card" aria-label="Product: Great Value Milk">
  <img src="milk.jpg" alt="Great Value Whole Milk, 1 Gallon">
  
  <h3 class="product-card__title">
    Great Value Whole Milk, 1 Gallon
  </h3>
  
  <div class="product-card__price" aria-label="Price: $3.48">
    <span aria-hidden="true">$3</span>
    <span class="cents" aria-hidden="true">48</span>
  </div>
  
  <div class="rating" aria-label="4.5 out of 5 stars, 1,234 reviews">
    <div class="rating__stars" aria-hidden="true">
      <!-- Star icons -->
    </div>
    <span class="rating__count">(1,234)</span>
  </div>
  
  <button class="btn-add-to-cart" aria-label="Add Great Value Whole Milk to cart">
    <span aria-hidden="true">Add to cart</span>
  </button>
</article>
```

### Form Accessibility

```html
<!-- Accessible Form Field -->
<div class="form-field">
  <label for="email" class="form-label">
    Email Address
    <span class="required" aria-label="required">*</span>
  </label>
  <input 
    type="email" 
    id="email" 
    name="email"
    aria-required="true"
    aria-describedby="email-hint email-error"
    class="form-input"
  >
  <span id="email-hint" class="form-hint">
    We'll send your order confirmation here
  </span>
  <span id="email-error" class="form-error" role="alert">
    <!-- Error message appears here -->
  </span>
</div>
```

### Motion Preferences

```css
/* Respect reduced motion preferences */
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

### Touch Target Sizes

```css
/* Minimum touch target: 44x44px */
.touch-target {
  min-width: 44px;
  min-height: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* Button minimum size */
.btn {
  min-height: 44px;
  padding: 12px 24px;
}
```

### Accessibility Checklist

- [ ] All images have meaningful alt text
- [ ] Color is not the only means of conveying information
- [ ] Form fields have associated labels
- [ ] Error messages are announced to screen readers
- [ ] Focus order follows visual order
- [ ] Interactive elements are keyboard accessible
- [ ] Sufficient color contrast on all text
- [ ] ARIA labels on icon-only buttons
- [ ] Skip navigation link available
- [ ] Page titles are unique and descriptive

---

## Quick Reference

### Design Tokens Summary

```css
:root {
  /* Colors */
  --color-primary: #0071DC;
  --color-primary-dark: #004F9A;
  --color-secondary: #FFC220;
  --color-rollback: #DE1C24;
  --color-success: #1E8900;
  --color-text-primary: #2E2F32;
  --color-text-secondary: #46474A;
  --color-text-muted: #74767C;
  --color-background: #FFFFFF;
  --color-background-gray: #F5F5F5;
  --color-border: #E6E6E6;
  
  /* Typography */
  --font-family: 'Bogle', 'Helvetica Neue', Helvetica, Arial, sans-serif;
  --font-weight-regular: 400;
  --font-weight-medium: 500;
  --font-weight-bold: 700;
  --font-weight-black: 900;
  
  /* Spacing */
  --spacing-1: 4px;
  --spacing-2: 8px;
  --spacing-3: 12px;
  --spacing-4: 16px;
  --spacing-5: 24px;
  --spacing-6: 32px;
  --spacing-7: 48px;
  --spacing-8: 64px;
  
  /* Border Radius */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 16px;
  --radius-pill: 24px;
  --radius-full: 50%;
  
  /* Shadows */
  --shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.05);
  --shadow-md: 0 4px 8px rgba(0, 0, 0, 0.1);
  --shadow-lg: 0 8px 16px rgba(0, 0, 0, 0.15);
  
  /* Transitions */
  --transition-fast: 200ms cubic-bezier(0.4, 0, 0.2, 1);
  --transition-normal: 300ms cubic-bezier(0.4, 0, 0.2, 1);
}
```

---

*This design system documentation is based on Walmart's public-facing digital properties and brand guidelines. For internal use, refer to the official Walmart Design System documentation.*
