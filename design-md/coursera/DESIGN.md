# Coursera Design System

> Online learning with marketplace breadth, academic trust, and blue-led clarity. Coursera's public site uses a clean sans system, white and pale-blue surfaces, structured category browsing, and strong Coursera blue (`#0056D2`) to organize courses, certificates, degrees, and career pathways.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Coursera feels like **digital education presented through a structured, trustworthy marketplace interface**. It combines academic credibility, catalog breadth, and career-oriented conversion in a bright, orderly system.

### Mood & Feeling
- Educational and trustworthy
- Career-focused and structured
- Mainstream, accessible, and global
- Marketplace-clear rather than boutique
- Supportive and progression-oriented

### Design Density
**Medium to high density.** Coursera surfaces contain many categories, partners, and program types, but strong modular sections and familiar blue cues keep the experience navigable.

### Visual Character
- White base with blue trust signals
- Partner logos and course categories as key browsing tools
- Card-based pathways for certificates and collections
- Clean educational-marketplace structure
- Friendly but not playful academic tone

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--coursera-blue` | `#0056D2` | Primary brand, CTA, and links |
| `--coursera-blue-deep` | `#003E9A` | Stronger interaction or heading accent |
| `--coursera-white` | `#FFFFFF` | Main surface and cards |
| `--coursera-surface` | `#F5F8FF` | Soft support background |
| `--coursera-ink` | `#1F1F1F` | Primary text |

### Support and Utility

| Token | Hex | Role |
|-------|-----|------|
| `--coursera-muted` | `#6B7280` | Secondary copy |
| `--coursera-border` | `#D9E3F5` | Card edges and dividers |
| `--coursera-success` | `#16825D` | Positive learning/progress state |
| `--coursera-warm` | `#FFF0D9` | Promo support surface |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Source Sans 3", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Source Sans 3", "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 54px | 700 | 1.06 | -0.02em | `#1F1F1F` |
| Page Title | 40px | 700 | 1.1 | -0.02em | `#1F1F1F` |
| Section Title | 30px | 700 | 1.14 | -0.01em | `#1F1F1F` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#1F1F1F` |
| Body Large | 18px | 400 | 1.6 | 0 | `#1F1F1F` |
| Body | 16px | 400 | 1.6 | 0 | `#1F1F1F` |
| Small Body | 14px | 400 | 1.5 | 0 | `#6B7280` |
| Label | 12px | 700 | 1.35 | 0.04em | `#6B7280` |

### Typography Philosophy
Coursera typography should feel **academic, accessible, and conversion-friendly**. It should support catalog exploration, educational trust, and career progression.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #0056d2;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #0045ab;
}

.button-secondary {
  background: #ffffff;
  color: #1f1f1f;
  border: 1px solid #d9e3f5;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Course and Program Cards

```css
.program-card {
  background: #ffffff;
  border: 1px solid #d9e3f5;
  border-radius: 20px;
  box-shadow: 0 10px 24px rgba(0, 86, 210, 0.05);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #1f1f1f;
  border: 1px solid #d9e3f5;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 16px;
}
```

### Component Notes
- Partner logos and educational credibility cues should stay prominent
- Course collections and professional certificates need strong modular framing
- Blue is the main orientation and trust color

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Dense metadata alignment |
| `--space-3` | `8px` | Small gaps |
| `--space-4` | `12px` | Compact spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card spacing |
| `--space-7` | `32px` | Category separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and category-browse rhythm |

### Layout Behavior
- Organize by goals: career, skills, degree, certificate, collection
- Use partner logos as a major trust and discovery tool
- Keep educational-marketplace flows clear and familiar
- Let promotions and collections stay distinct from evergreen catalog browsing

### Whitespace Philosophy
Whitespace should feel **structured and educational**, helping a very large course marketplace remain approachable.

---

## 6. Depth & Elevation

### Elevation Strategy
Coursera uses **light marketplace elevation** with clear program cards and soft blue support bands.

```css
--shadow-soft: 0 8px 18px rgba(0, 86, 210, 0.04);
--shadow-card: 0 14px 28px rgba(0, 86, 210, 0.08);
```

### Surface Hierarchy
- White base
- Soft blue support backgrounds
- Program and collection cards
- Blue used for trust, navigation, and action

---

## 7. Do's and Don'ts

### Do
- Keep the system clear, educational, and trustworthy
- Use blue to organize action and navigation
- Preserve partner and credential credibility cues
- Make large category systems easy to browse

### Don't
- Do not turn Coursera into a playful consumer-ed app
- Do not bury educational trust signals under aggressive promotions
- Do not overcomplicate the browsing hierarchy
- Do not reduce the clarity of course/program cards with unnecessary decoration

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked learning pathways and simplified category rails |
| Tablet | `768px - 1023px` | Wider course cards and compact logo/category sections |
| Desktop | `1024px+` | Full educational-marketplace browsing with broad category and partner layouts |

### Responsive Rules
- Keep the primary goal-selection flow obvious on mobile
- Preserve readable category and collection cards
- Stack broad educational catalog sections before shrinking them too far
- Maintain strong visual separation between courses, collections, and promotions

---

## 9. Agent Prompt Guide

### Quick Reference
- White and soft-blue online-learning marketplace foundation
- Coursera blue for trust, CTAs, and navigation
- Program cards, partner logos, category rails, and clear educational hierarchy
- Academic trust with career-oriented clarity

### Prompt Template
```text
Design this like Coursera's current public website:
- white and soft-blue online-learning marketplace foundation
- strong Coursera-blue navigation and CTA system
- program cards, partner logos, and category browsing with clear educational hierarchy
- academic trust plus career-focused conversion cues
- structured, mainstream, highly legible learning-platform UX
```
