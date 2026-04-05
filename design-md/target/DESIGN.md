# Target Design System

## 1. Brand Overview

Target Corporation is one of America's largest retailers, known for its distinctive red bullseye logo and commitment to delivering an elevated shopping experience at affordable prices. Founded in 1962, Target has cultivated a brand identity that balances approachability with style, often described as "cheap chic." The design system reflects Target's mission to help all families discover the joy of everyday life through accessible design, quality products, and exceptional value.

Target's visual identity centers around its iconic bullseye logo—a simple yet powerful symbol representing precision, focus, and hitting the mark for guests. The brand communicates warmth, reliability, and modern retail innovation while maintaining a clean, organized aesthetic that makes shopping intuitive and enjoyable.

**Core Brand Values:**
- Inclusivity and accessibility for all guests
- Joy and discovery in everyday shopping
- Quality and style at affordable prices
- Community connection and local relevance
- Innovation in retail experience

---

## 2. Color Palette

### Primary Colors

| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Target Red | `#CC0000` | 204, 0, 0 | Primary brand color, CTAs, bullseye logo, key actions |
| Target Red Dark | `#A80000` | 168, 0, 0 | Hover states, active buttons, emphasis |
| Target Red Light | `#FF3333` | 255, 51, 51 | Highlights, sale tags, promotional accents |

### Neutral Colors

| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| White | `#FFFFFF` | 255, 255, 255 | Primary background, cards, clean spaces |
| Off White | `#FAFAFA` | 250, 250, 250 | Alternate backgrounds, subtle separation |
| Light Gray | `#F7F7F7` | 247, 247, 247 | Section backgrounds, containers |
| Gray 100 | `#EDEDED` | 237, 237, 237 | Borders, dividers, disabled states |
| Gray 200 | `#D6D6D6` | 214, 214, 214 | Input borders, secondary dividers |
| Gray 300 | `#888888` | 136, 136, 136 | Placeholder text, muted content |
| Gray 400 | `#666666` | 102, 102, 102 | Secondary text, metadata |
| Charcoal | `#333333` | 51, 51, 51 | Primary text, headings |
| Black | `#000000` | 0, 0, 0 | High contrast text, icons |

### Semantic Colors

| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Success Green | `#008300` | 0, 131, 0 | In stock, delivery available, success states |
| Warning Yellow | `#FFB800` | 255, 184, 0 | Limited stock, warnings, attention |
| Error Red | `#CC0000` | 204, 0, 0 | Errors (same as brand red) |
| Info Blue | `#0066CC` | 0, 102, 204 | Links, informational elements |
| Circle Gold | `#DAAA00` | 218, 170, 0 | Target Circle rewards, member benefits |

### Promotional Colors

| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Sale Red | `#CC0000` | 204, 0, 0 | Sale pricing, clearance |
| Deal Green | `#008300` | 0, 131, 0 | Circle deals, member savings |
| Same-Day Blue | `#0066CC` | 0, 102, 204 | Same-day delivery/pickup badges |
| Shipt Green | `#00875A` | 0, 135, 90 | Shipt delivery integration |

---

## 3. Typography

### Font Stack

```css
/* Primary Font Stack */
font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;

/* System Font Fallback */
font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, 
             "Helvetica Neue", Arial, sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Usage |
|---------|------|--------|-------------|----------------|-------|
| Display XL | 48px | 700 (Bold) | 1.1 | -0.5px | Hero headlines, major promotions |
| Display L | 36px | 700 (Bold) | 1.15 | -0.3px | Page titles, campaign headers |
| Heading 1 | 28px | 700 (Bold) | 1.2 | -0.2px | Section headers, category titles |
| Heading 2 | 24px | 700 (Bold) | 1.25 | -0.1px | Subsection headers |
| Heading 3 | 20px | 600 (Semibold) | 1.3 | 0 | Card titles, product names |
| Heading 4 | 18px | 600 (Semibold) | 1.35 | 0 | Minor headings, labels |
| Body Large | 16px | 400 (Regular) | 1.5 | 0 | Primary body text |
| Body | 14px | 400 (Regular) | 1.5 | 0 | Standard body, descriptions |
| Body Small | 13px | 400 (Regular) | 1.45 | 0 | Secondary information |
| Caption | 12px | 400 (Regular) | 1.4 | 0.1px | Metadata, timestamps |
| Micro | 11px | 500 (Medium) | 1.3 | 0.3px | Badges, labels, legal text |

### Font Weights

| Weight Name | Value | Usage |
|-------------|-------|-------|
| Regular | 400 | Body text, descriptions |
| Medium | 500 | Emphasis, badges, buttons |
| Semibold | 600 | Subheadings, product titles |
| Bold | 700 | Headlines, CTAs, prices |

### Typography Guidelines

- Headlines use bold weights for strong visual hierarchy
- Product names are semibold to stand out in listings
- Prices are always bold with clear visual prominence
- Sale prices appear in Target Red, regular prices in charcoal
- Body text maintains comfortable reading with 1.5 line height
- All caps used sparingly for badges and labels only

---

## 4. Spacing System

### Base Unit

Target uses an 8px base spacing unit for consistent rhythm and alignment.

### Spacing Scale

| Token | Size | Usage |
|-------|------|-------|
| `space-0` | 0px | No spacing |
| `space-1` | 4px | Tight spacing, inline elements |
| `space-2` | 8px | Compact spacing, icon gaps |
| `space-3` | 12px | Small component padding |
| `space-4` | 16px | Standard padding, card gutters |
| `space-5` | 20px | Medium spacing |
| `space-6` | 24px | Section padding, card spacing |
| `space-7` | 32px | Large section gaps |
| `space-8` | 40px | Major section separators |
| `space-9` | 48px | Page section spacing |
| `space-10` | 64px | Large layout gaps |
| `space-11` | 80px | Hero spacing |
| `space-12` | 96px | Maximum spacing |

### Layout Spacing

| Context | Value | Usage |
|---------|-------|-------|
| Page Margin Mobile | 16px | Side margins on mobile |
| Page Margin Tablet | 24px | Side margins on tablet |
| Page Margin Desktop | 32-48px | Side margins on desktop |
| Grid Gutter | 16px | Gap between product cards |
| Section Gap | 32-48px | Vertical space between sections |
| Card Padding | 16px | Internal card spacing |
| Header Height | 64-72px | Top navigation bar |

---

## 5. Component Library

### Buttons

**Primary Button (Target Red)**
```
- Background: #CC0000
- Text: #FFFFFF
- Font: 14-16px, Bold (700)
- Padding: 12px 24px
- Border Radius: 4px
- Hover: #A80000
- Active: #8B0000
- Disabled: #D6D6D6 background, #888888 text
```

**Secondary Button (Outlined)**
```
- Background: Transparent
- Border: 2px solid #CC0000
- Text: #CC0000
- Font: 14-16px, Bold (700)
- Padding: 10px 22px
- Border Radius: 4px
- Hover: #CC0000 background, #FFFFFF text
```

**Tertiary Button (Text)**
```
- Background: Transparent
- Text: #CC0000
- Font: 14px, Medium (500)
- Padding: 8px 16px
- Hover: Underline, #A80000 text
```

**Add to Cart Button**
```
- Background: #CC0000
- Text: #FFFFFF
- Font: 14px, Bold (700)
- Padding: 12px 32px
- Border Radius: 4px
- Full width on product pages
- Icon: Cart icon left-aligned
```

### Product Cards

**Standard Product Card**
```
Structure:
├── Image Container (aspect ratio 1:1)
│   ├── Product Image
│   ├── Favorite Heart Icon (top right)
│   └── Badges (top left)
├── Product Info
│   ├── Brand Name (12px, #666666)
│   ├── Product Name (14px, #333333, semibold)
│   ├── Rating Stars + Review Count
│   └── Price Section
│       ├── Current Price (16px, bold)
│       ├── Was Price (strikethrough, #666666)
│       └── Circle Deal Badge (if applicable)
└── Delivery Options (12px icons + text)

Dimensions:
- Card Width: Flexible (grid-based)
- Image: Square aspect ratio
- Card Padding: 12-16px
- Border Radius: 8px
- Shadow: 0 2px 4px rgba(0,0,0,0.08) on hover
```

**Deal Card**
```
- Red accent border or badge
- Circle savings highlighted
- "Deal" label in red
- Member pricing prominent
```

### Navigation

**Header Navigation**
```
Structure:
├── Top Bar (utility nav)
│   ├── Store Finder
│   ├── Registry
│   ├── Weekly Ad
│   └── RedCard
├── Main Header
│   ├── Bullseye Logo
│   ├── Category Menu
│   ├── Search Bar (prominent, centered)
│   ├── Sign In
│   ├── Cart Icon with Count
│   └── Same-Day Delivery Location
└── Category Bar (desktop)
    └── Department Links

Colors:
- Background: #FFFFFF
- Text: #333333
- Logo: #CC0000
- Active/Hover: #CC0000
```

**Mobile Navigation**
```
- Hamburger menu icon
- Full-screen overlay
- Category accordion
- Search prominently placed
- Bottom nav bar with key actions
```

### Search

**Search Bar**
```
- Border: 1px solid #D6D6D6
- Border Radius: 4px
- Height: 44px
- Icon: Magnifying glass, #666666
- Placeholder: "What can we help you find?"
- Focus: Border #CC0000, subtle shadow
- Autocomplete dropdown with categories
```

### Badges

**Sale Badge**
```
- Background: #CC0000
- Text: #FFFFFF
- Font: 11px, Bold, uppercase
- Padding: 4px 8px
- Border Radius: 2px
- Text: "SALE", "CLEARANCE"
```

**Circle Deal Badge**
```
- Background: #008300
- Text: #FFFFFF
- Font: 11px, Bold
- Icon: Circle logo
- Text: "Circle" or percentage saved
```

**Same-Day Badge**
```
- Background: #0066CC or transparent with border
- Text: #0066CC
- Font: 11px, Medium
- Icon: Clock or delivery icon
- Text: "Same Day Delivery", "Drive Up", "Order Pickup"
```

**New Badge**
```
- Background: #333333
- Text: #FFFFFF
- Font: 11px, Bold, uppercase
- Text: "NEW"
```

### Rating Stars

```
- Filled Star: #DAAA00 (gold)
- Empty Star: #D6D6D6
- Size: 14-16px
- Review Count: (123) in #666666
```

### Form Elements

**Input Fields**
```
- Border: 1px solid #D6D6D6
- Border Radius: 4px
- Height: 44px
- Padding: 12px 16px
- Font: 14px, Regular
- Focus: Border #CC0000, shadow
- Error: Border #CC0000, error message below
```

**Checkbox**
```
- Size: 20px
- Border: 2px solid #666666
- Checked: #CC0000 fill, white checkmark
- Border Radius: 2px
```

**Radio Button**
```
- Size: 20px
- Border: 2px solid #666666
- Selected: #CC0000 inner dot
```

### Cards & Containers

**Category Card**
```
- Image: Circular or square with rounded corners
- Title: Centered below, 14px semibold
- Hover: Subtle lift, red underline on text
```

**Deal Tile**
```
- Background: Promotional color or image
- Large percentage or price
- Short description
- "Shop now" link in red
```

**Content Card**
```
- Background: #FFFFFF
- Border: None or 1px #EDEDED
- Border Radius: 8px
- Shadow: 0 1px 3px rgba(0,0,0,0.1)
- Padding: 16-24px
```

---

## 6. Iconography

### Icon Style

- **Style:** Outlined with 1.5-2px stroke weight
- **Corners:** Rounded for approachability
- **Size Grid:** 16px, 20px, 24px, 32px
- **Color:** Inherit from context or #333333 default

### Core Icons

| Icon | Usage | Notes |
|------|-------|-------|
| Bullseye | Brand logo, loading states | Always Target Red |
| Cart | Shopping cart, add to cart | Shows count badge |
| Heart | Favorites, save items | Filled when active |
| Search | Search functionality | Magnifying glass |
| User | Account, sign in | Profile silhouette |
| Location | Store finder, delivery | Pin marker |
| Clock | Same-day delivery times | Circular clock |
| Truck | Shipping, delivery | Delivery vehicle |
| Store | Pickup, store location | Building icon |
| Check | Success, completed | Checkmark |
| Star | Ratings | Five-star system |
| Filter | Sort/filter products | Funnel shape |
| Close | Close modals, remove | X mark |
| Menu | Mobile navigation | Hamburger |
| Arrow | Navigation, accordions | Directional |
| Gift | Registry, gifts | Gift box |
| Barcode | Scan, wallet | Scanner lines |
| Circle | Target Circle program | Circle logo mark |

### Icon Colors

| Context | Color | Hex |
|---------|-------|-----|
| Default | Charcoal | #333333 |
| Interactive | Target Red | #CC0000 |
| Muted | Gray | #888888 |
| Success | Green | #008300 |
| On Dark | White | #FFFFFF |

---

## 7. Layout & Grid

### Breakpoints

| Name | Width | Columns | Margin | Gutter |
|------|-------|---------|--------|--------|
| Mobile Small | 0-375px | 2 | 16px | 12px |
| Mobile | 376-599px | 2 | 16px | 16px |
| Tablet | 600-899px | 3-4 | 24px | 16px |
| Desktop Small | 900-1199px | 4-5 | 32px | 20px |
| Desktop | 1200-1439px | 5-6 | 40px | 24px |
| Desktop Large | 1440px+ | 6 | 48px | 24px |

### Max Content Width

```
- Maximum: 1440px
- Content area: 1200-1344px
- Centered with auto margins
```

### Product Grid

| Viewport | Products Per Row | Card Width |
|----------|------------------|------------|
| Mobile | 2 | ~160px |
| Tablet | 3-4 | ~180px |
| Desktop | 4-5 | ~220px |
| Large Desktop | 5-6 | ~240px |

### Page Structure

```
Layout:
├── Header (fixed on scroll)
│   ├── Utility Bar
│   ├── Main Navigation
│   └── Category Bar
├── Hero Section (optional)
├── Main Content
│   ├── Breadcrumbs
│   ├── Page Title
│   ├── Filters Sidebar (desktop)
│   ├── Product Grid
│   └── Pagination
├── Recommendations
└── Footer
    ├── Links Grid
    ├── App Downloads
    ├── Social Links
    └── Legal
```

---

## 8. Motion & Animation

### Timing Functions

| Name | Value | Usage |
|------|-------|-------|
| Ease Default | `cubic-bezier(0.4, 0, 0.2, 1)` | General transitions |
| Ease In | `cubic-bezier(0.4, 0, 1, 1)` | Elements exiting |
| Ease Out | `cubic-bezier(0, 0, 0.2, 1)` | Elements entering |
| Ease In Out | `cubic-bezier(0.4, 0, 0.2, 1)` | Morphing elements |

### Durations

| Duration | Time | Usage |
|----------|------|-------|
| Instant | 100ms | Micro-interactions, hovers |
| Fast | 150ms | Button states, toggles |
| Normal | 200ms | Standard transitions |
| Moderate | 300ms | Panels, modals appearing |
| Slow | 400ms | Page transitions, complex animations |

### Common Animations

**Hover Lift**
```css
transition: transform 200ms ease, box-shadow 200ms ease;
transform: translateY(-2px);
box-shadow: 0 4px 12px rgba(0, 0, 0, 0.12);
```

**Button Press**
```css
transition: transform 100ms ease;
transform: scale(0.98);
```

**Fade In**
```css
animation: fadeIn 200ms ease-out;
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}
```

**Slide Up (Modal/Drawer)**
```css
animation: slideUp 300ms ease-out;
@keyframes slideUp {
  from { 
    opacity: 0;
    transform: translateY(20px);
  }
  to { 
    opacity: 1;
    transform: translateY(0);
  }
}
```

**Add to Cart Success**
```css
/* Cart icon bounce */
animation: cartBounce 400ms ease;
@keyframes cartBounce {
  0%, 100% { transform: scale(1); }
  50% { transform: scale(1.2); }
}
```

**Loading Spinner**
```css
/* Bullseye-inspired spinner */
animation: spin 1s linear infinite;
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
```

### Animation Guidelines

- Use motion to provide feedback and guide attention
- Keep animations subtle and purposeful
- Respect user's reduced motion preferences
- Loading states should indicate progress
- Cart updates should be clearly visible
- Page transitions should feel quick and seamless

---

## 9. Accessibility

### Color Contrast

| Combination | Ratio | WCAG Level |
|-------------|-------|------------|
| Charcoal (#333333) on White (#FFFFFF) | 12.6:1 | AAA |
| Target Red (#CC0000) on White (#FFFFFF) | 5.9:1 | AA |
| White (#FFFFFF) on Target Red (#CC0000) | 5.9:1 | AA |
| Gray 400 (#666666) on White (#FFFFFF) | 5.7:1 | AA |
| Gray 300 (#888888) on White (#FFFFFF) | 3.5:1 | AA Large |
| Success Green (#008300) on White (#FFFFFF) | 4.6:1 | AA Large |

### Focus States

```css
/* Focus ring for keyboard navigation */
:focus-visible {
  outline: 2px solid #CC0000;
  outline-offset: 2px;
}

/* Enhanced focus for form elements */
input:focus,
select:focus,
textarea:focus {
  border-color: #CC0000;
  box-shadow: 0 0 0 3px rgba(204, 0, 0, 0.2);
  outline: none;
}
```

### Accessibility Requirements

**Keyboard Navigation**
- All interactive elements accessible via keyboard
- Logical tab order following visual layout
- Skip links to main content and navigation
- Focus traps in modals with Escape to close
- Arrow key navigation in menus and carousels

**Screen Readers**
- Semantic HTML structure (header, nav, main, footer)
- Proper heading hierarchy (h1-h6)
- Alt text for all product images
- ARIA labels for icon-only buttons
- Live regions for cart updates and notifications
- Form labels associated with inputs

**ARIA Patterns**

```html
<!-- Product Card -->
<article aria-label="Product: Pillowfort Kids Bedding Set">
  <img alt="Blue striped kids bedding set" />
  <h3>Pillowfort Kids Bedding Set</h3>
  <div role="img" aria-label="4 out of 5 stars">
    <!-- Star rating -->
  </div>
  <button aria-label="Add Pillowfort Kids Bedding Set to cart">
    Add to cart
  </button>
</article>

<!-- Favorite Button -->
<button 
  aria-label="Save to favorites" 
  aria-pressed="false">
  <svg aria-hidden="true"><!-- heart icon --></svg>
</button>

<!-- Cart Count -->
<a href="/cart" aria-label="Cart, 3 items">
  <svg aria-hidden="true"><!-- cart icon --></svg>
  <span aria-hidden="true">3</span>
</a>

<!-- Delivery Options -->
<div role="group" aria-label="Delivery options">
  <span>Same Day Delivery</span>
  <span>Free with orders $35+</span>
</div>
```

**Touch & Mobile**
- Minimum touch target: 44x44px
- Adequate spacing between touch targets
- Swipe gestures have button alternatives
- Pinch-to-zoom not disabled on product images
- Forms optimized for mobile input types

**Content Accessibility**
- Price information clearly announced
- Sale prices include original price context
- Delivery timeframes clearly stated
- Error messages are descriptive and helpful
- Success confirmations are announced

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

### Color Independence

- Never rely on color alone to convey information
- Sale items have "SALE" text labels in addition to red color
- In-stock status includes text, not just green indicator
- Form errors have icons and text descriptions
- Rating stars include numeric rating

---

## Summary

Target's design system embodies modern retail excellence through:

1. **Iconic Branding** - The unmistakable Target Red and bullseye create instant recognition
2. **Clean Simplicity** - White space and organized layouts make shopping effortless
3. **Clear Hierarchy** - Bold typography and strategic color use guide the eye
4. **Trust Signals** - Consistent badges for delivery options, Circle savings, and ratings
5. **Inclusive Design** - Accessible to all guests regardless of ability
6. **Mobile-First** - Responsive design optimized for any device
7. **Performance** - Efficient, fast-loading interface for seamless shopping

The design system supports Target's goal of making every guest feel welcome while delivering an intuitive, enjoyable shopping experience that builds loyalty and trust.
