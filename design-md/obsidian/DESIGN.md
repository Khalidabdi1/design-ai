# Obsidian Design System
> Markdown knowledge base with a dark, graph-centric aesthetic — deep charcoal surfaces, amethyst purple accents, and linked-thought-first UI.

---

## 1. Visual Theme & Atmosphere
Obsidian is a second brain in a dark, minimal interface. The app is deeply customizable but its default aesthetic is dark and focused: charcoal surfaces that disappear around markdown text, a purple accent that marks links and connections, and a graph view that turns notes into a constellation of knowledge. The UI stays out of the way, treating the editor as sacred space.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#7C6DF5` | Brand amethyst, links, CTAs |
| `--color-primary-dark` | `#6354D0` | Hover/active |
| `--color-primary-dim` | `rgba(124,109,245,0.15)` | Highlight backgrounds |
| `--color-bg-base` | `#1E1E1E` | App background |
| `--color-bg-sidebar` | `#252525` | Left file pane |
| `--color-bg-editor` | `#1E1E1E` | Editor area |
| `--color-bg-elevated` | `#2D2D2D` | Modals, command palette |
| `--color-border` | `#383838` | Default borders |
| `--color-text-primary` | `#DCDDDE` | Headings, body text |
| `--color-text-secondary` | `#888888` | File names, meta |
| `--color-text-muted` | `#555555` | Placeholders, hints |
| `--color-link` | `#7C6DF5` | [[wiki links]] |
| `--color-link-unresolved` | `rgba(124,109,245,0.5)` | Unresolved links |
| `--color-tag` | `#E6A817` | #tags in notes |
| `--color-heading-1` | `#C678DD` | H1 color |
| `--color-heading-2` | `#61AFEF` | H2 color |
| `--color-code-bg` | `#282C34` | Inline code background |
| `--color-graph-node` | `#7C6DF5` | Graph view node color |
| `--color-graph-edge` | `#454545` | Graph edge lines |

## 3. Typography Rules
```css
--font-text: 'Inter', -apple-system, sans-serif;
--font-monospace: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 16px;
--font-size-md: 18px;
--font-size-lg: 22px;
--font-size-xl: 26px;
--font-size-h1: 26px;
--font-size-h2: 22px;
--font-size-h3: 18px;
--font-weight-regular: 400;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.3;
--line-height-base: 1.6;
--line-height-editor: 1.75;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| H1 | 26px | 700 | 1.3 |
| H2 | 22px | 600 | 1.35 |
| H3 | 18px | 600 | 1.4 |
| Body / Editor | 16px | 400 | 1.75 |
| File Name | 13px | 400 | 1.4 |
| Code | 14px | 400 | 1.6 |

## 4. Component Stylings
```css
/* Editor Area */
.editor {
  padding: 40px 80px;
  max-width: 750px;
  margin: 0 auto;
  font-size: 16px;
  line-height: 1.75;
  color: #DCDDDE;
}

/* Wiki Link */
.wiki-link {
  color: #7C6DF5;
  text-decoration: none;
  background: rgba(124,109,245,0.08);
  border-radius: 3px;
  padding: 0 2px;
}
.wiki-link:hover { background: rgba(124,109,245,0.18); }
.wiki-link--unresolved { color: rgba(124,109,245,0.5); }

/* Tag */
.tag {
  color: #E6A817;
  font-size: 0.9em;
  text-decoration: none;
}
.tag:hover { text-decoration: underline; }

/* Inline Code */
.inline-code {
  background: #282C34;
  border-radius: 3px;
  padding: 2px 6px;
  font-family: var(--font-monospace);
  font-size: 0.9em;
  color: #E06C75;
}

/* Code Block */
.code-block {
  background: #282C34;
  border-radius: 6px;
  padding: 16px;
  font-family: var(--font-monospace);
  font-size: 14px;
  line-height: 1.6;
  border-left: 3px solid #7C6DF5;
  overflow-x: auto;
}

/* File Tree Item */
.file-item {
  display: flex;
  align-items: center;
  gap: 6px;
  padding: 4px 12px;
  border-radius: 4px;
  cursor: pointer;
  font-size: 13px;
  color: #888888;
  transition: background 0.08s, color 0.08s;
}
.file-item:hover { background: #2D2D2D; color: #DCDDDE; }
.file-item--active { background: rgba(124,109,245,0.12); color: #7C6DF5; }

/* Command Palette */
.command-palette {
  background: #2D2D2D;
  border: 1px solid #383838;
  border-radius: 10px;
  width: 560px;
  box-shadow: 0 16px 48px rgba(0,0,0,0.7);
  overflow: hidden;
}
.command-input {
  background: transparent;
  border: none;
  padding: 14px 16px;
  font-size: 15px;
  color: #DCDDDE;
  width: 100%;
}
.command-input:focus { outline: none; }
.command-result {
  padding: 8px 16px;
  font-size: 13px;
  color: #DCDDDE;
  cursor: pointer;
  display: flex;
  align-items: center;
  gap: 10px;
}
.command-result:hover,
.command-result--active { background: rgba(124,109,245,0.15); }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--editor-max-width` | `750px` | Editor content column |
| `--editor-padding` | `80px` | Horizontal editor padding |
| `--sidebar-width` | `260px` | File explorer pane |
| `--spacing-xs` | `4px` | File item gaps |
| `--spacing-sm` | `8px` | Section gaps |
| `--spacing-md` | `16px` | Panel padding |
| `--spacing-lg` | `40px` | Editor vertical padding |
| `--radius-sm` | `3px` | Inline code, wiki links |
| `--radius-md` | `6px` | Code blocks |
| `--radius-lg` | `10px` | Command palette |

## 6. Depth & Elevation
```css
.shadow-palette { box-shadow: 0 16px 48px rgba(0,0,0,0.7); }
.shadow-modal { box-shadow: 0 12px 40px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Keep the editor centered at max 750px with generous padding
- Color headings differently (H1 purple, H2 blue) for hierarchy
- Wiki links have a subtle purple background tint
- The command palette is the primary navigation — style it prominently

**Don't:**
- Don't add heavy chrome around the editor — notes need full focus
- Don't use bright accent colors for anything other than links and tags
- Don't show toolbar buttons by default — they appear on selection only

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Full-screen editor; sidebar as drawer |
| Tablet | 768px | Narrow sidebar + editor |
| Desktop | 1024px | Sidebar + editor + optional backlinks panel |
| Wide | 1440px | Three-panel or graph view visible |

## 9. Agent Prompt Guide
```
You are designing for Obsidian — a markdown knowledge base.
Use deep dark surfaces (#1E1E1E) with the editor centered at max 750px.
Amethyst purple (#7C6DF5) marks all wiki links, active file, and command palette selections.
H1 headings are colored purple, H2 blue — using CSS color per heading level.
Tags are golden-orange (#E6A817); inline code is on a dark code background.
The command palette is a floating dark modal with instant-search results.
Tone is focused, minimal, dark, and note-taking-first.
```
