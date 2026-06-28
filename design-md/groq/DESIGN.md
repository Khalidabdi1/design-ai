# Groq Design System

> AI inference design with electric orange identity, speed-first surfaces, token-throughput clarity, and developer-performance UX.

---

## 1. Visual Theme & Atmosphere

Groq should feel blazingly fast, technical, and powerful. The design language communicates LPU inference speed, low-latency API performance, developer tooling, and the competitive advantage of tokens-per-second.

- Mood: fast, technical, powerful, confident
- Density: medium, with API playground, benchmark comparisons, and performance dashboards
- Character: electric orange brand, near-black performance surfaces, speed-metric highlights, mono API panels

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--groq-orange` | `#F55036` | Primary brand CTA and speed highlight |
| `--groq-orange-dark` | `#D03E28` | Hover and active states |
| `--groq-black` | `#0A0A0A` | Primary dark surface |
| `--groq-gray` | `#1A1A1A` | Secondary dark panel |
| `--groq-green` | `#22C55E` | API success and healthy endpoint |
| `--groq-amber` | `#F59E0B` | Rate limit warning |
| `--groq-red` | `#EF4444` | API error and endpoint failure |
| `--surface-card` | `#FFFFFF` | Light content and pricing cards |
| `--surface-bg` | `#F9FAFB` | Light dashboard background |
| `--surface-dark` | `#0A0A0A` | Hero and playground surfaces |
| `--text-light` | `#FFFFFF` | Text on dark surfaces |
| `--text-primary` | `#111827` | Text on light surfaces |
| `--border-dark` | `#2A2A2A` | Dark surface borders |

Orange is the signature speed signal — use it for primary CTAs and speed-metric highlights. The dark surface is the primary visual statement for the brand.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-display: "Space Grotesk", Inter, sans-serif;
--font-mono: "JetBrains Mono", "Fira Code", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Hero Display | 72px | 800 | 0.95 |
| Page Title | 44px | 700 | 1.05 |
| Section Title | 28px | 600 | 1.2 |
| Metric Value | 48px | 800 | 1.0 |
| Body | 16px | 400 | 1.65 |
| Code | 14px | 400 | 1.7 |
| Label | 12px | 600 | 1.35 |

Use heavy weight (700-800) for performance metrics and hero display — Groq's identity is built on impressive numbers.

## 4. Component Stylings

```css
.button-primary {
  min-height: 44px;
  padding: 0 22px;
  border: none;
  border-radius: 8px;
  background: #F55036;
  color: #FFFFFF;
  font: 700 15px/1 Inter, sans-serif;
}

.speed-metric {
  font: 800 48px/1 "Space Grotesk", sans-serif;
  color: #F55036;
}

.api-panel {
  border-radius: 12px;
  background: #1A1A1A;
  border: 1px solid #2A2A2A;
  padding: 20px 24px;
  font: 400 13px/1.7 "JetBrains Mono", monospace;
  color: #E5E7EB;
}

.model-card {
  border: 1px solid #2A2A2A;
  border-radius: 12px;
  background: #1A1A1A;
  color: #FFFFFF;
  padding: 20px;
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-4` | `16px` | Card rhythm |
| `--space-6` | `24px` | Section padding |
| `--space-12` | `48px` | Major section gaps |
| `--space-20` | `80px` | Hero section padding |

Lead with speed metrics — tokens/second should be the largest number on the page. API playground takes the center. Model comparison tables below.

## 6. Depth & Elevation

```css
.shadow-card  { box-shadow: 0 0 0 1px #2A2A2A; }
.shadow-glow  { box-shadow: 0 0 40px rgba(245, 80, 54, 0.20); }
.shadow-modal { box-shadow: 0 20px 60px rgba(0, 0, 0, 0.60); }
```

On dark surfaces, use a subtle orange glow for the primary metric card to signal speed and performance.

## 7. Do's and Don'ts

Do make tokens/second the hero number on the homepage. Do use mono font in all API examples and response panels. Do use dark surfaces as the default — light mode is secondary. Do not use orange for error states. Do not understate the speed advantage — it is the entire product differentiation.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | Speed metric hero, API docs reference |
| Tablet | `768px` | Two-column model comparison, basic playground |
| Desktop | `1200px` | Full playground, model cards, benchmarks, and API explorer |

The API playground is desktop-primary. Mobile is for documentation reading.

## 9. Agent Prompt Guide

Design like Groq: electric orange CTAs, near-black dark surfaces, heavy-weight speed metrics, mono API panels, orange glow accents, tokens-per-second hero numbers, and performance-first inference hierarchy.
