# Duolingo Design System

> Playful learning with high-energy brand character. Duolingo's current public presence pairs a white app-like foundation with vivid green brand accents, rounded illustration-driven UI, bold friendly typography, and gamified feedback that keeps education feeling light, motivating, and immediately readable.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Duolingo feels like **education designed as a habit-forming game**. The interface is bright, rounded, and character-led, but still highly structured. Progress, rewards, mascot energy, and low-friction calls to action all work together to make learning feel approachable.

### Mood & Feeling
- Playful and encouraging
- Bright, optimistic, and energetic
- Game-like without becoming visually chaotic
- Friendly enough for kids, polished enough for adults
- Clear and habit-forming

### Design Density
**Medium density.** Duolingo shows lots of progress states, buttons, icons, and rewards, but the system stays readable by using bold hierarchy, big controls, and generous spacing between interactive clusters.

### Visual Character
- White and very light gray surfaces with vivid green anchors
- Rounded buttons, cards, and progress modules
- Strong mascot and character support
- App-first composition with obvious progression and rewards
- Cheerful illustration language with large touch-friendly controls

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--duo-green` | `#58CC02` | Primary brand and CTA color |
| `--duo-green-deep` | `#46A302` | Hover, active, and depth layer |
| `--duo-green-soft` | `#D7FFB8` | Highlight fill and success tint |
| `--duo-white` | `#FFFFFF` | Main canvas and cards |
| `--duo-surface` | `#F7F7F7` | App background and section support |

### Support Palette

| Token | Hex | Role |
|-------|-----|------|
| `--duo-ink` | `#4B4B4B` | Primary text |
| `--duo-muted` | `#777777` | Secondary labels and helper copy |
| `--duo-blue` | `#1CB0F6` | Secondary action, XP/progress accent |
| `--duo-yellow` | `#FFD900` | Reward, streak, and celebratory accent |
| `--duo-red` | `#FF4B4B` | Mistake or warning state |

### Utility and Structure

| Token | Hex | Role |
|-------|-----|------|
| `--duo-border` | `#E5E5E5` | Card outlines and separators |
| `--duo-shadow` | `#D7D7D7` | Pressed control depth |
| `--duo-focus` | `#84D8FF` | Focus ring tint |
| `--duo-purple` | `#CE82FF` | Streak/reward support accent |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "din-round", "Nunito", "Avenir Next Rounded", sans-serif;
--font-sans: "din-round", "Nunito", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 64px | 700 | 1.02 | -0.02em | `#58CC02` |
| Page Title | 44px | 700 | 1.08 | -0.015em | `#4B4B4B` |
| Section Title | 32px | 700 | 1.14 | -0.01em | `#4B4B4B` |
| Card Title | 22px | 700 | 1.2 | 0 | `#4B4B4B` |
| Body Large | 18px | 700 | 1.5 | 0 | `#4B4B4B` |
| Body | 16px | 700 | 1.45 | 0 | `#4B4B4B` |
| Small Body | 14px | 700 | 1.4 | 0 | `#777777` |
| Label | 12px | 700 | 1.3 | 0.04em | `#777777` |

### Typography Philosophy
Duolingo typography should feel **friendly, chunky, and instantly legible**. It is allowed to be playful, but never messy. Large rounded letterforms support the habit-building, game-like tone.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #58cc02;
  color: #ffffff;
  border: none;
  border-bottom: 4px solid #46a302;
  border-radius: 16px;
  min-height: 50px;
  padding: 0 20px;
  font-size: 16px;
  font-weight: 700;
  text-transform: uppercase;
}

.button-primary:hover {
  filter: brightness(1.03);
}

.button-secondary {
  background: #ffffff;
  color: #58cc02;
  border: 2px solid #e5e5e5;
  border-bottom-width: 4px;
  border-radius: 16px;
  min-height: 50px;
  padding: 0 20px;
}
```

### Cards and Progress Modules

```css
.lesson-card {
  background: #ffffff;
  border: 2px solid #e5e5e5;
  border-radius: 24px;
  box-shadow: 0 6px 0 #d7d7d7;
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #4b4b4b;
  border: 2px solid #e5e5e5;
  border-radius: 16px;
  min-height: 48px;
  padding: 12px 14px;
}

.input:focus {
  outline: none;
  border-color: #1cb0f6;
  box-shadow: 0 0 0 4px rgba(132, 216, 255, 0.35);
}
```

### Component Notes
- Buttons should feel pressable and toy-like, not flat
- Rewards, streaks, and progress indicators deserve strong color and shape clarity
- Character art can be prominent, but should support the learning path rather than distract from it

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight icon spacing |
| `--space-3` | `8px` | Small gaps |
| `--space-4` | `12px` | Control padding |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card interior spacing |
| `--space-7` | `32px` | Section grouping |
| `--space-8` | `48px` | Large app modules |
| `--space-9` | `64px` | Hero or campaign spacing |
| `--space-10` | `96px` | Major marketing sections |

### Layout Behavior
- Organize around obvious progression, rewards, and next actions
- Prefer stacked, app-like lanes over abstract marketing grids
- Keep supporting copy short and action-oriented
- Use mascot or character art to punctuate sections, not flood them

### Whitespace Philosophy
Whitespace should feel **energetic but controlled**, leaving enough room for game elements and mascot personality without turning the screen into visual noise.

---

## 6. Depth & Elevation

### Elevation Strategy
Duolingo uses **cartoon-physical depth**. Instead of airy SaaS shadows, components often feel pressed, stacked, or extruded with clear bottom edges.

```css
--shadow-soft: 0 2px 0 #d7d7d7;
--shadow-card: 0 6px 0 #d7d7d7;
--shadow-focus: 0 0 0 4px rgba(132, 216, 255, 0.35);
```

### Surface Hierarchy
- White primary canvas
- Light gray support surfaces
- Raised white cards with hard-edged bottom depth
- Green primary actions and bright progress accents

---

## 7. Do's and Don'ts

### Do
- Keep the experience cheerful, motivational, and crystal clear
- Use rounded shapes and bright accent colors with discipline
- Make progress and rewards instantly understandable
- Preserve the app-like feeling even on marketing pages

### Don't
- Do not make Duolingo feel sterile or enterprise-heavy
- Do not replace bold, chunky controls with thin minimalist UI
- Do not darken the palette so much that the playful tone disappears
- Do not let character art overpower the learning flow

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Single-column lesson flow, large stacked buttons, oversized touch targets |
| Tablet | `768px - 1023px` | Two-column promo or feature rows, roomy progress modules |
| Desktop | `1024px+` | Wide marketing hero with app previews and mascot support |

### Responsive Rules
- Keep buttons tall and easy to tap on every breakpoint
- Preserve progress visibility before adding extra decorative content
- Stack lesson and reward modules instead of shrinking controls too far
- Maintain strong contrast between primary green actions and neutral surfaces

---

## 9. Agent Prompt Guide

### Quick Reference
- White app-like foundation with vivid green primary actions
- Rounded, chunky controls with clear pressed depth
- Friendly rounded typography and short motivational copy
- Bright reward accents, mascot energy, and game-like progress framing

### Prompt Template
```text
Design this like Duolingo's current public product and brand style:
- white and light-gray surfaces with vivid green primary actions
- rounded, chunky, highly touch-friendly buttons and cards
- playful but structured app-like layout with progress and rewards
- bold friendly typography and cheerful character-driven energy
- motivating, habit-forming education product feel
```
