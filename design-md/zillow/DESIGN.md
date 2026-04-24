# Zillow Design System

> Real-estate discovery with high-trust search flows and map-driven clarity. Zillow's public site uses a white and soft-blue foundation, dark text, large search-led hero areas, and the strong Zillow blue (`#006AFF`) to anchor rentals, homes, agents, and loans.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Zillow feels like **property discovery translated into a trust-heavy search interface**. The system balances marketplace breadth, map/search functionality, and consumer-finance seriousness with a bright, approachable frame.

### Mood & Feeling
- Helpful and trustworthy
- Search-first and goal-oriented
- Marketplace-clear rather than editorially luxurious
- Consumer-friendly but serious
- Home discovery with financial credibility

### Design Density
**Medium density.** Zillow surfaces carry many navigation options, but the search-led structure keeps the hierarchy obvious.

### Visual Character
- Blue-led trust signals
- White cards and soft support surfaces
- Search bars, recommendations, and property modules
- Image-led listing previews and marketplace flows
- Calm, mainstream digital real-estate energy

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--zillow-blue` | `#006AFF` | Primary brand and CTA blue |
| `--zillow-blue-deep` | `#0F4AA1` | Darker support blue |
| `--zillow-white` | `#FFFFFF` | Main canvas and cards |
| `--zillow-surface` | `#F5F8FF` | Soft background tint |
| `--zillow-ink` | `#1B1F23` | Primary text |

### Support and Utility

| Token | Hex | Role |
|-------|-----|------|
| `--zillow-muted` | `#69707A` | Secondary text |
| `--zillow-border` | `#DCE5F5` | Divider and card edge |
| `--zillow-success` | `#16825D` | Positive state |
| `--zillow-warning` | `#A76014` | Attention state |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Zillow Sans", "Open Sans", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Zillow Sans", "Open Sans", "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 52px | 700 | 1.06 | -0.02em | `#1B1F23` |
| Page Title | 40px | 700 | 1.1 | -0.02em | `#1B1F23` |
| Section Title | 30px | 700 | 1.14 | -0.01em | `#1B1F23` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#1B1F23` |
| Body Large | 18px | 400 | 1.6 | 0 | `#1B1F23` |
| Body | 16px | 400 | 1.6 | 0 | `#1B1F23` |
| Small Body | 14px | 400 | 1.5 | 0 | `#69707A` |
| Label | 12px | 700 | 1.35 | 0.04em | `#69707A` |

### Typography Philosophy
Zillow typography should feel **reliable, consumer-readable, and search-friendly**. It should make property and loan workflows feel easy to trust.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #006aff;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #0058d6;
}

.button-secondary {
  background: #ffffff;
  color: #1b1f23;
  border: 1px solid #dce5f5;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Search and Listing Cards

```css
.listing-card {
  background: #ffffff;
  border: 1px solid #dce5f5;
  border-radius: 20px;
  box-shadow: 0 12px 26px rgba(15, 74, 161, 0.06);
}

.search-shell {
  background: #ffffff;
  border: 1px solid #dce5f5;
  border-radius: 999px;
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #1b1f23;
  border: 1px solid #dce5f5;
  border-radius: 999px;
  min-height: 48px;
  padding: 0 16px;
}
```

### Component Notes
- Search should remain the strongest product affordance
- Listings and recommendations need trust-forward framing
- Blue should guide action and orientation more than decoration

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Dense metadata alignment |
| `--space-3` | `8px` | Small gaps |
| `--space-4` | `12px` | Compact internal spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card spacing |
| `--space-7` | `32px` | Search/results separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Search-led hero rhythm |

### Layout Behavior
- Lead with search and clear housing goals
- Use cards and recommendations to keep browsing guided
- Balance listings, loans, rentals, and agents without losing clarity
- Keep visual structure mainstream and trustworthy

### Whitespace Philosophy
Whitespace should feel **calm and search-supportive**, helping large real-estate content sets remain easy to navigate.

---

## 6. Depth & Elevation

### Elevation Strategy
Zillow uses **light consumer-marketplace elevation** with rounded search shells and listing cards.

```css
--shadow-soft: 0 8px 18px rgba(15, 74, 161, 0.05);
--shadow-card: 0 16px 30px rgba(15, 74, 161, 0.08);
```

### Surface Hierarchy
- White base
- Soft blue support bands
- Search shell and listing card elevation
- Blue used for action, links, and trust

---

## 7. Do's and Don'ts

### Do
- Keep search and discovery central
- Use blue to reinforce trust and action
- Preserve mainstream readability and marketplace clarity
- Make property browsing feel guided and low-friction

### Don't
- Do not turn Zillow into luxury real-estate editorial
- Do not bury search under decorative hero content
- Do not make listing cards visually noisy
- Do not overcomplicate the trust signals around loans, agents, and rentals

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Search-first stacked layout and vertical listing cards |
| Tablet | `768px - 1023px` | Wider search, compact recommendation grids |
| Desktop | `1024px+` | Full property-discovery flows and broad category navigation |

### Responsive Rules
- Keep search prominent and easy to use on mobile
- Preserve readable listing cards and image thumbnails
- Stack recommendation and utility modules before compressing them
- Maintain strong CTA clarity in finance-related flows

---

## 9. Agent Prompt Guide

### Quick Reference
- White and soft-blue real-estate marketplace foundation
- Zillow-blue search and CTA anchors
- Rounded search shells, listing cards, and mainstream trust-heavy layout
- Search-first, helpful, and consumer-finance credible

### Prompt Template
```text
Design this like Zillow's current public website:
- white and soft-blue real-estate marketplace foundation
- Zillow-blue search and CTA anchors with strong trust cues
- rounded search shells and listing-card layouts
- consumer-friendly property discovery with loan, rental, and agent clarity
- guided, reliable, search-first UX over luxury editorial styling
```
