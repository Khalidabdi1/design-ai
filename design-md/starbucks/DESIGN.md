# DESIGN.md - Starbucks Design System

## 1. Brand Identity

### Brand Overview
Starbucks is the world's premier coffeehouse company, creating a "third place" between home and work where customers connect over handcrafted beverages and premium food. The brand embodies warmth, community, and the ritual of coffee culture.

### Brand Values
- **Human Connection**: Creating moments of warmth and belonging
- **Quality Craftsmanship**: Ethically sourced, expertly roasted coffee
- **Community**: Being a positive force in neighborhoods worldwide
- **Sustainability**: Commitment to ethical sourcing and environmental responsibility
- **Innovation**: Pioneering mobile ordering and rewards experiences

### Brand Voice
- **Warm**: Friendly and welcoming, like a conversation with your barista
- **Knowledgeable**: Expert without being pretentious
- **Inviting**: Inclusive and approachable to all
- **Personal**: Remembering your name and your drink
- **Optimistic**: Uplifting and positive in tone

### Brand Personality
Starbucks presents itself as a warm, sophisticated friend who knows coffee inside and out. The brand balances accessibility with premium quality, making artisan coffee culture approachable for everyone while maintaining craft integrity.

---

## 2. Color System

### Primary Colors

#### Starbucks Green (Primary)
```css
--starbucks-green: #00704A;
```
- **Usage**: Primary brand color, CTAs, headers, icons, navigation
- **Psychology**: Growth, freshness, premium quality, nature
- **Accessibility**: Use with white text for optimal contrast

#### House Green (Dark Green)
```css
--house-green: #1E3932;
```
- **Usage**: Text, backgrounds, footer, sophisticated accents
- **Psychology**: Sophistication, depth, premium experience
- **Accessibility**: Primary text color, excellent readability

### Secondary Colors

#### Accent Gold
```css
--starbucks-gold: #CBA258;
```
- **Usage**: Rewards program, Star icons, premium indicators, Gold member status
- **Psychology**: Reward, achievement, luxury, warmth

#### Light Green
```css
--light-green: #D4E9E2;
```
- **Usage**: Backgrounds, cards, subtle highlights
- **Psychology**: Fresh, clean, calming

### Neutral Colors

```css
/* Backgrounds */
--white: #FFFFFF;
--warm-white: #F9F9F9;
--cream: #F2F0EB;
--warm-cream: #F1F0EA;

/* Text */
--text-primary: #1E3932;
--text-secondary: #475D5B;
--text-muted: #6B7D7B;

/* Borders & Dividers */
--border-light: #E0E0E0;
--border-medium: #CCCCCC;

/* Functional */
--success: #00754A;
--error: #D62B1F;
--warning: #F2A900;
--info: #006DB6;
```

### Color Application

```css
/* Primary Buttons */
.btn-primary {
  background-color: #00704A;
  color: #FFFFFF;
}

.btn-primary:hover {
  background-color: #1E3932;
}

/* Rewards Gold */
.rewards-star {
  color: #CBA258;
}

.gold-member-badge {
  background: linear-gradient(135deg, #CBA258 0%, #D4AF37 100%);
}

/* Card Backgrounds */
.menu-card {
  background-color: #FFFFFF;
  border: 1px solid #E0E0E0;
}

.featured-card {
  background-color: #F2F0EB;
}
```

---

## 3. Typography

### Font Families

#### SoDo Sans (Primary)
```css
--font-primary: 'SoDo Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
```
- **Usage**: Body text, UI elements, navigation, descriptions
- **Characteristics**: Clean, modern, highly readable sans-serif
- **Weights**: Regular (400), Medium (500), SemiBold (600), Bold (700)

#### Lander (Display)
```css
--font-display: 'Lander', 'Georgia', serif;
```
- **Usage**: Headlines, promotional titles, seasonal campaigns
- **Characteristics**: Elegant serif with personality
- **Weights**: Regular, Bold

#### Pike (Accent)
```css
--font-accent: 'Pike', 'SoDo Sans', sans-serif;
```
- **Usage**: Special callouts, menu categories
- **Characteristics**: Distinctive Starbucks brand font

### Type Scale

```css
/* Display */
--text-display-1: 4rem;      /* 64px - Hero headlines */
--text-display-2: 3rem;      /* 48px - Section headers */
--text-display-3: 2.5rem;    /* 40px - Page titles */

/* Headings */
--text-h1: 2rem;             /* 32px */
--text-h2: 1.5rem;           /* 24px */
--text-h3: 1.25rem;          /* 20px */
--text-h4: 1.125rem;         /* 18px */

/* Body */
--text-body-lg: 1.125rem;    /* 18px */
--text-body: 1rem;           /* 16px */
--text-body-sm: 0.875rem;    /* 14px */

/* Small */
--text-caption: 0.75rem;     /* 12px */
--text-overline: 0.6875rem;  /* 11px */
```

### Typography Styles

```css
/* Hero Headline */
.hero-title {
  font-family: var(--font-display);
  font-size: var(--text-display-1);
  font-weight: 700;
  line-height: 1.1;
  color: var(--text-primary);
  letter-spacing: -0.02em;
}

/* Section Header */
.section-title {
  font-family: var(--font-primary);
  font-size: var(--text-h1);
  font-weight: 700;
  line-height: 1.25;
  color: var(--house-green);
}

/* Menu Item Title */
.menu-item-title {
  font-family: var(--font-primary);
  font-size: var(--text-h3);
  font-weight: 600;
  line-height: 1.3;
  color: var(--text-primary);
}

/* Body Text */
.body-text {
  font-family: var(--font-primary);
  font-size: var(--text-body);
  font-weight: 400;
  line-height: 1.6;
  color: var(--text-secondary);
}

/* Price Display */
.price {
  font-family: var(--font-primary);
  font-size: var(--text-body-lg);
  font-weight: 600;
  color: var(--text-primary);
}

/* Rewards Stars */
.star-count {
  font-family: var(--font-primary);
  font-size: var(--text-h3);
  font-weight: 700;
  color: var(--starbucks-gold);
}
```

---

## 4. Spacing & Layout

### Spacing Scale

```css
--space-0: 0;
--space-1: 0.25rem;    /* 4px */
--space-2: 0.5rem;     /* 8px */
--space-3: 0.75rem;    /* 12px */
--space-4: 1rem;       /* 16px */
--space-5: 1.25rem;    /* 20px */
--space-6: 1.5rem;     /* 24px */
--space-8: 2rem;       /* 32px */
--space-10: 2.5rem;    /* 40px */
--space-12: 3rem;      /* 48px */
--space-16: 4rem;      /* 64px */
--space-20: 5rem;      /* 80px */
--space-24: 6rem;      /* 96px */
```

### Layout Grid

```css
/* Container */
.container {
  max-width: 1440px;
  margin: 0 auto;
  padding: 0 var(--space-6);
}

/* Content Width */
.content-narrow {
  max-width: 680px;
}

.content-medium {
  max-width: 960px;
}

.content-wide {
  max-width: 1200px;
}

/* Menu Grid */
.menu-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: var(--space-6);
}

/* Store Card Grid */
.store-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
  gap: var(--space-4);
}
```

### Section Spacing

```css
/* Page Sections */
.section {
  padding: var(--space-16) 0;
}

.section-lg {
  padding: var(--space-24) 0;
}

/* Card Padding */
.card {
  padding: var(--space-6);
}

.card-compact {
  padding: var(--space-4);
}

/* Component Gaps */
.stack-sm {
  gap: var(--space-2);
}

.stack-md {
  gap: var(--space-4);
}

.stack-lg {
  gap: var(--space-8);
}
```

### Breakpoints

```css
--breakpoint-sm: 375px;   /* Mobile */
--breakpoint-md: 768px;   /* Tablet */
--breakpoint-lg: 1024px;  /* Desktop */
--breakpoint-xl: 1280px;  /* Large Desktop */
--breakpoint-2xl: 1440px; /* Extra Large */
```

---

## 5. Component Library

### Buttons

```css
/* Primary Button - Starbucks Green */
.btn-primary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 0.875rem 1.5rem;
  font-family: var(--font-primary);
  font-size: 1rem;
  font-weight: 600;
  color: #FFFFFF;
  background-color: #00704A;
  border: none;
  border-radius: 50px;
  cursor: pointer;
  transition: all 0.2s ease;
}

.btn-primary:hover {
  background-color: #1E3932;
  transform: scale(1.02);
}

/* Secondary Button - Outline */
.btn-secondary {
  padding: 0.875rem 1.5rem;
  font-family: var(--font-primary);
  font-size: 1rem;
  font-weight: 600;
  color: #00704A;
  background-color: transparent;
  border: 2px solid #00704A;
  border-radius: 50px;
  cursor: pointer;
  transition: all 0.2s ease;
}

.btn-secondary:hover {
  background-color: #00704A;
  color: #FFFFFF;
}

/* Ghost Button */
.btn-ghost {
  padding: 0.75rem 1rem;
  font-weight: 600;
  color: #00704A;
  background: transparent;
  border: none;
  cursor: pointer;
}

.btn-ghost:hover {
  text-decoration: underline;
}

/* Order Button */
.btn-order {
  padding: 0.75rem 1.25rem;
  font-weight: 600;
  color: #FFFFFF;
  background-color: #00704A;
  border-radius: 50px;
  min-width: 120px;
}
```

### Menu Item Cards

```css
/* Menu Item Card */
.menu-card {
  display: flex;
  flex-direction: column;
  background: #FFFFFF;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  cursor: pointer;
}

.menu-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
}

.menu-card__image {
  position: relative;
  aspect-ratio: 1;
  overflow: hidden;
}

.menu-card__image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.menu-card__content {
  padding: var(--space-4);
}

.menu-card__title {
  font-size: var(--text-body-lg);
  font-weight: 600;
  color: var(--text-primary);
  margin-bottom: var(--space-1);
}

.menu-card__calories {
  font-size: var(--text-body-sm);
  color: var(--text-muted);
}

.menu-card__price {
  font-size: var(--text-body);
  font-weight: 600;
  color: var(--text-primary);
  margin-top: var(--space-2);
}
```

### Drink Customization

```css
/* Size Selector */
.size-selector {
  display: flex;
  gap: var(--space-3);
  padding: var(--space-4) 0;
  border-bottom: 1px solid var(--border-light);
}

.size-option {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: var(--space-3);
  border: 2px solid transparent;
  border-radius: 8px;
  cursor: pointer;
  transition: all 0.2s ease;
}

.size-option.active {
  border-color: var(--starbucks-green);
  background-color: var(--light-green);
}

.size-option__icon {
  width: 40px;
  height: 60px;
  margin-bottom: var(--space-2);
}

.size-option__name {
  font-size: var(--text-body-sm);
  font-weight: 600;
  color: var(--text-primary);
}

.size-option__oz {
  font-size: var(--text-caption);
  color: var(--text-muted);
}

/* Customization Options */
.customization-group {
  padding: var(--space-4) 0;
  border-bottom: 1px solid var(--border-light);
}

.customization-group__title {
  font-size: var(--text-body);
  font-weight: 600;
  color: var(--text-primary);
  margin-bottom: var(--space-3);
}

.customization-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: var(--space-2) 0;
}

.quantity-stepper {
  display: flex;
  align-items: center;
  gap: var(--space-3);
}

.quantity-btn {
  width: 32px;
  height: 32px;
  border-radius: 50%;
  border: 2px solid var(--starbucks-green);
  background: transparent;
  color: var(--starbucks-green);
  font-size: 1.25rem;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}

.quantity-btn:disabled {
  border-color: var(--border-light);
  color: var(--text-muted);
  cursor: not-allowed;
}
```

### Rewards Components

```css
/* Star Counter */
.star-counter {
  display: flex;
  align-items: center;
  gap: var(--space-2);
}

.star-icon {
  width: 24px;
  height: 24px;
  fill: var(--starbucks-gold);
}

.star-count {
  font-size: var(--text-h3);
  font-weight: 700;
  color: var(--starbucks-gold);
}

.star-label {
  font-size: var(--text-body-sm);
  color: var(--text-secondary);
}

/* Rewards Progress Bar */
.rewards-progress {
  background: var(--warm-cream);
  border-radius: 8px;
  padding: var(--space-4);
}

.progress-bar {
  height: 8px;
  background: var(--border-light);
  border-radius: 4px;
  overflow: hidden;
  margin: var(--space-3) 0;
}

.progress-fill {
  height: 100%;
  background: linear-gradient(90deg, var(--starbucks-gold) 0%, #D4AF37 100%);
  border-radius: 4px;
  transition: width 0.3s ease;
}

.progress-milestones {
  display: flex;
  justify-content: space-between;
  font-size: var(--text-caption);
  color: var(--text-muted);
}

/* Reward Card */
.reward-card {
  display: flex;
  align-items: center;
  gap: var(--space-4);
  padding: var(--space-4);
  background: #FFFFFF;
  border-radius: 8px;
  border: 1px solid var(--border-light);
}

.reward-card__stars {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 48px;
  height: 48px;
  background: var(--starbucks-gold);
  color: #FFFFFF;
  border-radius: 50%;
  font-weight: 700;
}

.reward-card__info {
  flex: 1;
}

.reward-card__title {
  font-weight: 600;
  color: var(--text-primary);
}

.reward-card__description {
  font-size: var(--text-body-sm);
  color: var(--text-secondary);
}
```

### Store Locator

```css
/* Store Card */
.store-card {
  padding: var(--space-4);
  background: #FFFFFF;
  border-radius: 8px;
  border: 1px solid var(--border-light);
  cursor: pointer;
  transition: border-color 0.2s ease;
}

.store-card:hover {
  border-color: var(--starbucks-green);
}

.store-card.active {
  border-color: var(--starbucks-green);
  border-width: 2px;
}

.store-card__header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: var(--space-2);
}

.store-card__name {
  font-weight: 600;
  color: var(--text-primary);
}

.store-card__distance {
  font-size: var(--text-body-sm);
  color: var(--text-muted);
}

.store-card__address {
  font-size: var(--text-body-sm);
  color: var(--text-secondary);
  margin-bottom: var(--space-3);
}

.store-card__features {
  display: flex;
  flex-wrap: wrap;
  gap: var(--space-2);
}

.feature-tag {
  padding: 0.25rem 0.5rem;
  font-size: var(--text-caption);
  background: var(--warm-cream);
  color: var(--text-secondary);
  border-radius: 4px;
}

/* Store Hours */
.store-hours {
  font-size: var(--text-body-sm);
}

.store-hours__status {
  font-weight: 600;
}

.store-hours__status.open {
  color: var(--success);
}

.store-hours__status.closed {
  color: var(--error);
}
```

### Navigation

```css
/* Main Navigation */
.nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: var(--space-4) var(--space-6);
  background: #FFFFFF;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.08);
  position: sticky;
  top: 0;
  z-index: 100;
}

.nav__logo {
  width: 50px;
  height: 50px;
}

.nav__links {
  display: flex;
  align-items: center;
  gap: var(--space-8);
}

.nav__link {
  font-family: var(--font-primary);
  font-size: var(--text-body);
  font-weight: 600;
  color: var(--text-primary);
  text-decoration: none;
  padding: var(--space-2) 0;
  border-bottom: 2px solid transparent;
  transition: border-color 0.2s ease;
}

.nav__link:hover {
  border-color: var(--starbucks-green);
}

.nav__link.active {
  color: var(--starbucks-green);
  border-color: var(--starbucks-green);
}

.nav__actions {
  display: flex;
  align-items: center;
  gap: var(--space-4);
}

/* Mobile Menu */
.mobile-menu {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: #FFFFFF;
  padding: var(--space-6);
  z-index: 200;
  transform: translateX(100%);
  transition: transform 0.3s ease;
}

.mobile-menu.open {
  transform: translateX(0);
}
```

---

## 6. Iconography

### Icon Style Guidelines
- **Style**: Rounded, friendly, approachable
- **Stroke Width**: 2px for consistency
- **Corners**: Rounded ends, soft curves
- **Size**: 24px base, scaling to 16px, 20px, 32px, 48px

### Core Icons

```
Navigation:
[=]  Menu hamburger
[<-] Back arrow
[X]  Close
[v]  Chevron down
[>]  Chevron right
[O]  Search (magnifying glass)

Actions:
[+]  Add to cart
[-]  Remove
[heart] Favorite
[share] Share
[edit] Edit/Customize
[trash] Delete

Drinks & Food:
[cup] Coffee cup (various sizes)
[mug] Hot drink
[ice] Iced drink
[food] Food item
[bakery] Pastry

Rewards:
[star] Star (filled/outline)
[gift] Reward/Gift
[crown] Gold status
[sparkle] Bonus stars

Location:
[pin] Store location
[compass] Navigate
[clock] Store hours
[car] Drive-thru

Account:
[person] Profile
[card] Payment
[history] Order history
[settings] Settings
```

### Icon Sizes

```css
--icon-xs: 16px;  /* Inline indicators */
--icon-sm: 20px;  /* Compact UI */
--icon-md: 24px;  /* Default */
--icon-lg: 32px;  /* Featured icons */
--icon-xl: 48px;  /* Hero icons */
```

### Star Icon (Rewards)

```css
/* Filled Star */
.star-filled {
  fill: var(--starbucks-gold);
}

/* Outline Star */
.star-outline {
  fill: none;
  stroke: var(--starbucks-gold);
  stroke-width: 2px;
}

/* Animated Star Earn */
@keyframes starEarn {
  0% { transform: scale(1); }
  50% { transform: scale(1.3); }
  100% { transform: scale(1); }
}

.star-earned {
  animation: starEarn 0.4s ease;
}
```

---

## 7. Motion & Animation

### Animation Principles
- **Natural**: Movements inspired by coffee pouring, steam rising
- **Purposeful**: Animations guide attention and provide feedback
- **Warm**: Easing curves that feel inviting, not mechanical
- **Quick**: Snappy interactions that respect user time

### Timing Values

```css
--duration-instant: 100ms;   /* Micro-interactions */
--duration-fast: 200ms;      /* Buttons, toggles */
--duration-normal: 300ms;    /* Cards, modals */
--duration-slow: 400ms;      /* Page transitions */
--duration-slower: 500ms;    /* Complex animations */
```

### Easing Curves

```css
--ease-default: cubic-bezier(0.4, 0, 0.2, 1);     /* Standard */
--ease-in: cubic-bezier(0.4, 0, 1, 1);            /* Enter */
--ease-out: cubic-bezier(0, 0, 0.2, 1);           /* Exit */
--ease-bounce: cubic-bezier(0.34, 1.56, 0.64, 1); /* Playful */
```

### Component Animations

```css
/* Button Hover */
.btn-primary {
  transition: background-color var(--duration-fast) var(--ease-default),
              transform var(--duration-fast) var(--ease-default);
}

.btn-primary:hover {
  transform: scale(1.02);
}

.btn-primary:active {
  transform: scale(0.98);
}

/* Card Hover */
.menu-card {
  transition: transform var(--duration-normal) var(--ease-out),
              box-shadow var(--duration-normal) var(--ease-out);
}

.menu-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
}

/* Add to Bag Animation */
@keyframes addToBag {
  0% { transform: scale(1); }
  25% { transform: scale(1.1); }
  50% { transform: scale(0.95); }
  100% { transform: scale(1); }
}

.add-to-bag-success {
  animation: addToBag 0.4s var(--ease-bounce);
}

/* Star Earn Animation */
@keyframes earnStar {
  0% { 
    opacity: 0;
    transform: translateY(10px) scale(0.5);
  }
  100% { 
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}

.star-earn {
  animation: earnStar 0.5s var(--ease-bounce);
}

/* Progress Fill */
.progress-fill {
  transition: width 1s var(--ease-out);
}

/* Page Fade In */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

.page-enter {
  animation: fadeIn var(--duration-normal) var(--ease-out);
}

/* Slide Up (Modal/Sheet) */
@keyframes slideUp {
  from {
    opacity: 0;
    transform: translateY(100%);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.modal-enter {
  animation: slideUp var(--duration-slow) var(--ease-out);
}

/* Loading Spinner */
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.spinner {
  width: 24px;
  height: 24px;
  border: 3px solid var(--border-light);
  border-top-color: var(--starbucks-green);
  border-radius: 50%;
  animation: spin 0.8s linear infinite;
}

/* Skeleton Loading */
@keyframes shimmer {
  0% { background-position: -200% 0; }
  100% { background-position: 200% 0; }
}

.skeleton {
  background: linear-gradient(
    90deg,
    var(--warm-cream) 25%,
    #E0E0E0 50%,
    var(--warm-cream) 75%
  );
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite;
}
```

---

## 8. Accessibility

### Color Contrast

| Combination | Ratio | WCAG |
|-------------|-------|------|
| White on Starbucks Green (#00704A) | 4.8:1 | AA |
| White on House Green (#1E3932) | 11.5:1 | AAA |
| House Green on White | 11.5:1 | AAA |
| Starbucks Green on White | 4.8:1 | AA |
| Gold (#CBA258) on House Green | 5.2:1 | AA |
| Text Secondary on White | 7.1:1 | AAA |

### Focus States

```css
/* Default Focus Ring */
*:focus-visible {
  outline: 2px solid var(--starbucks-green);
  outline-offset: 2px;
}

/* Button Focus */
.btn:focus-visible {
  outline: 3px solid var(--starbucks-green);
  outline-offset: 2px;
  box-shadow: 0 0 0 4px rgba(0, 112, 74, 0.2);
}

/* Input Focus */
.input:focus {
  border-color: var(--starbucks-green);
  box-shadow: 0 0 0 3px rgba(0, 112, 74, 0.15);
}

/* Card Focus */
.menu-card:focus-visible {
  outline: 2px solid var(--starbucks-green);
  outline-offset: 4px;
}

/* Skip Link */
.skip-link {
  position: absolute;
  top: -100px;
  left: 50%;
  transform: translateX(-50%);
  padding: var(--space-3) var(--space-4);
  background: var(--house-green);
  color: #FFFFFF;
  border-radius: 4px;
  z-index: 1000;
}

.skip-link:focus {
  top: var(--space-4);
}
```

### Screen Reader Support

```html
<!-- Live Region for Cart Updates -->
<div 
  aria-live="polite" 
  aria-atomic="true" 
  class="sr-only"
>
  Item added to bag. Total: 3 items.
</div>

<!-- Star Counter -->
<div aria-label="You have 125 Stars">
  <span aria-hidden="true">125</span>
  <span class="sr-only">Stars</span>
</div>

<!-- Menu Item Card -->
<article aria-labelledby="item-name" role="button" tabindex="0">
  <img src="drink.jpg" alt="Caramel Macchiato, iced, in a tall cup">
  <h3 id="item-name">Caramel Macchiato</h3>
  <p>250 calories</p>
  <p><span class="sr-only">Price:</span> $5.25</p>
</article>

<!-- Size Selector -->
<fieldset>
  <legend>Choose your size</legend>
  <label>
    <input type="radio" name="size" value="tall">
    Tall (12 fl oz)
  </label>
  <label>
    <input type="radio" name="size" value="grande" checked>
    Grande (16 fl oz)
  </label>
  <label>
    <input type="radio" name="size" value="venti">
    Venti (20 fl oz)
  </label>
</fieldset>
```

### Touch Targets

```css
/* Minimum touch target: 44x44px */
.btn,
.nav__link,
.menu-card,
.store-card {
  min-height: 44px;
  min-width: 44px;
}

/* Quantity Stepper */
.quantity-btn {
  width: 44px;
  height: 44px;
}

/* Checkbox/Radio */
.custom-checkbox,
.custom-radio {
  width: 24px;
  height: 24px;
  /* Padding extends touch target */
  padding: 10px;
  margin: -10px;
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
  }
  
  .menu-card:hover {
    transform: none;
  }
}
```

---

## 9. Platform-Specific Guidelines

### iOS App

```swift
// Colors
extension Color {
    static let starbucksGreen = Color(hex: "#00704A")
    static let houseGreen = Color(hex: "#1E3932")
    static let rewardsGold = Color(hex: "#CBA258")
    static let warmCream = Color(hex: "#F2F0EB")
}

// Typography
extension Font {
    static let headline = Font.custom("SoDoSans-Bold", size: 24)
    static let title = Font.custom("SoDoSans-SemiBold", size: 20)
    static let body = Font.custom("SoDoSans-Regular", size: 16)
    static let caption = Font.custom("SoDoSans-Regular", size: 14)
}

// Corner Radius
extension CGFloat {
    static let radiusSmall: CGFloat = 8
    static let radiusMedium: CGFloat = 12
    static let radiusLarge: CGFloat = 16
    static let radiusFull: CGFloat = 50
}
```

#### iOS-Specific Patterns
- Use native tab bar with custom green tint
- Support Dynamic Type for accessibility
- Implement haptic feedback for add-to-cart actions
- Use SF Symbols alongside custom icons
- Support Dark Mode with inverted greens

### Android App

```kotlin
// Colors (colors.xml)
<color name="starbucks_green">#00704A</color>
<color name="house_green">#1E3932</color>
<color name="rewards_gold">#CBA258</color>
<color name="warm_cream">#F2F0EB</color>

// Typography
<style name="TextAppearance.Starbucks.Headline">
    <item name="fontFamily">@font/sodo_sans_bold</item>
    <item name="android:textSize">24sp</item>
</style>

// Button Style
<style name="Widget.Starbucks.Button.Primary">
    <item name="android:background">@drawable/bg_button_primary</item>
    <item name="android:textColor">@color/white</item>
    <item name="android:paddingVertical">14dp</item>
    <item name="android:paddingHorizontal">24dp</item>
    <item name="cornerRadius">50dp</item>
</style>
```

#### Android-Specific Patterns
- Follow Material Design 3 with Starbucks theming
- Support edge-to-edge content
- Implement predictive back gestures
- Use Material motion patterns
- Support Dynamic Color with brand color fallbacks

### Web Application

```css
/* Responsive Images */
.menu-image {
  aspect-ratio: 1;
  object-fit: cover;
  width: 100%;
}

/* Mobile-First Menu */
@media (max-width: 767px) {
  .menu-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: var(--space-3);
  }
  
  .menu-card__image {
    aspect-ratio: 1;
  }
}

@media (min-width: 768px) {
  .menu-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

@media (min-width: 1024px) {
  .menu-grid {
    grid-template-columns: repeat(4, 1fr);
  }
}

/* Mobile Order Flow */
@media (max-width: 767px) {
  .order-footer {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    padding: var(--space-4);
    background: #FFFFFF;
    box-shadow: 0 -4px 12px rgba(0, 0, 0, 0.1);
  }
}
```

### In-Store Kiosk

```css
/* Large Touch Targets */
.kiosk-btn {
  min-height: 72px;
  min-width: 200px;
  font-size: 1.5rem;
  padding: var(--space-6) var(--space-8);
}

/* High Contrast Mode */
.kiosk-mode {
  --text-primary: #000000;
  --starbucks-green: #006644;
}

/* Menu Item (Larger) */
.kiosk-menu-card {
  padding: var(--space-6);
}

.kiosk-menu-card__title {
  font-size: 1.5rem;
}

.kiosk-menu-card__image {
  min-height: 200px;
}
```

### Email Templates

```html
<!-- Email-Safe Colors -->
<style>
  .header { background-color: #1E3932; }
  .cta-button { 
    background-color: #00704A;
    color: #FFFFFF;
    padding: 16px 32px;
    border-radius: 50px;
    text-decoration: none;
    display: inline-block;
  }
  .stars { color: #CBA258; }
  .footer { background-color: #F2F0EB; }
</style>

<!-- Fallback Fonts -->
<td style="font-family: 'SoDo Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;">
```

---

## Appendix: Quick Reference

### Color Tokens
```
Primary:      #00704A (Starbucks Green)
Secondary:    #1E3932 (House Green)
Accent:       #CBA258 (Rewards Gold)
Background:   #FFFFFF, #F2F0EB
Text:         #1E3932, #475D5B
```

### Font Stack
```
Primary:  SoDo Sans, Helvetica Neue, Arial, sans-serif
Display:  Lander, Georgia, serif
```

### Core Spacing
```
4px | 8px | 12px | 16px | 24px | 32px | 48px | 64px
```

### Border Radius
```
Small:    4px
Medium:   8px
Large:    12px
Full:     50px (buttons)
```

### Breakpoints
```
Mobile:   375px
Tablet:   768px
Desktop:  1024px
Large:    1280px
```

### Z-Index Scale
```
Dropdown:   100
Sticky:     200
Modal:      300
Toast:      400
Tooltip:    500
```

---

*Version 1.0 | Starbucks Design System*
*Creating warmth and connection, one cup at a time*
