# Cursor Design System

> AI code editor design with deep navy identity, editor-first surfaces, agent-panel clarity, and AI-native coding UX.

---

## 1. Visual Theme & Atmosphere

Cursor should feel fast, intelligent, and editor-native. The design language communicates AI code completion, multi-file edits, natural-language coding, and an IDE that thinks alongside the developer.

- Mood: fast, intelligent, focused, developer-native
- Density: high, with editor panes, AI chat panels, diff views, and file trees
- Character: deep navy editor surface, subtle blue AI accents, minimal chrome, code-first aesthetic

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--cur-blue` | `#5B9EF5` | Primary AI accent and CTA |
| `--cur-blue-dark` | `#3D82E0` | Hover and active states |
| `--cur-bg` | `#0E1117` | Primary editor background |
| `--cur-panel` | `#161B27` | Sidebar and panel background |
| `--cur-border` | `#2A3042` | Editor and panel borders |
| `--cur-green` | `#4ADE80` | Accept suggestion and success |
| `--cur-red` | `#F87171` | Reject suggestion and diff removed |
| `--cur-amber` | `#FBBF24` | Warning and lint highlight |
| `--cur-purple` | `#A78BFA` | Agent mode and multi-file edit |
| `--text-primary` | `#E2E8F0` | Code and primary UI text |
| `--text-secondary` | `#8892A4` | Comments and secondary labels |
| `--text-dim` | `#4A5568` | Inactive tabs and dim UI |

Blue is the AI accent — it signals AI-generated content and active suggestions. Purple is reserved for Agent mode (multi-step autonomous edits) only.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-mono: "Fira Code", "JetBrains Mono", "Cascadia Code", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Editor Code | 14px | 400 | 1.6 |
| Chat Message | 14px | 400 | 1.65 |
| File Name | 13px | 500 | 1.3 |
| Panel Title | 13px | 600 | 1.3 |
| Breadcrumb | 12px | 400 | 1.4 |
| Label | 11px | 600 | 1.35 |
| Keybinding | 11px | 400 | 1.3 |

## 4. Component Stylings

```css
.button-primary {
  min-height: 32px;
  padding: 0 14px;
  border: none;
  border-radius: 6px;
  background: #5B9EF5;
  color: #0E1117;
  font: 600 13px/1 Inter, sans-serif;
}

.ai-suggestion {
  background: rgba(91, 158, 245, 0.08);
  border-left: 2px solid #5B9EF5;
  color: #8892A4;
  font: 400 14px/1.6 "Fira Code", monospace;
  padding-left: 8px;
}

.chat-bubble-ai {
  border-radius: 12px 12px 12px 4px;
  background: #161B27;
  border: 1px solid #2A3042;
  color: #E2E8F0;
  padding: 12px 16px;
  font: 400 14px/1.65 Inter, sans-serif;
}

.diff-added   { background: rgba(74, 222, 128, 0.10); border-left: 2px solid #4ADE80; }
.diff-removed { background: rgba(248, 113, 113, 0.10); border-left: 2px solid #F87171; }

.tab-active {
  background: #0E1117;
  border-bottom: 2px solid #5B9EF5;
  color: #E2E8F0;
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-1` | `4px` | Editor gutter padding |
| `--space-2` | `8px` | Sidebar item padding |
| `--space-3` | `12px` | Panel section rhythm |
| `--space-6` | `24px` | Chat message spacing |

Editor takes 60–70% of the viewport. AI chat panel on the right (collapsible). File tree on the left (collapsible). No persistent top menu bar — actions live in the command palette.

## 6. Depth & Elevation

```css
.shadow-panel   { box-shadow: 0 0 0 1px #2A3042; }
.shadow-tooltip { box-shadow: 0 4px 16px rgba(0, 0, 0, 0.40); }
.shadow-modal   { box-shadow: 0 20px 50px rgba(0, 0, 0, 0.50); }
```

On dark surfaces, borders replace shadows. Use `box-shadow: 0 0 0 1px` as the elevation primitive for panels and menus.

## 7. Do's and Don'ts

Do use blue to visually distinguish AI-generated content from user-written code. Do use purple only for Agent mode — it signals multi-step autonomous edits. Do keep the editor surface completely dark with minimal chrome. Do not use light backgrounds anywhere in the editor UI. Do not show AI suggestions in a color that resembles syntax highlighting.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | Not applicable — Cursor is a desktop application |
| Tablet | `768px` | Simplified two-panel: editor + collapsed AI |
| Desktop | `1200px` | Full layout: file tree + editor + AI chat panel |

Cursor is a desktop-first application. All layouts optimize for large screens.

## 9. Agent Prompt Guide

Design like Cursor: deep navy editor surfaces, blue AI suggestion highlights, purple agent-mode accent, inline diff colors, mono code font, minimal chrome, command-palette-first navigation, and AI-native coding hierarchy.
