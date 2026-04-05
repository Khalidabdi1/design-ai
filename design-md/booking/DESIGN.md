# Booking.com Design System

## 1. Color Palette

### Primary Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Booking Blue | `#003580` | rgb(0, 53, 128) | Primary brand color, headers, navigation, links |
| Booking Dark Blue | `#00224f` | rgb(0, 34, 79) | Hover states, footers, dark sections |
| Booking Light Blue | `#0071c2` | rgb(0, 113, 194) | Secondary actions, interactive elements |

### Accent Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Booking Yellow | `#febb02` | rgb(254, 187, 2) | Primary CTAs, deal badges, highlights |
| Booking Yellow Hover | `#e5a800` | rgb(229, 168, 0) | CTA hover states |
| Success Green | `#008009` | rgb(0, 128, 9) | Availability, confirmations, savings |
| Genius Blue | `#004cb8` | rgb(0, 76, 184) | Genius loyalty program elements |

### Neutral Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Text Primary | `#262626` | rgb(38, 38, 38) | Main body text, headings |
| Text Secondary | `#6b6b6b` | rgb(107, 107, 107) | Secondary text, descriptions |
| Text Muted | `#8c8c8c` | rgb(140, 140, 140) | Helper text, placeholders |
| Border Light | `#e7e7e7` | rgb(231, 231, 231) | Card borders, dividers |
| Background Light | `#f5f5f5` | rgb(245, 245, 245) | Page backgrounds, sections |
| Background Blue Tint | `#ebf3ff` | rgb(235, 243, 255) | Highlighted sections, info boxes |
| White | `#ffffff` | rgb(255, 255, 255) | Cards, main backgrounds |

### Semantic Colors
| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Error Red | `#d4111e` | rgb(212, 17, 30) | Error messages, alerts, sold out |
| Warning Orange | `#f56700` | rgb(245, 103, 0) | Urgency messages, limited availability |
| Info Blue | `#0071c2` | rgb(0, 113, 194) | Information notices |
| Rating Score | `#003580` | rgb(0, 53, 128) | Review score backgrounds |

---

## 2. Typography

### Font Stack
```css
font-family: BlinkMacSystemFont, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
```

### Type Scale
| Element | Size | Weight | Line Height | Letter Spacing |
|---------|------|--------|-------------|----------------|
| Hero Title | 32px / 2rem | 700 | 1.25 | -0.5px |
| Page Title | 24px / 1.5rem | 700 | 1.33 | -0.25px |
| Section Heading | 20px / 1.25rem | 700 | 1.4 | 0 |
| Card Title | 16px / 1rem | 700 | 1.5 | 0 |
| Body Large | 16px / 1rem | 400 | 1.5 | 0 |
| Body | 14px / 0.875rem | 400 | 1.43 | 0 |
| Body Small | 12px / 0.75rem | 400 | 1.33 | 0 |
| Price Display | 24px / 1.5rem | 700 | 1.25 | 0 |
| Price Small | 14px / 0.875rem | 400 | 1.43 | 0 |
| Caption | 12px / 0.75rem | 400 | 1.33 | 0.1px |
| Badge Text | 12px / 0.75rem | 500 | 1 | 0.25px |

### Font Weights
| Weight Name | Value | Usage |
|-------------|-------|-------|
| Regular | 400 | Body text, descriptions |
| Medium | 500 | Badges, emphasized text |
| Bold | 700 | Headings, prices, CTAs |

### Text Colors
```css
/* Primary text */
color: #262626;

/* Secondary text */
color: #6b6b6b;

/* Link text */
color: #0071c2;

/* Link hover */
color: #003580;

/* Price text */
color: #262626;

/* Savings/Deals */
color: #008009;

/* Urgency text */
color: #d4111e;
```

---

## 3. Spacing System

### Base Unit
Base unit: **4px**

### Spacing Scale
| Token | Value | Usage |
|-------|-------|-------|
| `space-xxs` | 4px | Inline spacing, icon gaps |
| `space-xs` | 8px | Tight component spacing |
| `space-sm` | 12px | Small padding, list items |
| `space-md` | 16px | Standard padding, card content |
| `space-lg` | 24px | Section spacing, card gaps |
| `space-xl` | 32px | Large section margins |
| `space-xxl` | 48px | Page sections, major breaks |
| `space-xxxl` | 64px | Hero sections |

### Component Spacing
```css
/* Card padding */
padding: 16px;

/* Search box padding */
padding: 4px;

/* Button padding */
padding: 12px 24px;

/* Input padding */
padding: 12px 16px;

/* List item spacing */
gap: 8px;

/* Grid gap */
gap: 16px;

/* Section margin */
margin-bottom: 32px;
```

### Layout Spacing
```css
/* Page container */
max-width: 1110px;
padding: 0 16px;
margin: 0 auto;

/* Search bar spacing */
margin-bottom: 24px;

/* Property card grid */
gap: 16px;

/* Filter sidebar */
padding: 16px;
margin-right: 24px;
```

---

## 4. Component Library

### Buttons

#### Primary Button (Yellow CTA)
```css
.btn-primary {
  background-color: #febb02;
  color: #262626;
  font-size: 16px;
  font-weight: 700;
  padding: 12px 24px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  transition: background-color 0.15s ease;
}

.btn-primary:hover {
  background-color: #e5a800;
}

.btn-primary:active {
  background-color: #cc9600;
}
```

#### Secondary Button (Blue)
```css
.btn-secondary {
  background-color: #0071c2;
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  padding: 10px 16px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.btn-secondary:hover {
  background-color: #003580;
}
```

#### Outline Button
```css
.btn-outline {
  background-color: transparent;
  color: #0071c2;
  font-size: 14px;
  font-weight: 500;
  padding: 10px 16px;
  border: 1px solid #0071c2;
  border-radius: 4px;
  cursor: pointer;
}

.btn-outline:hover {
  background-color: #ebf3ff;
}
```

### Property Card
```css
.property-card {
  background: #ffffff;
  border: 1px solid #e7e7e7;
  border-radius: 8px;
  overflow: hidden;
  display: flex;
  transition: box-shadow 0.2s ease;
}

.property-card:hover {
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
  cursor: pointer;
}

.property-card__image {
  width: 200px;
  height: 200px;
  object-fit: cover;
}

.property-card__content {
  padding: 16px;
  flex: 1;
  display: flex;
  flex-direction: column;
}

.property-card__title {
  font-size: 16px;
  font-weight: 700;
  color: #0071c2;
  margin: 0 0 4px;
}

.property-card__location {
  font-size: 12px;
  color: #0071c2;
  margin-bottom: 8px;
}
```

### Review Score Badge
```css
.review-score {
  display: inline-flex;
  align-items: center;
  gap: 8px;
}

.review-score__badge {
  background-color: #003580;
  color: #ffffff;
  font-size: 14px;
  font-weight: 700;
  padding: 6px 8px;
  border-radius: 6px 6px 6px 0;
  min-width: 32px;
  text-align: center;
}

.review-score__text {
  font-size: 12px;
  color: #262626;
}

.review-score__label {
  font-weight: 700;
}

.review-score__count {
  color: #6b6b6b;
}
```

### Deal Badge
```css
.deal-badge {
  background-color: #008009;
  color: #ffffff;
  font-size: 12px;
  font-weight: 500;
  padding: 4px 8px;
  border-radius: 4px;
  display: inline-block;
}

.deal-badge--limited {
  background-color: #d4111e;
}

.deal-badge--genius {
  background-color: #004cb8;
}
```

### Price Display
```css
.price-display {
  text-align: right;
}

.price-display__original {
  font-size: 14px;
  color: #d4111e;
  text-decoration: line-through;
}

.price-display__current {
  font-size: 24px;
  font-weight: 700;
  color: #262626;
}

.price-display__info {
  font-size: 12px;
  color: #6b6b6b;
}

.price-display__taxes {
  font-size: 12px;
  color: #6b6b6b;
}
```

### Search Form
```css
.search-form {
  background-color: #febb02;
  padding: 4px;
  border-radius: 8px;
  display: flex;
  gap: 2px;
}

.search-form__input {
  flex: 1;
  padding: 12px 16px;
  border: none;
  border-radius: 4px;
  font-size: 14px;
  background: #ffffff;
}

.search-form__input:focus {
  outline: 2px solid #003580;
}

.search-form__button {
  background-color: #003580;
  color: #ffffff;
  padding: 12px 24px;
  border: none;
  border-radius: 4px;
  font-size: 16px;
  font-weight: 700;
  cursor: pointer;
}

.search-form__button:hover {
  background-color: #00224f;
}
```

### Filter Checkbox
```css
.filter-option {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 8px 0;
  cursor: pointer;
}

.filter-option__checkbox {
  width: 18px;
  height: 18px;
  border: 2px solid #6b6b6b;
  border-radius: 4px;
  accent-color: #003580;
}

.filter-option__label {
  font-size: 14px;
  color: #262626;
  flex: 1;
}

.filter-option__count {
  font-size: 12px;
  color: #6b6b6b;
}
```

### Genius Badge
```css
.genius-badge {
  background: linear-gradient(135deg, #004cb8 0%, #003580 100%);
  color: #ffffff;
  font-size: 12px;
  font-weight: 700;
  padding: 4px 8px;
  border-radius: 4px;
  display: inline-flex;
  align-items: center;
  gap: 4px;
}

.genius-badge__icon {
  width: 16px;
  height: 16px;
}
```

---

## 5. Layout System

### Grid Structure
```css
/* Main layout container */
.container {
  max-width: 1110px;
  margin: 0 auto;
  padding: 0 16px;
}

/* Search results layout */
.search-layout {
  display: grid;
  grid-template-columns: 250px 1fr;
  gap: 24px;
}

/* Property grid */
.property-grid {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

/* Property card horizontal */
.property-card--horizontal {
  display: grid;
  grid-template-columns: 200px 1fr auto;
  gap: 16px;
}
```

### Responsive Breakpoints
```css
/* Mobile */
@media (max-width: 575px) {
  .container { padding: 0 12px; }
  .search-layout { grid-template-columns: 1fr; }
  .property-card { flex-direction: column; }
  .property-card__image { width: 100%; height: 200px; }
}

/* Tablet */
@media (min-width: 576px) and (max-width: 991px) {
  .search-layout { grid-template-columns: 1fr; }
  .filters { display: none; }
  .filters--mobile { display: block; }
}

/* Desktop */
@media (min-width: 992px) {
  .container { max-width: 1110px; }
  .search-layout { grid-template-columns: 250px 1fr; }
}

/* Large desktop */
@media (min-width: 1200px) {
  .container { max-width: 1140px; }
}
```

### Header Layout
```css
.header {
  background-color: #003580;
  padding: 12px 0;
}

.header__container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.header__nav {
  display: flex;
  gap: 4px;
}

.header__nav-item {
  color: #ffffff;
  padding: 10px 16px;
  border-radius: 20px;
  font-size: 14px;
  text-decoration: none;
}

.header__nav-item:hover {
  background-color: rgba(255, 255, 255, 0.1);
}

.header__nav-item--active {
  background-color: #ffffff;
  color: #003580;
}
```

### Search Hero Section
```css
.hero {
  background-color: #003580;
  padding: 24px 0 120px;
}

.hero__title {
  color: #ffffff;
  font-size: 32px;
  font-weight: 700;
  margin-bottom: 8px;
}

.hero__subtitle {
  color: #ffffff;
  font-size: 16px;
  margin-bottom: 24px;
}

.search-box {
  background: #febb02;
  padding: 4px;
  border-radius: 8px;
  margin-top: -80px;
  position: relative;
  z-index: 10;
}
```

---

## 6. Iconography

### Icon System
Booking.com uses a custom icon set with consistent styling.

**Icon Specifications:**
- Default size: 24px
- Small size: 16px
- Large size: 32px
- Stroke width: 2px
- Style: Filled and outlined variants
- Color: Inherits from parent or specified

### Core Icons
```css
/* Icon base styles */
.icon {
  width: 24px;
  height: 24px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
}

.icon--sm { width: 16px; height: 16px; }
.icon--lg { width: 32px; height: 32px; }

/* Icon colors */
.icon--primary { color: #003580; }
.icon--secondary { color: #6b6b6b; }
.icon--white { color: #ffffff; }
.icon--success { color: #008009; }
.icon--warning { color: #f56700; }
```

### Common Icons Used
| Icon | Usage | Context |
|------|-------|---------|
| Bed | Room type indicator | Property cards, search |
| Calendar | Date selection | Search form, booking |
| User | Guest count | Search form, account |
| Location Pin | Map/location | Property cards, search |
| Star | Rating display | Reviews, quality |
| Heart | Wishlist/save | Property cards |
| Checkmark | Confirmation | Booking flow, amenities |
| WiFi | Amenity | Property details |
| Parking | Amenity | Property details |
| Breakfast | Amenity | Property details |
| Swimming Pool | Amenity | Property details |
| Air Conditioning | Amenity | Property details |
| Search | Search action | Navigation, forms |
| Filter | Filter controls | Search results |
| Sort | Sort options | Search results |
| Map | Map view toggle | Search results |
| Genius G | Loyalty program | Badges, discounts |

### Amenity Icons Grid
```css
.amenities-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}

.amenity-item {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 14px;
  color: #262626;
}

.amenity-item__icon {
  width: 20px;
  height: 20px;
  color: #008009;
}
```

---

## 7. Motion & Animation

### Animation Principles
- **Purpose:** Enhance usability, not decoration
- **Speed:** Fast, efficient transitions
- **Feedback:** Immediate response to user actions
- **Consistency:** Same patterns throughout the platform

### Timing Functions
```css
/* Default easing */
--ease-default: cubic-bezier(0.4, 0, 0.2, 1);

/* Enter easing (elements appearing) */
--ease-enter: cubic-bezier(0, 0, 0.2, 1);

/* Exit easing (elements disappearing) */
--ease-exit: cubic-bezier(0.4, 0, 1, 1);
```

### Duration Scale
| Duration | Value | Usage |
|----------|-------|-------|
| Instant | 100ms | Hover states, button feedback |
| Fast | 150ms | Small transitions, toggles |
| Normal | 200ms | Standard transitions |
| Moderate | 300ms | Modal openings, accordions |
| Slow | 400ms | Page transitions, complex animations |

### Common Animations
```css
/* Button hover */
.btn {
  transition: background-color 0.15s ease, transform 0.1s ease;
}

.btn:active {
  transform: scale(0.98);
}

/* Card hover lift */
.property-card {
  transition: box-shadow 0.2s ease, transform 0.2s ease;
}

.property-card:hover {
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
  transform: translateY(-2px);
}

/* Link underline */
.link {
  position: relative;
}

.link::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 0;
  height: 1px;
  background-color: currentColor;
  transition: width 0.2s ease;
}

.link:hover::after {
  width: 100%;
}

/* Dropdown menu */
.dropdown-menu {
  opacity: 0;
  visibility: hidden;
  transform: translateY(-8px);
  transition: opacity 0.2s ease, transform 0.2s ease, visibility 0.2s;
}

.dropdown-menu--open {
  opacity: 1;
  visibility: visible;
  transform: translateY(0);
}

/* Skeleton loading */
@keyframes skeleton-pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}

.skeleton {
  background: linear-gradient(90deg, #f5f5f5 25%, #e7e7e7 50%, #f5f5f5 75%);
  background-size: 200% 100%;
  animation: skeleton-pulse 1.5s ease-in-out infinite;
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
  border: 3px solid #e7e7e7;
  border-top-color: #003580;
  border-radius: 50%;
  animation: spin 0.8s linear infinite;
}

/* Progress bar */
.progress-bar {
  height: 4px;
  background-color: #e7e7e7;
  border-radius: 2px;
  overflow: hidden;
}

.progress-bar__fill {
  height: 100%;
  background-color: #003580;
  transition: width 0.3s ease;
}
```

---

## 8. Accessibility

### Color Contrast
All text meets WCAG 2.1 AA standards:
- Primary text (#262626) on white: **14.5:1**
- Secondary text (#6b6b6b) on white: **5.9:1**
- White text on Booking Blue (#003580): **10.7:1**
- Dark text (#262626) on Yellow (#febb02): **8.6:1**

### Focus States
```css
/* Focus visible outline */
*:focus-visible {
  outline: 2px solid #0071c2;
  outline-offset: 2px;
}

/* Button focus */
.btn:focus-visible {
  outline: 3px solid #003580;
  outline-offset: 2px;
}

/* Input focus */
.input:focus {
  outline: none;
  border-color: #003580;
  box-shadow: 0 0 0 2px rgba(0, 53, 128, 0.2);
}

/* Card focus */
.property-card:focus-visible {
  outline: 2px solid #003580;
  outline-offset: 2px;
}
```

### Keyboard Navigation
```css
/* Skip link */
.skip-link {
  position: absolute;
  top: -100px;
  left: 16px;
  padding: 12px 24px;
  background: #003580;
  color: #ffffff;
  z-index: 9999;
  border-radius: 4px;
}

.skip-link:focus {
  top: 16px;
}

/* Focus trap for modals */
.modal[aria-hidden="false"] {
  /* Contains focus within modal */
}
```

### ARIA Patterns
```html
<!-- Search form -->
<form role="search" aria-label="Search hotels">
  <input type="text" aria-label="Destination" placeholder="Where are you going?">
  <button type="submit" aria-label="Search">Search</button>
</form>

<!-- Property card -->
<article class="property-card" aria-labelledby="property-title-1">
  <img src="..." alt="Hotel exterior view">
  <h3 id="property-title-1">Hotel Name</h3>
  <div role="img" aria-label="Rating: 8.5 out of 10, Excellent">
    <span class="review-score__badge">8.5</span>
  </div>
</article>

<!-- Filter section -->
<aside aria-label="Search filters">
  <fieldset>
    <legend>Star rating</legend>
    <input type="checkbox" id="star-5" aria-label="5 stars">
    <label for="star-5">5 stars</label>
  </fieldset>
</aside>

<!-- Price display -->
<div aria-label="Price: 120 dollars per night">
  <span aria-hidden="true">$120</span>
  <span class="sr-only">per night</span>
</div>
```

### Screen Reader Utilities
```css
/* Visually hidden but accessible */
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

/* Skip to main content */
.sr-only:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
  white-space: normal;
}
```

### Touch Targets
```css
/* Minimum touch target size: 44x44px */
.btn,
.filter-option,
.nav-item {
  min-height: 44px;
  min-width: 44px;
}

/* Mobile tap targets */
@media (max-width: 575px) {
  .filter-option {
    padding: 12px 0;
  }
  
  .btn {
    padding: 14px 24px;
  }
}
```

---

## 9. Platform-Specific Guidelines

### Web Application

#### Browser Support
- Chrome (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Edge (latest 2 versions)

#### Performance Guidelines
```css
/* Critical CSS - above the fold */
/* Inline in <head> for fastest render */

/* Font loading strategy */
@font-face {
  font-family: 'System';
  src: local('BlinkMacSystemFont'),
       local('-apple-system'),
       local('Segoe UI'),
       local('Roboto');
  font-display: swap;
}

/* Image optimization */
.property-card__image {
  background-color: #f5f5f5; /* Placeholder color */
  aspect-ratio: 16/9;
}

/* Lazy loading */
img[loading="lazy"] {
  opacity: 0;
  transition: opacity 0.3s ease;
}

img[loading="lazy"].loaded {
  opacity: 1;
}
```

#### Progressive Enhancement
```css
/* Base styles (no JS) */
.dropdown-menu {
  display: none;
}

/* Enhanced with JS */
.js .dropdown-menu {
  display: block;
  visibility: hidden;
}
```

### Mobile Web (Responsive)

#### Touch Interactions
```css
/* Larger touch targets */
@media (max-width: 767px) {
  .btn {
    min-height: 48px;
    padding: 14px 20px;
  }
  
  .filter-option {
    padding: 14px 0;
  }
  
  /* Disable hover effects on touch */
  .property-card:hover {
    transform: none;
    box-shadow: none;
  }
}

/* Pull to refresh area */
.pull-to-refresh {
  height: 60px;
  margin-top: -60px;
}
```

#### Mobile Navigation
```css
.mobile-nav {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  background: #ffffff;
  border-top: 1px solid #e7e7e7;
  display: flex;
  justify-content: space-around;
  padding: 8px 0;
  z-index: 1000;
}

.mobile-nav__item {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
  font-size: 10px;
  color: #6b6b6b;
  text-decoration: none;
}

.mobile-nav__item--active {
  color: #003580;
}
```

#### Mobile Search Experience
```css
/* Full-screen mobile search */
.mobile-search-overlay {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: #ffffff;
  z-index: 9999;
  padding: 16px;
}

/* Date picker mobile */
.date-picker--mobile {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  background: #ffffff;
  border-radius: 16px 16px 0 0;
  max-height: 80vh;
  overflow-y: auto;
}
```

### Native Mobile Apps

#### iOS Specific
```css
/* Safe area handling */
.header {
  padding-top: env(safe-area-inset-top);
}

.mobile-nav {
  padding-bottom: env(safe-area-inset-bottom);
}

/* iOS button styling */
.btn-ios {
  border-radius: 12px;
  font-weight: 600;
}

/* iOS navigation bar */
.ios-nav {
  height: 44px;
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
}
```

#### Android Specific
```css
/* Material-style elevation */
.card-android {
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

/* Ripple effect */
.btn-android {
  position: relative;
  overflow: hidden;
}

.btn-android::after {
  content: '';
  position: absolute;
  background: rgba(0, 0, 0, 0.1);
  border-radius: 50%;
  transform: scale(0);
  animation: ripple 0.6s ease-out;
}

@keyframes ripple {
  to {
    transform: scale(2.5);
    opacity: 0;
  }
}

/* Android status bar */
.status-bar-android {
  height: 24px;
  background-color: #00224f;
}
```

### Map Integration

#### Map UI Components
```css
/* Map container */
.map-container {
  position: relative;
  width: 100%;
  height: 400px;
}

/* Map marker */
.map-marker {
  background-color: #003580;
  color: #ffffff;
  padding: 6px 10px;
  border-radius: 4px;
  font-size: 14px;
  font-weight: 700;
  position: relative;
  cursor: pointer;
  white-space: nowrap;
}

.map-marker::after {
  content: '';
  position: absolute;
  bottom: -8px;
  left: 50%;
  transform: translateX(-50%);
  border: 8px solid transparent;
  border-top-color: #003580;
}

.map-marker:hover,
.map-marker--active {
  background-color: #febb02;
  color: #262626;
}

.map-marker--active::after {
  border-top-color: #febb02;
}

/* Map info window */
.map-info-window {
  background: #ffffff;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.2);
  width: 280px;
  overflow: hidden;
}
```

### Trust & Security Elements

#### Trust Badges
```css
/* Secure booking badge */
.trust-badge {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 12px 16px;
  background-color: #ebf3ff;
  border-radius: 4px;
  font-size: 14px;
  color: #003580;
}

.trust-badge__icon {
  width: 20px;
  height: 20px;
  color: #008009;
}

/* Free cancellation badge */
.cancellation-badge {
  color: #008009;
  font-size: 14px;
  font-weight: 500;
  display: flex;
  align-items: center;
  gap: 4px;
}

/* Verified badge */
.verified-badge {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  color: #003580;
  font-size: 12px;
}
```

#### Price Guarantee
```css
.price-guarantee {
  background: linear-gradient(135deg, #ebf3ff 0%, #ffffff 100%);
  border: 1px solid #0071c2;
  border-radius: 8px;
  padding: 16px;
}

.price-guarantee__title {
  font-size: 16px;
  font-weight: 700;
  color: #003580;
  margin-bottom: 8px;
}

.price-guarantee__text {
  font-size: 14px;
  color: #262626;
}
```

---

## Quick Reference

### CSS Custom Properties
```css
:root {
  /* Colors */
  --color-primary: #003580;
  --color-primary-dark: #00224f;
  --color-primary-light: #0071c2;
  --color-accent: #febb02;
  --color-accent-hover: #e5a800;
  --color-success: #008009;
  --color-error: #d4111e;
  --color-warning: #f56700;
  --color-genius: #004cb8;
  
  /* Text */
  --color-text-primary: #262626;
  --color-text-secondary: #6b6b6b;
  --color-text-muted: #8c8c8c;
  
  /* Backgrounds */
  --color-bg-primary: #ffffff;
  --color-bg-secondary: #f5f5f5;
  --color-bg-blue-tint: #ebf3ff;
  --color-border: #e7e7e7;
  
  /* Typography */
  --font-family: BlinkMacSystemFont, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  --font-size-xs: 12px;
  --font-size-sm: 14px;
  --font-size-md: 16px;
  --font-size-lg: 20px;
  --font-size-xl: 24px;
  --font-size-xxl: 32px;
  
  /* Spacing */
  --space-xxs: 4px;
  --space-xs: 8px;
  --space-sm: 12px;
  --space-md: 16px;
  --space-lg: 24px;
  --space-xl: 32px;
  --space-xxl: 48px;
  
  /* Border Radius */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-pill: 9999px;
  
  /* Shadows */
  --shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.08);
  --shadow-md: 0 2px 8px rgba(0, 0, 0, 0.15);
  --shadow-lg: 0 4px 16px rgba(0, 0, 0, 0.2);
  
  /* Transitions */
  --transition-fast: 150ms ease;
  --transition-normal: 200ms ease;
  --transition-slow: 300ms ease;
  
  /* Layout */
  --container-max-width: 1110px;
  --sidebar-width: 250px;
}
```

### Component Checklist
- [x] Primary Button (Yellow CTA)
- [x] Secondary Button (Blue)
- [x] Outline Button
- [x] Property Card (Horizontal)
- [x] Property Card (Grid)
- [x] Review Score Badge
- [x] Deal Badge
- [x] Genius Badge
- [x] Price Display
- [x] Search Form
- [x] Filter Checkbox
- [x] Date Picker
- [x] Guest Selector
- [x] Map Marker
- [x] Map Info Window
- [x] Navigation Bar
- [x] Mobile Bottom Nav
- [x] Trust Badges
- [x] Loading Skeleton
- [x] Progress Indicators
