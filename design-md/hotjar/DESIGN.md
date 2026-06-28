# Hotjar Design System

> Behavior analytics design with warm coral identity, heatmap visualization surfaces, session-replay clarity, and user-empathy UX.

---

## 1. Visual Theme & Atmosphere

Hotjar should feel warm, insightful, and human. The design language communicates heatmaps, session recordings, feedback surveys, user interviews, and the empathy behind understanding real user behavior.

- Mood: warm, empathetic, insightful, approachable
- Density: medium, with heatmap overlays, session replay controls, survey builders, and feedback widgets
- Character: warm coral brand, white insights surfaces, heatmap gradient (blue-to-red), human-centered messaging

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--hj-coral` | `#FF3C00` | Primary brand CTA and highlights |
| `--hj-coral-dark` | `#CC3000` | Hover and active states |
| `--hj-orange` | `#FF7A00` | Secondary brand gradient endpoint |
| `--hj-purple` | `#7C3AED` | Recordings and session replay accent |
| `--hj-green` | `#16A34A` | Positive feedback and survey success |
| `--hj-blue` | `#3B82F6` | Informational and link states |
| `--heat-cold` | `#3B82F6` | Heatmap cold zone (low activity) |
| `--heat-warm` | `#F59E0B` | Heatmap warm zone (medium activity) |
| `--heat-hot` | `#EF4444` | Heatmap hot zone (high activity) |
| `--surface-card` | `#FFFFFF` | Insight and recording cards |
| `--surface-bg` | `#FFF8F6` | Warm-tinted dashboard background |
| `--text-primary` | `#1A1A2E` | Labels and headings |
| `--border-default` | `#E5E7EB` | Card and panel borders |

The heatmap gradient (blue → yellow → red) is a signature visual. It must always use this exact progression — never reverse or alter the color order.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-mono: "JetBrains Mono", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 30px | 700 | 1.1 |
| Section Title | 22px | 600 | 1.2 |
| Card Title | 18px | 600 | 1.3 |
| Body | 15px | 400 | 1.65 |
| Survey Question | 17px | 500 | 1.5 |
| Metric Value | 32px | 700 | 1.0 |
| Label | 12px | 600 | 1.35 |

## 4. Component Stylings

```css
.button-primary {
  min-height: 42px;
  padding: 0 20px;
  border: none;
  border-radius: 8px;
  background: #FF3C00;
  color: #FFFFFF;
  font: 600 14px/1 Inter, sans-serif;
}

.recording-card {
  border: 1px solid #E5E7EB;
  border-radius: 12px;
  background: #FFFFFF;
  padding: 16px 20px;
  display: flex;
  align-items: center;
  gap: 14px;
  cursor: pointer;
}

.heatmap-overlay {
  position: absolute;
  inset: 0;
  opacity: 0.75;
  pointer-events: none;
  background: radial-gradient(circle, rgba(239,68,68,0.8) 0%, rgba(245,158,11,0.6) 40%, rgba(59,130,246,0.3) 80%);
}

.feedback-widget {
  border-radius: 999px 999px 0 0;
  background: #FF3C00;
  color: #FFFFFF;
  padding: 10px 20px;
  font: 600 14px/1 Inter, sans-serif;
  writing-mode: vertical-rl;
  transform: rotate(180deg);
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `8px` | Recording list spacing |
| `--space-4` | `16px` | Card rhythm |
| `--space-6` | `24px` | Section padding |
| `--space-10` | `40px` | Dashboard section gaps |

Dashboard leads with key metrics (recordings, heatmaps, responses). Heatmap view is full-page with a floating controls overlay. Session replay uses a bottom-anchored timeline.

## 6. Depth & Elevation

```css
.shadow-card    { box-shadow: 0 2px 8px rgba(26, 26, 46, 0.06); }
.shadow-panel   { box-shadow: 0 8px 24px rgba(255, 60, 0, 0.10); }
.shadow-modal   { box-shadow: 0 20px 52px rgba(26, 26, 46, 0.16); }
```

Recording and heatmap cards use a warm coral shadow to reinforce the brand's empathetic warmth.

## 7. Do's and Don'ts

Do always use the blue-to-red heatmap gradient in the correct order. Do make session recordings scannable with thumbnail previews. Do surface rage-click and u-turn signals prominently in recordings. Do not use coral for error states. Do not clutter the heatmap overlay with UI chrome.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | Survey responses and recording count summary |
| Tablet | `768px` | Recording list, basic heatmap view |
| Desktop | `1200px` | Full dashboard: heatmaps, recordings, surveys, funnels |

Heatmap creation and session replay require desktop. Mobile is for reviewing summaries and feedback.

## 9. Agent Prompt Guide

Design like Hotjar: warm coral CTAs, heatmap gradient (cold blue → warm amber → hot red), session-replay controls, survey builder surfaces, coral feedback widget, and user-behavior empathy hierarchy.
