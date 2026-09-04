# WhatsApp Design System

> Utilitarian, trustworthy messaging built for speed and clarity. WhatsApp's public product pairs a calm green-and-white identity with a chat-bubble-first layout, dense contact lists, and no-frills controls that prioritize legibility and reliability over decoration.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
WhatsApp feels like **a plain, dependable notebook for conversations**. The interface avoids ornamentation almost entirely: flat panels, clear bubbles, and a single confident green accent carry the entire brand identity.

### Mood & Feeling
- Calm, private, and trustworthy
- Efficient and utilitarian
- Warm but restrained (green accent, not a saturated wash)
- Familiar and low-friction across every screen
- Function over flourish

### Design Density
**High density in lists, low density in conversation view.** Chat lists pack many rows tightly; the conversation screen itself stays sparse, giving bubbles room to breathe against a textured background.

### Visual Character
- White/near-white panels in light mode, deep charcoal (`#111B21`) in dark mode
- Signature green (`#25D366`) reserved for primary actions and sent-message bubbles
- Subtle doodle-pattern wallpaper behind chat bubbles
- Rounded chat bubbles with small tail accents
- Circular avatars and simple line icons throughout

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--wa-green` | `#25D366` | Primary brand accent, FAB, online indicator |
| `--wa-teal-dark` | `#075E54` | Header bar, brand anchor (legacy/marketing) |
| `--wa-teal` | `#128C7E` | Secondary brand accent |
| `--wa-white` | `#FFFFFF` | Light-mode surface |
| `--wa-panel-dark` | `#111B21` | Dark-mode base surface |

### Chat Bubble Colors

| Token | Hex | Role |
|-------|-----|------|
| `--wa-bubble-sent` | `#DCF8C6` | Sent message bubble (light mode) |
| `--wa-bubble-sent-dark` | `#005C4B` | Sent message bubble (dark mode) |
| `--wa-bubble-received` | `#FFFFFF` | Received message bubble (light mode) |
| `--wa-bubble-received-dark` | `#202C33` | Received message bubble (dark mode) |
| `--wa-check-blue` | `#34B7F1` | Read-receipt double-check accent |

### Support Palette

| Token | Hex | Role |
|-------|-----|------|
| `--wa-ink` | `#111B21` | Primary text (light mode) |
| `--wa-muted` | `#667781` | Secondary text, timestamps, status |
| `--wa-border` | `#E9EDEF` | Dividers between list rows |
| `--wa-background` | `#F0F2F5` | App chrome background |

---

## 3. Typography Rules

### Font Stack

```css
--font-sans: "Segoe UI", Helvetica, Arial, sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Screen Title | 19px | 600 | 1.3 | 0 | `#111B21` |
| Contact Name | 17px | 500 | 1.3 | 0 | `#111B21` |
| Message Text | 14.2px | 400 | 1.35 | 0 | `#111B21` |
| List Preview | 14px | 400 | 1.3 | 0 | `#667781` |
| Timestamp | 12px | 400 | 1.2 | 0 | `#667781` |
| Button Label | 16px | 500 | 1.2 | 0 | `#25D366` |

### Typography Philosophy
Type should be **plain, legible, and system-native** — no display fonts, no decorative weights. Hierarchy comes from size and color contrast, not typographic style.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #25d366;
  color: #ffffff;
  border: none;
  border-radius: 24px;
  min-height: 40px;
  padding: 0 24px;
  font-size: 14px;
  font-weight: 500;
}

.fab-button {
  width: 56px;
  height: 56px;
  border-radius: 50%;
  background: #25d366;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.25);
}
```

### Chat Bubbles

```css
.bubble-sent {
  background: #dcf8c6;
  border-radius: 8px 0 8px 8px;
  padding: 6px 8px 8px 8px;
  max-width: 65%;
}

.bubble-received {
  background: #ffffff;
  border-radius: 0 8px 8px 8px;
  padding: 6px 8px 8px 8px;
  max-width: 65%;
  box-shadow: 0 1px 0.5px rgba(0, 0, 0, 0.08);
}
```

### List Row

```css
.chat-list-row {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 16px;
  border-bottom: 1px solid #e9edef;
}
```

### Component Notes
- Sent and received bubbles must always be visually distinct by alignment and color
- The floating action button (FAB) is reserved for the primary "new chat/call" action
- Read receipts use double-check glyphs; blue only once read

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-1` | `4px` | Icon-to-text gaps |
| `--space-2` | `8px` | Bubble internal padding |
| `--space-3` | `12px` | List row gaps |
| `--space-4` | `16px` | Screen edge padding |
| `--space-5` | `24px` | Section separation |

### Layout Behavior
- Three-pane structure on desktop/web: chat list, active conversation, contact/group info
- Mobile collapses to a single-pane stack navigated by push/pop transitions
- Chat lists prioritize name, preview text, and timestamp in a fixed three-column row
- Conversation view scrolls bottom-anchored with bubbles growing upward

### Whitespace Philosophy
Whitespace is **functional, not aesthetic** — just enough padding to keep dense lists and bubble stacks legible without wasting screen space.

---

## 6. Depth & Elevation

### Elevation Strategy
WhatsApp uses **minimal, functional elevation** — flat lists and headers, with soft shadows reserved for floating buttons and bubble tails.

```css
--shadow-bubble: 0 1px 0.5px rgba(0, 0, 0, 0.08);
--shadow-fab: 0 2px 6px rgba(0, 0, 0, 0.25);
--shadow-header: 0 1px 2px rgba(0, 0, 0, 0.1);
```

### Surface Hierarchy
- Flat background wallpaper behind conversation
- Slightly elevated bubbles with directional tails
- Floating action button as the highest-elevation element on a screen

---

## 7. Do's and Don'ts

### Do
- Keep the green accent confined to actions, indicators, and sent bubbles
- Maintain clear visual separation between sent and received messages
- Use plain system typography with strong size/color hierarchy
- Preserve dense, scannable list rows for chats and contacts

### Don't
- Do not saturate large surfaces in green or teal
- Do not add decorative shadows or gradients to bubbles
- Do not mix bubble alignment (sent should always be one side, received the other)
- Do not introduce display fonts or heavy custom typography

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Single-pane stack navigation, full-width chat list and conversation |
| Tablet | `768px - 1023px` | Two-pane layout: chat list + active conversation |
| Desktop | `1024px+` | Three-pane layout: chat list, conversation, contact/group info panel |

### Responsive Rules
- Bubble max-width stays around 65% of the conversation column at every size
- Chat list rows keep name, preview, and timestamp aligned regardless of width
- Touch targets (list rows, buttons) stay at least 44px tall on mobile
- Info/detail panel is dismissible on tablet, persistent on desktop

---

## 9. Agent Prompt Guide

### Quick Reference
- Calm white/charcoal surfaces with a single confident green accent
- Rounded chat bubbles with directional tails, distinct sent/received styling
- Dense, scannable chat lists paired with a sparse conversation view
- Plain system typography, minimal shadows, functional over decorative

### Prompt Template
```text
Design this like WhatsApp's current public product and brand style:
- calm white (or dark charcoal) surfaces with a single green brand accent
- rounded chat bubbles with clear sent/received distinction and tail accents
- dense, scannable chat list rows next to a sparse conversation view
- plain system typography, minimal shadows, utilitarian and trustworthy tone
```
