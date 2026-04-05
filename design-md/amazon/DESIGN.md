# Amazon Design System

## 1. Color Palette

### Primary Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Amazon Orange | `#FF9900` | rgb(255, 153, 0) | Primary brand color, buttons, accents, links on dark backgrounds |
| Amazon Dark Navy | `#131921` | rgb(19, 25, 33) | Primary header, footer background |
| Amazon Navy | `#232F3E` | rgb(35, 47, 62) | Secondary header, navigation panels |

### Background Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| White | `#FFFFFF` | rgb(255, 255, 255) | Primary page background, product cards |
| Light Gray | `#EAEDED` | rgb(234, 237, 237) | Page background, section dividers |
| Soft Gray | `#F3F3F3` | rgb(243, 243, 243) | Input fields, hover states |
| Card Background | `#FAFAFA` | rgb(250, 250, 250) | Product card backgrounds |

### Text Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Primary Text | `#0F1111` | rgb(15, 17, 17) | Main body text, headings |
| Secondary Text | `#565959` | rgb(86, 89, 89) | Subtext, descriptions |
| Muted Text | `#767676` | rgb(118, 118, 118) | Tertiary information |
| Link Blue | `#007185` | rgb(0, 113, 133) | Text links, interactive elements |
| Link Hover | `#C7511F` | rgb(199, 81, 31) | Link hover state |

### Status & Alert Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Success Green | `#067D62` | rgb(6, 125, 98) | In stock, success messages |
| Error Red | `#B12704` | rgb(177, 39, 4) | Errors, sale prices |
| Warning Orange | `#F0AD4E` | rgb(240, 173, 78) | Warnings, limited stock |
| Deal Red | `#CC0C39` | rgb(204, 12, 57) | Deal badges, lightning deals |

### Rating & Badge Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Star Gold | `#FFA41C` | rgb(255, 164, 28) | Star ratings filled |
| Star Empty | `#DDDDDD` | rgb(221, 221, 221) | Star ratings empty |
| Prime Blue | `#00A8E1` | rgb(0, 168, 225) | Prime badges, Prime-related elements |
| Prime Dark | `#146EB4` | rgb(20, 110, 180) | Prime text, secondary Prime elements |

### Button Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Button Yellow | `#FFD814` | rgb(255, 216, 20) | Add to Cart primary button |
| Button Yellow Hover | `#F7CA00` | rgb(247, 202, 0) | Add to Cart hover state |
| Button Orange | `#FFA41C` | rgb(255, 164, 28) | Buy Now button |
| Button Orange Hover | `#FA8900` | rgb(250, 137, 0) | Buy Now hover state |
| Button Gray | `#F0F2F2` | rgb(240, 242, 242) | Secondary buttons |
| Button Gray Hover | `#E3E6E6` | rgb(227, 230, 230) | Secondary button hover |

---

## 2. Typography

### Font Stack
```css
/* Primary Font */
font-family: "Amazon Ember", Arial, sans-serif;

/* Display Font */
font-family: "Amazon Ember Display", "Amazon Ember", Arial, sans-serif;

/* Monospace (for prices, codes) */
font-family: "Amazon Ember Mono", Consolas, monospace;
```

### Font Weights
| Weight Name | Value | Usage |
|-------------|-------|-------|
| Light | 300 | Large display text, subtle headings |
| Regular | 400 | Body text, descriptions |
| Medium | 500 | Subheadings, emphasis |
| Bold | 700 | Headings, prices, important text |

### Type Scale
| Element | Size | Weight | Line Height | Letter Spacing |
|---------|------|--------|-------------|----------------|
| Hero Title | 28px | 400 | 1.2 | -0.01em |
| Page Title | 24px | 400 | 1.25 | normal |
| Section Title | 21px | 700 | 1.25 | normal |
| Product Title | 18px | 400 | 1.35 | normal |
| Card Title | 16px | 400 | 1.4 | normal |
| Body Large | 14px | 400 | 1.45 | normal |
| Body | 13px | 400 | 1.45 | normal |
| Body Small | 12px | 400 | 1.5 | normal |
| Caption | 11px | 400 | 1.4 | normal |
| Price Large | 28px | 400 | 1.2 | -0.02em |
| Price Medium | 21px | 400 | 1.25 | -0.01em |
| Price Small | 14px | 400 | 1.3 | normal |

### Text Treatments
```css
/* Product Title */
.product-title {
  font-size: 16px;
  font-weight: 400;
  line-height: 1.4;
  color: #0F1111;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}

/* Price Display */
.price {
  font-size: 21px;
  font-weight: 400;
  color: #0F1111;
}

.price-symbol {
  font-size: 13px;
  vertical-align: top;
  position: relative;
  top: 2px;
}

.price-fraction {
  font-size: 13px;
  vertical-align: top;
}

/* Strikethrough Price */
.original-price {
  font-size: 14px;
  color: #565959;
  text-decoration: line-through;
}

/* Link Text */
.link {
  color: #007185;
  text-decoration: none;
}

.link:hover {
  color: #C7511F;
  text-decoration: underline;
}
```

---

## 3. Spacing System

### Base Unit
- Base spacing unit: **4px**

### Spacing Scale
| Token | Value | Usage |
|-------|-------|-------|
| `space-0` | 0px | Reset |
| `space-1` | 4px | Tight spacing, inline elements |
| `space-2` | 8px | Related elements, icon padding |
| `space-3` | 12px | Card internal padding |
| `space-4` | 16px | Section padding, card gaps |
| `space-5` | 20px | Standard container padding |
| `space-6` | 24px | Section gaps |
| `space-7` | 32px | Large section gaps |
| `space-8` | 40px | Major section separation |
| `space-9` | 48px | Page level spacing |
| `space-10` | 64px | Hero sections |

### Layout Spacing
```css
/* Container Padding */
.container {
  padding: 0 18px;
  max-width: 1500px;
  margin: 0 auto;
}

/* Product Grid Gap */
.product-grid {
  gap: 14px;
}

/* Card Internal Spacing */
.product-card {
  padding: 12px;
}

/* Section Spacing */
.section {
  padding: 20px 0;
  margin-bottom: 24px;
}

/* Dense List Spacing */
.dense-list-item {
  padding: 8px 12px;
}
```

### Responsive Spacing
| Breakpoint | Container Padding | Grid Gap |
|------------|-------------------|----------|
| Mobile (<768px) | 12px | 8px |
| Tablet (768-1024px) | 16px | 12px |
| Desktop (1024-1440px) | 18px | 14px |
| Wide (>1440px) | 24px | 16px |

---

## 4. Component Library

### Buttons

#### Primary Button (Add to Cart)
```css
.btn-primary {
  background: linear-gradient(to bottom, #f7dfa5, #f0c14b);
  border: 1px solid #a88734;
  border-radius: 8px;
  padding: 8px 18px;
  font-size: 13px;
  font-weight: 400;
  color: #0F1111;
  cursor: pointer;
  box-shadow: 0 2px 5px 0 rgba(213, 217, 217, 0.5);
}

.btn-primary:hover {
  background: linear-gradient(to bottom, #f5d78e, #eeb933);
}

.btn-primary:active {
  background: #f0c14b;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.2) inset;
}

/* Modern Yellow Button */
.btn-cart {
  background-color: #FFD814;
  border: 1px solid #FCD200;
  border-radius: 20px;
  padding: 10px 24px;
  font-size: 13px;
  color: #0F1111;
}

.btn-cart:hover {
  background-color: #F7CA00;
}
```

#### Buy Now Button
```css
.btn-buy-now {
  background-color: #FFA41C;
  border: 1px solid #FF8F00;
  border-radius: 20px;
  padding: 10px 24px;
  font-size: 13px;
  color: #0F1111;
}

.btn-buy-now:hover {
  background-color: #FA8900;
}
```

#### Secondary Button
```css
.btn-secondary {
  background-color: #FFFFFF;
  border: 1px solid #D5D9D9;
  border-radius: 8px;
  padding: 8px 18px;
  font-size: 13px;
  color: #0F1111;
  box-shadow: 0 2px 5px 0 rgba(213, 217, 217, 0.5);
}

.btn-secondary:hover {
  background-color: #F7FAFA;
}
```

### Product Card
```css
.product-card {
  background: #FFFFFF;
  border: 1px solid #DDD;
  border-radius: 8px;
  padding: 12px;
  position: relative;
  transition: box-shadow 0.2s ease;
}

.product-card:hover {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

.product-image {
  width: 100%;
  aspect-ratio: 1;
  object-fit: contain;
  margin-bottom: 8px;
}

.product-title {
  font-size: 14px;
  line-height: 1.4;
  color: #0F1111;
  margin-bottom: 4px;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.product-rating {
  display: flex;
  align-items: center;
  gap: 4px;
  margin-bottom: 4px;
}

.product-price {
  font-size: 21px;
  font-weight: 400;
  color: #0F1111;
}
```

### Star Rating
```css
.star-rating {
  display: inline-flex;
  gap: 1px;
}

.star {
  width: 15px;
  height: 15px;
  color: #FFA41C;
}

.star-empty {
  color: #DDDDDD;
}

.star-half {
  background: linear-gradient(90deg, #FFA41C 50%, #DDDDDD 50%);
  -webkit-background-clip: text;
}

.rating-count {
  color: #007185;
  font-size: 12px;
  margin-left: 4px;
}

.rating-count:hover {
  color: #C7511F;
  text-decoration: underline;
}
```

### Badges
```css
/* Prime Badge */
.badge-prime {
  display: inline-flex;
  align-items: center;
  gap: 4px;
}

.prime-logo {
  height: 16px;
  color: #00A8E1;
}

/* Deal Badge */
.badge-deal {
  background-color: #CC0C39;
  color: #FFFFFF;
  font-size: 12px;
  font-weight: 700;
  padding: 4px 8px;
  border-radius: 2px;
  text-transform: uppercase;
}

/* Limited Time Deal */
.badge-limited-deal {
  background-color: #CC0C39;
  color: #FFFFFF;
  font-size: 11px;
  padding: 3px 6px;
}

/* Best Seller Badge */
.badge-bestseller {
  background-color: #FF9900;
  color: #FFFFFF;
  font-size: 12px;
  font-weight: 700;
  padding: 4px 8px;
  border-radius: 2px;
}

/* Amazon's Choice Badge */
.badge-amazons-choice {
  background-color: #232F3E;
  color: #FFFFFF;
  font-size: 12px;
  padding: 4px 8px;
  border-radius: 2px;
}

.badge-amazons-choice::before {
  content: "";
  background-color: #FF9900;
  width: 4px;
  height: 100%;
  position: absolute;
  left: 0;
}

/* Discount Badge */
.badge-discount {
  background-color: #CC0C39;
  color: #FFFFFF;
  font-size: 12px;
  padding: 4px 6px;
  border-radius: 2px;
}
```

### Input Fields
```css
.input-field {
  width: 100%;
  padding: 8px 10px;
  border: 1px solid #A6A6A6;
  border-radius: 4px;
  font-size: 13px;
  color: #0F1111;
  background-color: #FFFFFF;
}

.input-field:focus {
  outline: none;
  border-color: #E77600;
  box-shadow: 0 0 0 3px rgba(228, 121, 17, 0.5);
}

.input-field::placeholder {
  color: #767676;
}

/* Search Input */
.search-input {
  border: none;
  border-radius: 0;
  padding: 10px 14px;
  font-size: 15px;
  flex: 1;
}
```

### Search Bar
```css
.search-bar {
  display: flex;
  align-items: stretch;
  border-radius: 4px;
  overflow: hidden;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.search-category {
  background-color: #F3F3F3;
  border: none;
  border-right: 1px solid #CDCDCD;
  padding: 8px 12px;
  font-size: 12px;
  color: #555;
  border-radius: 4px 0 0 4px;
}

.search-input {
  flex: 1;
  border: none;
  padding: 10px 14px;
  font-size: 15px;
}

.search-button {
  background-color: #FEBD69;
  border: none;
  padding: 8px 14px;
  cursor: pointer;
  border-radius: 0 4px 4px 0;
}

.search-button:hover {
  background-color: #F3A847;
}

.search-icon {
  width: 22px;
  height: 22px;
  color: #131921;
}
```

### Quantity Selector
```css
.quantity-selector {
  display: inline-flex;
  align-items: center;
  border: 1px solid #D5D9D9;
  border-radius: 8px;
  overflow: hidden;
  background: #F0F2F2;
}

.qty-btn {
  width: 36px;
  height: 36px;
  border: none;
  background: transparent;
  font-size: 18px;
  color: #0F1111;
  cursor: pointer;
}

.qty-btn:hover {
  background: #E3E6E6;
}

.qty-value {
  width: 44px;
  text-align: center;
  font-size: 14px;
  background: #FFFFFF;
  border-left: 1px solid #D5D9D9;
  border-right: 1px solid #D5D9D9;
  padding: 8px 0;
}
```

---

## 5. Layout System

### Grid System
```css
/* Product Grid - Dense Layout */
.product-grid {
  display: grid;
  gap: 14px;
}

/* Responsive Grid Columns */
@media (min-width: 1500px) {
  .product-grid { grid-template-columns: repeat(6, 1fr); }
}

@media (min-width: 1200px) and (max-width: 1499px) {
  .product-grid { grid-template-columns: repeat(5, 1fr); }
}

@media (min-width: 992px) and (max-width: 1199px) {
  .product-grid { grid-template-columns: repeat(4, 1fr); }
}

@media (min-width: 768px) and (max-width: 991px) {
  .product-grid { grid-template-columns: repeat(3, 1fr); }
}

@media (min-width: 480px) and (max-width: 767px) {
  .product-grid { grid-template-columns: repeat(2, 1fr); }
}

@media (max-width: 479px) {
  .product-grid { grid-template-columns: 1fr; }
}
```

### Container Widths
| Breakpoint | Max Width | Padding |
|------------|-----------|---------|
| Default | 100% | 12px |
| Small (576px+) | 540px | 16px |
| Medium (768px+) | 720px | 18px |
| Large (992px+) | 960px | 18px |
| X-Large (1200px+) | 1140px | 18px |
| XX-Large (1400px+) | 1500px | 24px |

### Page Layout Structure
```css
/* Main Layout */
.page-layout {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.main-content {
  flex: 1;
  max-width: 1500px;
  margin: 0 auto;
  padding: 14px 18px;
  width: 100%;
}

/* Two Column Layout (Search Results) */
.search-layout {
  display: grid;
  grid-template-columns: 245px 1fr;
  gap: 20px;
}

/* Sidebar Filters */
.sidebar-filters {
  width: 245px;
  flex-shrink: 0;
}

/* Three Column Layout (Product Page) */
.product-page-layout {
  display: grid;
  grid-template-columns: 450px 1fr 300px;
  gap: 24px;
}
```

### Header Structure
```css
/* Primary Header */
.header-primary {
  background-color: #131921;
  padding: 10px 18px;
  display: flex;
  align-items: center;
  gap: 16px;
}

/* Secondary Navigation */
.header-secondary {
  background-color: #232F3E;
  padding: 8px 18px;
}

.nav-links {
  display: flex;
  gap: 16px;
  font-size: 14px;
  color: #FFFFFF;
}
```

### Carousel/Slider Layout
```css
.carousel-container {
  position: relative;
  overflow: hidden;
}

.carousel-track {
  display: flex;
  gap: 14px;
  transition: transform 0.3s ease;
}

.carousel-item {
  flex: 0 0 auto;
  width: calc(16.666% - 12px); /* 6 items */
}

.carousel-arrow {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  width: 40px;
  height: 80px;
  background: rgba(255, 255, 255, 0.9);
  border: 1px solid #DDD;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  z-index: 10;
}

.carousel-arrow-left { left: 0; }
.carousel-arrow-right { right: 0; }
```

---

## 6. Iconography

### Icon Sizes
| Size | Dimensions | Usage |
|------|------------|-------|
| xs | 12px | Inline text icons, ratings |
| sm | 16px | Navigation, badges |
| md | 20px | Buttons, actions |
| lg | 24px | Headers, primary actions |
| xl | 32px | Feature icons |
| 2xl | 48px | Empty states, illustrations |

### Icon Style Guidelines
- **Stroke width**: 1.5px for outlined icons
- **Corner radius**: 2px on icon paths
- **Color**: Inherit from parent or specified
- **Alignment**: Center-aligned within bounds

### Common Icons
```css
/* Icon Base Styles */
.icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}

.icon-sm { width: 16px; height: 16px; }
.icon-md { width: 20px; height: 20px; }
.icon-lg { width: 24px; height: 24px; }

/* Icon Colors */
.icon-default { color: #0F1111; }
.icon-muted { color: #565959; }
.icon-link { color: #007185; }
.icon-white { color: #FFFFFF; }
.icon-orange { color: #FF9900; }
.icon-prime { color: #00A8E1; }
```

### Essential Icon Set
| Icon | Usage | Context |
|------|-------|---------|
| Search | Search bar, navigation | Header |
| Cart | Shopping cart | Header, product pages |
| User | Account, sign in | Header |
| Location | Delivery address | Header, checkout |
| Star | Ratings | Product cards, reviews |
| Star-half | Half ratings | Product cards |
| Heart | Wishlist, save | Product actions |
| Share | Share product | Product pages |
| Compare | Compare products | Search results |
| Filter | Filter results | Search sidebar |
| Sort | Sort options | Search results |
| Grid | Grid view | View toggle |
| List | List view | View toggle |
| Checkmark | Prime, verified | Badges, confirmation |
| Truck | Delivery | Shipping info |
| Return | Free returns | Product info |
| Lock | Secure checkout | Checkout |
| Arrow-down | Dropdowns | Navigation, selects |
| Arrow-right | Navigation, links | Carousels, breadcrumbs |
| Close | Close modal | Modals, notifications |
| Menu | Mobile menu | Mobile header |
| Plus | Add quantity | Quantity selector |
| Minus | Remove quantity | Quantity selector |

---

## 7. Motion & Animation

### Timing Functions
```css
/* Easing Curves */
--ease-default: cubic-bezier(0.4, 0, 0.2, 1);
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-bounce: cubic-bezier(0.34, 1.56, 0.64, 1);
```

### Duration Scale
| Token | Duration | Usage |
|-------|----------|-------|
| `instant` | 0ms | Immediate feedback |
| `fast` | 100ms | Micro-interactions, hovers |
| `normal` | 200ms | Standard transitions |
| `slow` | 300ms | Modal, drawer animations |
| `slower` | 400ms | Complex animations |

### Standard Animations
```css
/* Hover Lift */
.hover-lift {
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.hover-lift:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

/* Fade In */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

.fade-in {
  animation: fadeIn 0.2s ease forwards;
}

/* Slide Down (Dropdowns) */
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

.slide-down {
  animation: slideDown 0.2s ease forwards;
}

/* Skeleton Loading */
@keyframes shimmer {
  0% { background-position: -200% 0; }
  100% { background-position: 200% 0; }
}

.skeleton {
  background: linear-gradient(
    90deg,
    #F3F3F3 25%,
    #E8E8E8 50%,
    #F3F3F3 75%
  );
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite;
}

/* Add to Cart Animation */
@keyframes addToCart {
  0% { transform: scale(1); }
  50% { transform: scale(0.95); }
  100% { transform: scale(1); }
}

.add-to-cart-animation {
  animation: addToCart 0.2s ease;
}

/* Cart Count Badge */
@keyframes cartBounce {
  0%, 100% { transform: scale(1); }
  50% { transform: scale(1.2); }
}

.cart-badge-update {
  animation: cartBounce 0.3s ease;
}
```

### Loading States
```css
/* Spinner */
@keyframes spin {
  to { transform: rotate(360deg); }
}

.spinner {
  width: 24px;
  height: 24px;
  border: 3px solid #EAEDED;
  border-top-color: #FF9900;
  border-radius: 50%;
  animation: spin 0.8s linear infinite;
}

/* Progress Bar */
.progress-bar {
  height: 4px;
  background-color: #EAEDED;
  border-radius: 2px;
  overflow: hidden;
}

.progress-fill {
  height: 100%;
  background-color: #FF9900;
  transition: width 0.3s ease;
}
```

---

## 8. Responsive Breakpoints

### Breakpoint Definitions
| Name | Min Width | Max Width | Target |
|------|-----------|-----------|--------|
| xs | 0 | 479px | Small phones |
| sm | 480px | 767px | Large phones |
| md | 768px | 991px | Tablets |
| lg | 992px | 1199px | Small laptops |
| xl | 1200px | 1499px | Desktops |
| xxl | 1500px | - | Large desktops |

### Media Query Mixins
```css
/* Mobile First Approach */
/* Base styles for mobile */

/* Small devices and up */
@media (min-width: 480px) { }

/* Medium devices and up */
@media (min-width: 768px) { }

/* Large devices and up */
@media (min-width: 992px) { }

/* Extra large devices and up */
@media (min-width: 1200px) { }

/* Extra extra large devices */
@media (min-width: 1500px) { }
```

### Responsive Component Behavior

#### Header
| Breakpoint | Behavior |
|------------|----------|
| xs-sm | Hamburger menu, simplified search, stacked layout |
| md | Full navigation visible, search expands |
| lg+ | Full header with all elements, account dropdown |

#### Product Grid
| Breakpoint | Columns | Card Style |
|------------|---------|------------|
| xs | 1 | Full width, horizontal layout |
| sm | 2 | Vertical cards |
| md | 3 | Vertical cards |
| lg | 4 | Vertical cards |
| xl | 5 | Vertical cards |
| xxl | 6 | Vertical cards, compact |

#### Navigation
| Breakpoint | Behavior |
|------------|----------|
| xs-md | Slide-out drawer, hamburger trigger |
| lg+ | Horizontal mega-menu on hover |

### Responsive Typography
```css
/* Responsive Font Sizes */
.heading-responsive {
  font-size: 18px;
}

@media (min-width: 768px) {
  .heading-responsive { font-size: 21px; }
}

@media (min-width: 1200px) {
  .heading-responsive { font-size: 24px; }
}

/* Price Responsive */
.price-responsive {
  font-size: 16px;
}

@media (min-width: 768px) {
  .price-responsive { font-size: 18px; }
}

@media (min-width: 1200px) {
  .price-responsive { font-size: 21px; }
}
```

---

## 9. Accessibility & States

### Focus States
```css
/* Default Focus Ring */
:focus-visible {
  outline: 2px solid #E77600;
  outline-offset: 2px;
}

/* Button Focus */
.btn:focus-visible {
  outline: 2px solid #E77600;
  outline-offset: 2px;
  box-shadow: 0 0 0 4px rgba(228, 121, 17, 0.3);
}

/* Link Focus */
a:focus-visible {
  outline: 2px solid #007185;
  outline-offset: 2px;
  border-radius: 2px;
}

/* Input Focus */
.input-field:focus {
  outline: none;
  border-color: #E77600;
  box-shadow: 0 0 0 3px rgba(228, 121, 17, 0.5);
}

/* Card Focus */
.product-card:focus-within {
  outline: 2px solid #E77600;
  outline-offset: 2px;
}
```

### Interactive States
```css
/* Button States */
.btn {
  /* Default */
  background-color: #FFD814;
  cursor: pointer;
}

.btn:hover {
  background-color: #F7CA00;
}

.btn:active {
  background-color: #F0C14B;
  transform: scale(0.98);
}

.btn:disabled {
  background-color: #E7E9EC;
  color: #8D9096;
  cursor: not-allowed;
  opacity: 0.6;
}

/* Link States */
.link {
  color: #007185;
  text-decoration: none;
}

.link:hover {
  color: #C7511F;
  text-decoration: underline;
}

.link:visited {
  color: #0066C0;
}

.link:active {
  color: #C7511F;
}
```

### Color Contrast Requirements
| Element | Foreground | Background | Ratio |
|---------|------------|------------|-------|
| Body Text | #0F1111 | #FFFFFF | 18.1:1 |
| Secondary Text | #565959 | #FFFFFF | 7.0:1 |
| Links | #007185 | #FFFFFF | 5.0:1 |
| Primary Button | #0F1111 | #FFD814 | 10.4:1 |
| Header Text | #FFFFFF | #131921 | 16.8:1 |

### ARIA Labels
```html
<!-- Star Rating -->
<div role="img" aria-label="4.5 out of 5 stars" class="star-rating">
  <!-- stars -->
</div>

<!-- Add to Cart Button -->
<button aria-label="Add Product Name to cart">
  Add to Cart
</button>

<!-- Quantity Selector -->
<div role="group" aria-label="Quantity selector">
  <button aria-label="Decrease quantity">-</button>
  <input type="number" aria-label="Quantity" value="1">
  <button aria-label="Increase quantity">+</button>
</div>

<!-- Prime Badge -->
<span role="img" aria-label="Prime eligible">
  <img src="prime-logo.svg" alt="">
</span>

<!-- Navigation -->
<nav aria-label="Product categories">
  <!-- nav items -->
</nav>

<!-- Search -->
<form role="search" aria-label="Search Amazon">
  <input type="search" aria-label="Search products">
  <button type="submit" aria-label="Submit search">
    Search
  </button>
</form>
```

### Keyboard Navigation
```css
/* Skip Link */
.skip-link {
  position: absolute;
  top: -40px;
  left: 0;
  background: #000;
  color: #FFF;
  padding: 8px 16px;
  z-index: 100;
}

.skip-link:focus {
  top: 0;
}

/* Tab Order Indicators */
[tabindex]:focus-visible {
  outline: 2px solid #E77600;
  outline-offset: 2px;
}
```

### Screen Reader Support
```css
/* Visually Hidden (for screen readers) */
.sr-only {
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

/* Live Regions */
[aria-live="polite"] {
  /* Announces changes at next convenient moment */
}

[aria-live="assertive"] {
  /* Announces changes immediately */
}
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
    scroll-behavior: auto !important;
  }
}
```

### Form Validation States
```css
/* Error State */
.input-error {
  border-color: #B12704;
  box-shadow: 0 0 0 3px rgba(177, 39, 4, 0.2);
}

.error-message {
  color: #B12704;
  font-size: 12px;
  margin-top: 4px;
  display: flex;
  align-items: center;
  gap: 4px;
}

/* Success State */
.input-success {
  border-color: #067D62;
}

.success-message {
  color: #067D62;
  font-size: 12px;
  margin-top: 4px;
}

/* Warning State */
.input-warning {
  border-color: #F0AD4E;
  background-color: #FFF9E6;
}
```

---

## E-Commerce Specific Patterns

### Price Display Patterns
```css
/* Standard Price */
.price-block {
  display: flex;
  align-items: baseline;
  gap: 8px;
}

.current-price {
  font-size: 28px;
  color: #0F1111;
}

.current-price .symbol {
  font-size: 14px;
  vertical-align: top;
}

.current-price .fraction {
  font-size: 14px;
  vertical-align: top;
}

/* Deal Price */
.deal-price {
  color: #B12704;
}

.original-price {
  font-size: 14px;
  color: #565959;
  text-decoration: line-through;
}

.savings {
  color: #B12704;
  font-size: 14px;
}
```

### Shipping Information
```css
.shipping-info {
  font-size: 14px;
  color: #0F1111;
}

.free-shipping {
  color: #067D62;
  font-weight: 700;
}

.delivery-date {
  font-weight: 700;
}

.delivery-fastest {
  color: #067D62;
}
```

### Buy Box Pattern
```css
.buy-box {
  border: 1px solid #DDD;
  border-radius: 8px;
  padding: 16px;
  background: #FFFFFF;
}

.buy-box-price {
  font-size: 28px;
  margin-bottom: 8px;
}

.buy-box-shipping {
  font-size: 14px;
  margin-bottom: 12px;
}

.buy-box-stock {
  color: #067D62;
  font-size: 18px;
  margin-bottom: 16px;
}

.buy-box-buttons {
  display: flex;
  flex-direction: column;
  gap: 8px;
}
```

### Filter Sidebar Pattern
```css
.filter-section {
  border-bottom: 1px solid #EAEDED;
  padding: 12px 0;
}

.filter-title {
  font-size: 14px;
  font-weight: 700;
  color: #0F1111;
  margin-bottom: 8px;
}

.filter-option {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 4px 0;
  font-size: 14px;
  color: #0F1111;
  cursor: pointer;
}

.filter-checkbox {
  width: 18px;
  height: 18px;
  accent-color: #FF9900;
}
```

### Cart Item Pattern
```css
.cart-item {
  display: grid;
  grid-template-columns: 180px 1fr auto;
  gap: 16px;
  padding: 16px 0;
  border-bottom: 1px solid #EAEDED;
}

.cart-item-image {
  width: 180px;
  height: 180px;
  object-fit: contain;
}

.cart-item-details {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.cart-item-actions {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 13px;
}

.cart-item-action-link {
  color: #007185;
  cursor: pointer;
  padding: 0 8px;
  border-right: 1px solid #DDD;
}

.cart-item-action-link:last-child {
  border-right: none;
}
```

### Checkout Progress
```css
.checkout-progress {
  display: flex;
  justify-content: center;
  gap: 0;
  margin-bottom: 24px;
}

.progress-step {
  display: flex;
  align-items: center;
  font-size: 13px;
  color: #565959;
}

.progress-step.active {
  color: #C7511F;
  font-weight: 700;
}

.progress-step.completed {
  color: #067D62;
}

.progress-divider {
  width: 40px;
  height: 2px;
  background: #EAEDED;
  margin: 0 16px;
}

.progress-divider.completed {
  background: #067D62;
}
```
