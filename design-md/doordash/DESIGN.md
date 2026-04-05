# DoorDash Design System

## 1. Color Palette

### Primary Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| DoorDash Red | `#FF3008` | rgb(255, 48, 8) | Primary brand, CTAs, logo |
| DoorDash Red Dark | `#C41E00` | rgb(196, 30, 0) | Hover states, emphasis |
| DoorDash Red Light | `#FF6B4D` | rgb(255, 107, 77) | Accent highlights |

### Secondary Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| DashPass Purple | `#5C2D91` | rgb(92, 45, 145) | DashPass membership branding |
| DashPass Purple Light | `#7B4CB8` | rgb(123, 76, 184) | DashPass accents |
| Success Green | `#00A651` | rgb(0, 166, 81) | Delivery confirmations, savings |
| Alert Yellow | `#FFBE00` | rgb(255, 190, 0) | Warnings, attention |
| Star Gold | `#FFCC00` | rgb(255, 204, 0) | Rating stars |

### Neutral Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Black | `#191919` | rgb(25, 25, 25) | Primary text |
| Gray 900 | `#2E2E2E` | rgb(46, 46, 46) | Headings |
| Gray 700 | `#494949` | rgb(73, 73, 73) | Secondary text |
| Gray 500 | `#767676` | rgb(118, 118, 118) | Placeholder text |
| Gray 300 | `#B8B8B8` | rgb(184, 184, 184) | Disabled states |
| Gray 200 | `#E8E8E8` | rgb(232, 232, 232) | Borders, dividers |
| Gray 100 | `#F5F5F5` | rgb(245, 245, 245) | Background secondary |
| White | `#FFFFFF` | rgb(255, 255, 255) | Primary background |

### Delivery Status Colors
| Color Name | Hex Code | Usage |
|------------|----------|-------|
| Preparing | `#FF9500` | Order being prepared |
| On The Way | `#007AFF` | Dasher en route |
| Arriving | `#34C759` | Dasher nearby |
| Delivered | `#00A651` | Order complete |

---

## 2. Typography

### Font Family
```css
/* Primary Font */
font-family: 'DD-TTNorms', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;

/* Numeric Display (Prices, Times) */
font-family: 'DD-TTNorms', 'SF Pro Display', -apple-system, sans-serif;
```

### Type Scale
| Style | Size | Weight | Line Height | Letter Spacing | Usage |
|-------|------|--------|-------------|----------------|-------|
| Display XL | 48px | 800 | 1.1 | -0.02em | Hero promotions |
| Display Large | 36px | 700 | 1.2 | -0.01em | Page titles |
| Heading 1 | 28px | 700 | 1.25 | -0.01em | Section headers |
| Heading 2 | 24px | 700 | 1.3 | 0 | Restaurant names |
| Heading 3 | 20px | 600 | 1.35 | 0 | Category titles |
| Heading 4 | 18px | 600 | 1.4 | 0 | Dish names |
| Body Large | 16px | 400 | 1.5 | 0 | Primary content |
| Body | 14px | 400 | 1.5 | 0 | Descriptions |
| Body Small | 13px | 400 | 1.45 | 0 | Metadata |
| Caption | 12px | 500 | 1.4 | 0.01em | Labels, times |
| Micro | 11px | 500 | 1.3 | 0.02em | Badges |

### Font Weights
| Weight Name | Value | Usage |
|-------------|-------|-------|
| Regular | 400 | Body text, descriptions |
| Medium | 500 | Labels, metadata |
| Semibold | 600 | Subheadings, emphasis |
| Bold | 700 | Headings, restaurant names |
| Extrabold | 800 | Promotional displays |

### Typography Tokens
```css
/* Restaurant Card */
.restaurant-name {
  font-size: 16px;
  font-weight: 700;
  color: #191919;
  line-height: 1.3;
}

.restaurant-meta {
  font-size: 13px;
  font-weight: 400;
  color: #767676;
}

/* Dish Item */
.dish-name {
  font-size: 15px;
  font-weight: 600;
  color: #191919;
}

.dish-description {
  font-size: 13px;
  font-weight: 400;
  color: #767676;
  line-height: 1.4;
}

/* Price Display */
.price {
  font-size: 14px;
  font-weight: 600;
  color: #191919;
}

.price-strikethrough {
  font-size: 13px;
  font-weight: 400;
  color: #767676;
  text-decoration: line-through;
}
```

---

## 3. Spacing System

### Base Unit
```css
--spacing-unit: 4px;
```

### Spacing Scale
| Token | Value | Usage |
|-------|-------|-------|
| `--space-0` | 0px | Reset |
| `--space-1` | 4px | Tight spacing |
| `--space-2` | 8px | Icon gaps |
| `--space-3` | 12px | Small gaps |
| `--space-4` | 16px | Component padding |
| `--space-5` | 20px | Card padding |
| `--space-6` | 24px | Section spacing |
| `--space-8` | 32px | Large gaps |
| `--space-10` | 40px | Section margins |
| `--space-12` | 48px | Page sections |
| `--space-16` | 64px | Hero spacing |

### Component Spacing
```css
/* Restaurant Card */
.restaurant-card {
  padding: 0;
  margin-bottom: 24px;
}

.restaurant-card-content {
  padding: 12px 0;
}

/* Menu Item */
.menu-item {
  padding: 16px;
  gap: 12px;
}

/* Cart Item */
.cart-item {
  padding: 16px;
  border-bottom: 1px solid #E8E8E8;
}

/* Category Section */
.menu-category {
  padding: 24px 0 16px;
}
```

### Grid System
```css
/* Restaurant Grid */
.restaurant-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 24px;
  padding: 0 16px;
}

/* Cuisine Category Scroll */
.cuisine-scroll {
  display: flex;
  gap: 12px;
  padding: 16px;
  overflow-x: auto;
}

/* Menu Layout */
.menu-layout {
  display: grid;
  grid-template-columns: 1fr 380px;
  gap: 24px;
}
```

---

## 4. Border Radius

### Radius Scale
| Token | Value | Usage |
|-------|-------|-------|
| `--radius-none` | 0px | Sharp edges |
| `--radius-xs` | 4px | Small chips |
| `--radius-sm` | 8px | Buttons, inputs |
| `--radius-md` | 12px | Cards |
| `--radius-lg` | 16px | Restaurant images |
| `--radius-xl` | 20px | Modal corners |
| `--radius-2xl` | 24px | Bottom sheets |
| `--radius-full` | 9999px | Pills, badges |

### Component Radius
```css
/* Restaurant Card Image */
.restaurant-image {
  border-radius: 16px;
}

/* Food Item Image */
.food-image {
  border-radius: 8px;
}

/* Buttons */
.btn-primary {
  border-radius: 24px;
}

.btn-secondary {
  border-radius: 8px;
}

/* Search Bar */
.search-bar {
  border-radius: 8px;
}

/* Category Chips */
.category-chip {
  border-radius: 20px;
}

/* Cart Badge */
.cart-badge {
  border-radius: 50%;
}

/* DashPass Banner */
.dashpass-banner {
  border-radius: 12px;
}
```

---

## 5. Shadow System

### Shadow Scale
| Token | Value | Usage |
|-------|-------|-------|
| `--shadow-none` | none | Flat elements |
| `--shadow-sm` | 0 1px 2px rgba(0,0,0,0.06) | Subtle lift |
| `--shadow-md` | 0 2px 8px rgba(0,0,0,0.08) | Cards |
| `--shadow-lg` | 0 4px 16px rgba(0,0,0,0.1) | Floating cart |
| `--shadow-xl` | 0 8px 32px rgba(0,0,0,0.12) | Modals |
| `--shadow-2xl` | 0 16px 48px rgba(0,0,0,0.16) | Bottom sheets |

### Component Shadows
```css
/* Restaurant Card Hover */
.restaurant-card:hover {
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.1);
  transform: translateY(-2px);
}

/* Floating Cart Button */
.floating-cart {
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
}

/* Header Shadow */
.header-shadow {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
}

/* Modal */
.modal {
  box-shadow: 0 16px 48px rgba(0, 0, 0, 0.2);
}

/* Search Dropdown */
.search-dropdown {
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.15);
}

/* Sticky Category Nav */
.sticky-nav {
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
}
```

---

## 6. Component Specifications

### Restaurant Card
```css
.restaurant-card {
  display: flex;
  flex-direction: column;
  background: #FFFFFF;
  border-radius: 16px;
  overflow: hidden;
  cursor: pointer;
  transition: all 0.2s ease;
}

.restaurant-card-image {
  position: relative;
  width: 100%;
  aspect-ratio: 16 / 10;
  border-radius: 16px;
  overflow: hidden;
}

.restaurant-card-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* Delivery Time Badge */
.delivery-time-badge {
  position: absolute;
  bottom: 8px;
  left: 8px;
  background: #FFFFFF;
  padding: 4px 8px;
  border-radius: 4px;
  font-size: 13px;
  font-weight: 600;
  color: #191919;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

/* Promotion Badge */
.promo-badge {
  position: absolute;
  top: 8px;
  left: 8px;
  background: #00A651;
  color: #FFFFFF;
  padding: 4px 8px;
  border-radius: 4px;
  font-size: 12px;
  font-weight: 600;
}

.restaurant-card-info {
  padding: 12px 0;
}

.restaurant-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 4px;
}

.restaurant-name {
  font-size: 16px;
  font-weight: 700;
  color: #191919;
}

.restaurant-rating {
  display: flex;
  align-items: center;
  gap: 4px;
  font-size: 13px;
  font-weight: 600;
  color: #191919;
  background: #F5F5F5;
  padding: 2px 6px;
  border-radius: 4px;
}

.restaurant-meta {
  font-size: 13px;
  color: #767676;
}
```

### Rating Stars
```css
.rating-stars {
  display: flex;
  align-items: center;
  gap: 2px;
}

.star {
  width: 14px;
  height: 14px;
}

.star-filled {
  color: #FFCC00;
}

.star-empty {
  color: #E8E8E8;
}

.rating-value {
  font-size: 13px;
  font-weight: 600;
  color: #191919;
  margin-left: 4px;
}

.rating-count {
  font-size: 12px;
  color: #767676;
}
```

### Menu Item
```css
.menu-item {
  display: flex;
  gap: 12px;
  padding: 16px;
  border-bottom: 1px solid #E8E8E8;
  cursor: pointer;
  transition: background 0.15s ease;
}

.menu-item:hover {
  background: #F5F5F5;
}

.menu-item-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 4px;
}

.menu-item-name {
  font-size: 15px;
  font-weight: 600;
  color: #191919;
}

.menu-item-description {
  font-size: 13px;
  color: #767676;
  line-height: 1.4;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.menu-item-price {
  font-size: 14px;
  font-weight: 600;
  color: #191919;
  margin-top: auto;
}

.menu-item-image {
  width: 120px;
  height: 120px;
  border-radius: 8px;
  object-fit: cover;
  flex-shrink: 0;
}

/* Popular Badge */
.popular-badge {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  background: #FFF5F2;
  color: #FF3008;
  padding: 2px 8px;
  border-radius: 4px;
  font-size: 11px;
  font-weight: 600;
  margin-bottom: 4px;
}
```

### DashPass Badge
```css
.dashpass-badge {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  background: linear-gradient(135deg, #5C2D91 0%, #7B4CB8 100%);
  color: #FFFFFF;
  padding: 4px 8px;
  border-radius: 4px;
  font-size: 11px;
  font-weight: 600;
}

.dashpass-icon {
  width: 12px;
  height: 12px;
}

/* DashPass Banner */
.dashpass-banner {
  background: linear-gradient(135deg, #5C2D91 0%, #7B4CB8 100%);
  color: #FFFFFF;
  padding: 16px;
  border-radius: 12px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.dashpass-banner-title {
  font-size: 18px;
  font-weight: 700;
}

.dashpass-banner-subtitle {
  font-size: 13px;
  opacity: 0.9;
}

.dashpass-banner-cta {
  background: #FFFFFF;
  color: #5C2D91;
  padding: 8px 16px;
  border-radius: 20px;
  font-size: 13px;
  font-weight: 600;
}
```

### Primary Button
```css
.btn-primary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: #FF3008;
  color: #FFFFFF;
  padding: 14px 24px;
  border-radius: 24px;
  font-size: 15px;
  font-weight: 600;
  border: none;
  cursor: pointer;
  transition: all 0.15s ease;
}

.btn-primary:hover {
  background: #C41E00;
  transform: scale(1.02);
}

.btn-primary:active {
  transform: scale(0.98);
}

.btn-primary:disabled {
  background: #B8B8B8;
  cursor: not-allowed;
}

/* Add to Cart Button */
.btn-add-cart {
  width: 100%;
  padding: 16px;
  font-size: 16px;
}
```

### Cart/Checkout Button
```css
.cart-button {
  position: fixed;
  bottom: 24px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: #FF3008;
  color: #FFFFFF;
  padding: 12px 20px;
  border-radius: 30px;
  min-width: 340px;
  box-shadow: 0 4px 20px rgba(255, 48, 8, 0.35);
  cursor: pointer;
  transition: all 0.2s ease;
}

.cart-button:hover {
  transform: translateX(-50%) scale(1.02);
  box-shadow: 0 6px 24px rgba(255, 48, 8, 0.4);
}

.cart-button-left {
  display: flex;
  align-items: center;
  gap: 8px;
}

.cart-item-count {
  background: rgba(255, 255, 255, 0.2);
  padding: 4px 10px;
  border-radius: 16px;
  font-size: 13px;
  font-weight: 600;
}

.cart-button-text {
  font-size: 15px;
  font-weight: 600;
}

.cart-total {
  font-size: 15px;
  font-weight: 700;
}
```

### Search Bar
```css
.search-bar {
  display: flex;
  align-items: center;
  gap: 12px;
  background: #F5F5F5;
  padding: 12px 16px;
  border-radius: 8px;
  border: 2px solid transparent;
  transition: all 0.15s ease;
}

.search-bar:focus-within {
  background: #FFFFFF;
  border-color: #FF3008;
  box-shadow: 0 0 0 3px rgba(255, 48, 8, 0.1);
}

.search-icon {
  color: #767676;
  width: 20px;
  height: 20px;
  flex-shrink: 0;
}

.search-input {
  flex: 1;
  border: none;
  background: transparent;
  font-size: 15px;
  color: #191919;
  outline: none;
}

.search-input::placeholder {
  color: #767676;
}
```

### Category Chips
```css
.category-chips {
  display: flex;
  gap: 8px;
  padding: 16px;
  overflow-x: auto;
  scrollbar-width: none;
}

.category-chip {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
  padding: 12px 16px;
  background: #F5F5F5;
  border-radius: 12px;
  cursor: pointer;
  transition: all 0.15s ease;
  flex-shrink: 0;
}

.category-chip:hover {
  background: #E8E8E8;
}

.category-chip.active {
  background: #FFF5F2;
  border: 2px solid #FF3008;
}

.category-chip-icon {
  font-size: 24px;
}

.category-chip-label {
  font-size: 12px;
  font-weight: 500;
  color: #191919;
  white-space: nowrap;
}
```

### Quantity Selector
```css
.quantity-selector {
  display: flex;
  align-items: center;
  gap: 16px;
  background: #F5F5F5;
  padding: 4px;
  border-radius: 24px;
}

.qty-btn {
  width: 36px;
  height: 36px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #FFFFFF;
  border-radius: 50%;
  border: none;
  cursor: pointer;
  font-size: 18px;
  color: #191919;
  transition: all 0.15s ease;
}

.qty-btn:hover {
  background: #FF3008;
  color: #FFFFFF;
}

.qty-btn:disabled {
  background: #E8E8E8;
  color: #B8B8B8;
  cursor: not-allowed;
}

.qty-value {
  font-size: 16px;
  font-weight: 600;
  min-width: 24px;
  text-align: center;
}
```

### Delivery Progress
```css
.delivery-progress {
  background: #FFFFFF;
  border-radius: 16px;
  padding: 20px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
}

.progress-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 16px;
}

.progress-eta {
  font-size: 28px;
  font-weight: 700;
  color: #191919;
}

.progress-status {
  font-size: 14px;
  color: #767676;
}

.progress-track {
  height: 4px;
  background: #E8E8E8;
  border-radius: 2px;
  overflow: hidden;
}

.progress-fill {
  height: 100%;
  background: linear-gradient(90deg, #FF3008 0%, #FF6B4D 100%);
  border-radius: 2px;
  transition: width 0.3s ease;
}

.progress-steps {
  display: flex;
  justify-content: space-between;
  margin-top: 12px;
}

.progress-step {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
}

.step-dot {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: #E8E8E8;
}

.step-dot.completed {
  background: #FF3008;
}

.step-dot.active {
  background: #FF3008;
  box-shadow: 0 0 0 4px rgba(255, 48, 8, 0.2);
}

.step-label {
  font-size: 11px;
  color: #767676;
}
```

---

## 7. Iconography

### Icon Specifications
| Property | Value |
|----------|-------|
| Default Size | 24px |
| Small Size | 16px |
| Large Size | 32px |
| Stroke Width | 1.5px - 2px |
| Style | Rounded, friendly |
| Color | Inherit from parent |

### Core Icons
```
Navigation:
- home (house)
- search (magnifying glass)
- browse (grid)
- orders (receipt)
- account (person)

Food Categories:
- restaurant (storefront)
- grocery (shopping bag)
- alcohol (wine glass)
- convenience (clock)
- pets (paw)
- flowers (flower)

Actions:
- cart (shopping cart)
- add (plus circle)
- remove (minus circle)
- favorite (heart)
- share (share arrow)
- filter (sliders)
- sort (arrows up/down)

Delivery:
- delivery (motorcycle/car)
- pickup (walking person)
- schedule (calendar)
- location (map pin)
- time (clock)
- dasher (delivery person)

Rating:
- star-filled
- star-half
- star-empty
- thumbs-up
- thumbs-down

Order:
- order-placed (checkmark)
- preparing (cooking pot)
- on-the-way (road)
- delivered (package check)
```

### Icon Usage
```css
/* Navigation Icons */
.nav-icon {
  width: 24px;
  height: 24px;
  color: #767676;
}

.nav-icon.active {
  color: #FF3008;
}

/* Action Icons */
.action-icon {
  width: 20px;
  height: 20px;
  color: #494949;
}

/* Category Icons */
.category-icon {
  width: 32px;
  height: 32px;
  color: #191919;
}

/* Rating Star */
.star-icon {
  width: 14px;
  height: 14px;
}

.star-icon.filled {
  color: #FFCC00;
}
```

---

## 8. Animation Guidelines

### Timing Functions
```css
/* Standard Easing */
--ease-default: cubic-bezier(0.4, 0, 0.2, 1);
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-spring: cubic-bezier(0.175, 0.885, 0.32, 1.275);
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
```

### Duration Scale
| Token | Duration | Usage |
|-------|----------|-------|
| `--duration-instant` | 100ms | Micro-interactions |
| `--duration-fast` | 150ms | Buttons, hovers |
| `--duration-normal` | 200ms | Most transitions |
| `--duration-slow` | 300ms | Page transitions |
| `--duration-slower` | 400ms | Complex animations |

### Component Animations
```css
/* Restaurant Card Hover */
.restaurant-card {
  transition: transform 0.2s var(--ease-default),
              box-shadow 0.2s var(--ease-default);
}

.restaurant-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
}

/* Button Press */
.btn-primary:active {
  transform: scale(0.96);
  transition: transform 0.1s var(--ease-out);
}

/* Add to Cart Animation */
@keyframes addToCart {
  0% { transform: scale(1); }
  50% { transform: scale(0.9); }
  100% { transform: scale(1); }
}

.adding-to-cart {
  animation: addToCart 0.3s var(--ease-spring);
}

/* Cart Button Bounce */
@keyframes cartBounce {
  0%, 100% { transform: translateX(-50%) scale(1); }
  50% { transform: translateX(-50%) scale(1.05); }
}

.cart-updated {
  animation: cartBounce 0.3s var(--ease-spring);
}

/* Loading Skeleton */
@keyframes shimmer {
  0% { background-position: -200% 0; }
  100% { background-position: 200% 0; }
}

.skeleton {
  background: linear-gradient(
    90deg,
    #F5F5F5 25%,
    #E8E8E8 50%,
    #F5F5F5 75%
  );
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite;
}

/* Delivery Tracker Pulse */
@keyframes deliveryPulse {
  0%, 100% { 
    box-shadow: 0 0 0 0 rgba(255, 48, 8, 0.4);
  }
  50% { 
    box-shadow: 0 0 0 8px rgba(255, 48, 8, 0);
  }
}

.dasher-marker {
  animation: deliveryPulse 2s infinite;
}

/* Modal Entry */
@keyframes modalEntry {
  from {
    opacity: 0;
    transform: translateY(20px) scale(0.95);
  }
  to {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}

.modal {
  animation: modalEntry 0.3s var(--ease-out);
}

/* Bottom Sheet */
@keyframes bottomSheetUp {
  from { transform: translateY(100%); }
  to { transform: translateY(0); }
}

.bottom-sheet {
  animation: bottomSheetUp 0.35s var(--ease-out);
}
```

### Page Transitions
```css
/* Page Fade */
.page-enter {
  opacity: 0;
}

.page-enter-active {
  opacity: 1;
  transition: opacity 0.25s var(--ease-out);
}

.page-exit {
  opacity: 1;
}

.page-exit-active {
  opacity: 0;
  transition: opacity 0.2s var(--ease-in);
}
```

---

## 9. Responsive Breakpoints

### Breakpoint Scale
| Name | Width | Description |
|------|-------|-------------|
| `xs` | 0-479px | Small phones |
| `sm` | 480-767px | Large phones |
| `md` | 768-1023px | Tablets |
| `lg` | 1024-1279px | Small desktop |
| `xl` | 1280-1439px | Desktop |
| `2xl` | 1440px+ | Large desktop |

### Media Queries
```css
/* Mobile First Approach */
@media (min-width: 480px) { /* sm */ }
@media (min-width: 768px) { /* md */ }
@media (min-width: 1024px) { /* lg */ }
@media (min-width: 1280px) { /* xl */ }
@media (min-width: 1440px) { /* 2xl */ }
```

### Responsive Layout
```css
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

/* Restaurant Grid */
.restaurant-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 16px;
}

@media (min-width: 480px) {
  .restaurant-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 768px) {
  .restaurant-grid {
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
  }
}

@media (min-width: 1280px) {
  .restaurant-grid {
    grid-template-columns: repeat(4, 1fr);
    gap: 24px;
  }
}

/* Store Page Layout */
.store-layout {
  display: flex;
  flex-direction: column;
}

@media (min-width: 1024px) {
  .store-layout {
    display: grid;
    grid-template-columns: 1fr 380px;
    gap: 24px;
  }
}

/* Cart Sidebar */
.cart-sidebar {
  display: none;
}

@media (min-width: 1024px) {
  .cart-sidebar {
    display: block;
    position: sticky;
    top: 80px;
    height: fit-content;
    max-height: calc(100vh - 100px);
    overflow-y: auto;
  }
}

/* Mobile Cart Button */
.mobile-cart-button {
  display: flex;
}

@media (min-width: 1024px) {
  .mobile-cart-button {
    display: none;
  }
}

/* Navigation */
.mobile-nav {
  display: flex;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  background: #FFFFFF;
  border-top: 1px solid #E8E8E8;
  padding: 8px 0 env(safe-area-inset-bottom);
}

@media (min-width: 768px) {
  .mobile-nav {
    display: none;
  }
}

.desktop-nav {
  display: none;
}

@media (min-width: 768px) {
  .desktop-nav {
    display: flex;
  }
}

/* Menu Item Image */
.menu-item-image {
  width: 100px;
  height: 100px;
}

@media (min-width: 768px) {
  .menu-item-image {
    width: 120px;
    height: 120px;
  }
}

/* Category Scroll vs Grid */
.categories-scroll {
  display: flex;
  overflow-x: auto;
}

@media (min-width: 768px) {
  .categories-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
    overflow: visible;
  }
}

/* Typography Scaling */
.heading-xl {
  font-size: 28px;
}

@media (min-width: 768px) {
  .heading-xl {
    font-size: 36px;
  }
}

@media (min-width: 1024px) {
  .heading-xl {
    font-size: 48px;
  }
}
```

### Touch Targets
```css
/* Ensure minimum touch target size on mobile */
@media (max-width: 767px) {
  .btn,
  .nav-link,
  .category-chip {
    min-height: 44px;
    min-width: 44px;
  }
}
```

---

## Design Tokens Summary

```css
:root {
  /* Colors */
  --color-primary: #FF3008;
  --color-primary-dark: #C41E00;
  --color-primary-light: #FF6B4D;
  --color-dashpass: #5C2D91;
  --color-success: #00A651;
  --color-warning: #FFBE00;
  --color-star: #FFCC00;
  
  --color-text-primary: #191919;
  --color-text-secondary: #767676;
  --color-text-disabled: #B8B8B8;
  
  --color-bg-primary: #FFFFFF;
  --color-bg-secondary: #F5F5F5;
  --color-border: #E8E8E8;
  
  /* Typography */
  --font-family: 'DD-TTNorms', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  
  /* Spacing */
  --space-unit: 4px;
  --space-xs: 4px;
  --space-sm: 8px;
  --space-md: 16px;
  --space-lg: 24px;
  --space-xl: 32px;
  --space-2xl: 48px;
  
  /* Border Radius */
  --radius-sm: 8px;
  --radius-md: 12px;
  --radius-lg: 16px;
  --radius-full: 9999px;
  
  /* Shadows */
  --shadow-sm: 0 1px 2px rgba(0,0,0,0.06);
  --shadow-md: 0 2px 8px rgba(0,0,0,0.08);
  --shadow-lg: 0 4px 16px rgba(0,0,0,0.1);
  --shadow-xl: 0 8px 32px rgba(0,0,0,0.12);
  
  /* Animation */
  --ease-default: cubic-bezier(0.4, 0, 0.2, 1);
  --ease-spring: cubic-bezier(0.175, 0.885, 0.32, 1.275);
  --duration-fast: 150ms;
  --duration-normal: 200ms;
  --duration-slow: 300ms;
  
  /* Breakpoints (for reference) */
  --breakpoint-sm: 480px;
  --breakpoint-md: 768px;
  --breakpoint-lg: 1024px;
  --breakpoint-xl: 1280px;
  --breakpoint-2xl: 1440px;
}
```

---

*DoorDash Design System - Food delivery focused with emphasis on appetite appeal, delivery time prominence, and seamless ordering experience.*
