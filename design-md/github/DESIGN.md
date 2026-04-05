# GitHub Primer Design System

> The official design system for building GitHub's product UI. Primer provides foundations, patterns, and components for creating consistent, accessible, and developer-focused interfaces.

**Design Philosophy:** Technical clarity meets functional minimalism. Every element serves a purpose in the developer workflow.

---

## 1. Color Palette

### Primary Brand Colors

| Color Name | Hex Code | RGB | CSS Variable | Usage |
|------------|----------|-----|--------------|-------|
| GitHub Blue | `#0969da` | rgb(9, 105, 218) | `--fgColor-accent` | Primary actions, links, focus states |
| Success Green | `#1a7f37` | rgb(26, 127, 55) | `--fgColor-success` | Open states, success, positive actions |
| Danger Red | `#d1242f` | rgb(209, 36, 47) | `--fgColor-danger` | Errors, destructive actions, closed states |
| Attention Yellow | `#9a6700` | rgb(154, 103, 0) | `--fgColor-attention` | Warnings, attention required |
| Done Purple | `#8250df` | rgb(130, 80, 223) | `--fgColor-done` | Completed states, merged PRs |
| Severe Orange | `#bc4c00` | rgb(188, 76, 0) | `--fgColor-severe` | Critical warnings |
| Sponsors Pink | `#bf3989` | rgb(191, 57, 137) | `--fgColor-sponsors` | Sponsorship, heart actions |

### Light Mode Colors

| Element | Hex Code | RGB | CSS Variable |
|---------|----------|-----|--------------|
| Background Default | `#ffffff` | rgb(255, 255, 255) | `--bgColor-default` |
| Background Muted | `#f6f8fa` | rgb(246, 248, 250) | `--bgColor-muted` |
| Background Inset | `#f6f8fa` | rgb(246, 248, 250) | `--bgColor-inset` |
| Background Emphasis | `#25292e` | rgb(37, 41, 46) | `--bgColor-emphasis` |
| Text Default | `#1f2328` | rgb(31, 35, 40) | `--fgColor-default` |
| Text Muted | `#59636e` | rgb(89, 99, 110) | `--fgColor-muted` |
| Text Disabled | `#818b98` | rgb(129, 139, 152) | `--fgColor-disabled` |
| Border Default | `#d1d9e0` | rgb(209, 217, 224) | `--borderColor-default` |
| Border Muted | `#d1d9e0b3` | rgba(209, 217, 224, 0.7) | `--borderColor-muted` |
| Border Emphasis | `#818b98` | rgb(129, 139, 152) | `--borderColor-emphasis` |

### Dark Mode Colors

| Element | Hex Code | RGB | CSS Variable |
|---------|----------|-----|--------------|
| Background Default | `#0d1117` | rgb(13, 17, 23) | `--bgColor-default` |
| Background Muted | `#161b22` | rgb(22, 27, 34) | `--bgColor-muted` |
| Background Emphasis | `#6e7681` | rgb(110, 118, 129) | `--bgColor-emphasis` |
| Text Default | `#e6edf3` | rgb(230, 237, 243) | `--fgColor-default` |
| Text Muted | `#8b949e` | rgb(139, 148, 158) | `--fgColor-muted` |
| Border Default | `#30363d` | rgb(48, 54, 61) | `--borderColor-default` |

### State Colors

| State | Background | Border | Text |
|-------|------------|--------|------|
| Open (Issue/PR) | `#dafbe1` | `#4ac26b66` | `#1a7f37` |
| Closed | `#ffebe9` | `#ff818266` | `#d1242f` |
| Merged | `#fbefff` | `#c297ff66` | `#8250df` |
| Draft | `#818b981f` | `#d1d9e0b3` | `#59636e` |

### Data Visualization Colors

| Color Name | Emphasis | Muted | Usage |
|------------|----------|-------|-------|
| Blue | `#006edb` | `#d1f0ff` | Primary data series |
| Green | `#30a147` | `#caf7ca` | Positive trends, additions |
| Red | `#df0c24` | `#ffe2e0` | Negative trends, deletions |
| Purple | `#894ceb` | `#f1e5ff` | Tertiary data |
| Orange | `#eb670f` | `#ffe7d1` | Warnings, attention |
| Teal | `#179b9b` | `#c7f5ef` | Alternative primary |
| Pink | `#ce2c85` | `#ffe5f1` | Accent data |
| Gray | `#808fa3` | `#e8ecf2` | Neutral, inactive |

---

## 2. Typography

### Font Stacks

```css
/* System Sans-Serif (Default) */
--fontStack-sansSerif: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans', 
                        Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji';

/* Monospace (Code) */
--fontStack-monospace: ui-monospace, SFMono-Regular, SF Mono, Menlo, Consolas, 
                        Liberation Mono, monospace;
```

### Type Scale

| Style | Size | Weight | Line Height | CSS Variable |
|-------|------|--------|-------------|--------------|
| Display | 2.5rem (40px) | 500 (Medium) | 1.375 | `--text-display-shorthand` |
| Title Large | 2rem (32px) | 600 (Semibold) | 1.5 | `--text-title-shorthand-large` |
| Title Medium | 1.25rem (20px) | 600 (Semibold) | 1.625 | `--text-title-shorthand-medium` |
| Title Small | 1rem (16px) | 600 (Semibold) | 1.5 | `--text-title-shorthand-small` |
| Subtitle | 1.25rem (20px) | 400 (Normal) | 1.625 | `--text-subtitle-shorthand` |
| Body Large | 1rem (16px) | 400 (Normal) | 1.5 | `--text-body-shorthand-large` |
| Body Medium | 0.875rem (14px) | 400 (Normal) | 1.5 | `--text-body-shorthand-medium` |
| Body Small | 0.75rem (12px) | 400 (Normal) | 1.625 | `--text-body-shorthand-small` |
| Caption | 0.75rem (12px) | 400 (Normal) | 1.25 | `--text-caption-shorthand` |
| Code Block | 0.8125rem (13px) | 400 (Normal) | 1.5 | `--text-codeBlock-shorthand` |

### Font Weights

| Weight | Value | CSS Variable | Usage |
|--------|-------|--------------|-------|
| Light | 300 | `--base-text-weight-light` | Rarely used |
| Normal | 400 | `--base-text-weight-normal` | Body text, descriptions |
| Medium | 500 | `--base-text-weight-medium` | Display headings |
| Semibold | 600 | `--base-text-weight-semibold` | Titles, emphasis |

### Typography Guidelines

- **Line length:** Keep lines around 80 characters or less for optimal readability
- **Alignment:** Content is typically left-aligned with ragged right
- **Hierarchy:** Use font weight and size for hierarchy, avoid color as primary emphasis
- **Code:** Always use monospace font for code, file names, branch names

---

## 3. Spacing & Layout

### Base Spacing Scale

| Token | Value | Pixels | CSS Variable |
|-------|-------|--------|--------------|
| 2 | 0.125rem | 2px | `--base-size-2` |
| 4 | 0.25rem | 4px | `--base-size-4` |
| 6 | 0.375rem | 6px | `--base-size-6` |
| 8 | 0.5rem | 8px | `--base-size-8` |
| 12 | 0.75rem | 12px | `--base-size-12` |
| 16 | 1rem | 16px | `--base-size-16` |
| 20 | 1.25rem | 20px | `--base-size-20` |
| 24 | 1.5rem | 24px | `--base-size-24` |
| 28 | 1.75rem | 28px | `--base-size-28` |
| 32 | 2rem | 32px | `--base-size-32` |
| 40 | 2.5rem | 40px | `--base-size-40` |
| 48 | 3rem | 48px | `--base-size-48` |
| 64 | 4rem | 64px | `--base-size-64` |
| 80 | 5rem | 80px | `--base-size-80` |
| 96 | 6rem | 96px | `--base-size-96` |

### Stack Spacing

| Density | Gap | Padding | CSS Variable |
|---------|-----|---------|--------------|
| Condensed | 8px | 8px | `--stack-gap-condensed` |
| Normal | 16px | 16px | `--stack-gap-normal` |
| Spacious | 24px | 24px | `--stack-gap-spacious` |

### Breakpoints

| Name | Value | CSS Variable |
|------|-------|--------------|
| X-Small | 320px (20rem) | `--breakpoint-xsmall` |
| Small | 544px (34rem) | `--breakpoint-small` |
| Medium | 768px (48rem) | `--breakpoint-medium` |
| Large | 1012px (63.25rem) | `--breakpoint-large` |
| X-Large | 1280px (80rem) | `--breakpoint-xlarge` |
| XX-Large | 1400px (87.5rem) | `--breakpoint-xxlarge` |

### Layout Grid

- **4px baseline grid:** All spacing aligns to 4px increments
- **Flexible columns:** Use CSS Grid or Flexbox for responsive layouts
- **Content max-width:** Typically constrained for readability
- **Responsive design:** Mobile-first approach with progressive enhancement

---

## 4. Borders & Shadows

### Border Width

| Style | Value | CSS Variable |
|-------|-------|--------------|
| Thin (Default) | 1px | `--borderWidth-thin` |
| Thick | 2px | `--borderWidth-thick` |
| Thicker | 4px | `--borderWidth-thicker` |

### Border Radius

| Size | Value | CSS Variable | Usage |
|------|-------|--------------|-------|
| Small | 3px | `--borderRadius-small` | Small elements, tokens |
| Medium | 6px | `--borderRadius-medium` | Buttons, inputs, cards |
| Large | 12px | `--borderRadius-large` | Large containers |
| Full | 50% | `--borderRadius-full` | Avatars, circular elements |

### Shadows

| Shadow | CSS Variable | Usage |
|--------|--------------|-------|
| Resting X-Small | `--shadow-resting-xsmall` | Subtle elevation |
| Resting Small | `--shadow-resting-small` | Cards, default elevation |
| Resting Medium | `--shadow-resting-medium` | Elevated cards |
| Floating Small | `--shadow-floating-small` | Dropdowns, popovers |
| Floating Medium | `--shadow-floating-medium` | Dialogs |
| Floating Large | `--shadow-floating-large` | Modals |
| Inset | `--shadow-inset` | Pressed states, inputs |

### Shadow Values (Light Mode)

```css
--shadow-resting-xsmall: 0 1px 1px 0 rgba(31, 35, 40, 0.05);
--shadow-resting-small: 0 1px 1px 0 rgba(31, 35, 40, 0.04), 0 1px 2px 0 rgba(31, 35, 40, 0.03);
--shadow-resting-medium: 0 1px 1px 0 rgba(37, 41, 46, 0.1), 0 3px 6px 0 rgba(37, 41, 46, 0.12);
--shadow-floating-small: 0 0 0 1px rgba(209, 217, 224, 0.5), 0 6px 12px -3px rgba(37, 41, 46, 0.04), 
                          0 6px 18px 0 rgba(37, 41, 46, 0.12);
--shadow-floating-medium: 0 0 0 1px rgba(209, 217, 224, 0), 0 8px 16px -4px rgba(37, 41, 46, 0.08), 
                          0 4px 32px -4px rgba(37, 41, 46, 0.08);
```

### Focus States

```css
--focus-outlineColor: #0969da;
--outline-focus-width: 2px;
--outline-focus-offset: -2px;
```

---

## 5. Iconography

### Octicons System

GitHub uses **Octicons**, a custom SVG icon set designed specifically for GitHub's interface.

### Icon Sizes

| Size | Dimensions | Usage |
|------|------------|-------|
| 12px | 12 x 12 | Inline indicators, compact UI |
| 16px | 16 x 16 | Standard UI icons, buttons |
| 24px | 24 x 24 | Larger UI elements, headers |
| 32px | 32 x 32 | Feature icons |
| 48px | 48 x 48 | Empty states, marketing |
| 96px | 96 x 96 | Large illustrations |

### Icon Categories

| Category | Examples | Usage |
|----------|----------|-------|
| **Git Operations** | `git-branch`, `git-commit`, `git-merge`, `git-pull-request` | Version control actions |
| **File System** | `file`, `file-code`, `file-directory`, `file-zip` | Files and folders |
| **Actions** | `plus`, `pencil`, `trash`, `download`, `upload` | User actions |
| **Navigation** | `arrow-left`, `chevron-down`, `link-external` | Navigation elements |
| **Status** | `check-circle`, `x-circle`, `alert`, `info` | State indicators |
| **Communication** | `comment`, `mention`, `bell`, `mail` | Notifications, discussions |
| **Objects** | `repo`, `organization`, `person`, `calendar` | GitHub entities |

### Key Icons

```
repo            - Repository
git-pull-request - Pull Request (open)
git-pull-request-closed - Pull Request (closed)
git-merge       - Merged
issue-opened    - Issue (open)
issue-closed    - Issue (closed)
check           - Checkmark
x               - Close/Delete
alert           - Warning
info            - Information
search          - Search
gear            - Settings
kebab-horizontal - More actions
star            - Star/Favorite
eye             - Watch
git-branch      - Branch
git-commit      - Commit
code            - Code
terminal        - Terminal/CLI
copilot         - GitHub Copilot
```

### Icon Guidelines

- **Stroke width:** 1.5px for 16px icons
- **Alignment:** Pixel-perfect alignment on grid
- **Color:** Inherit from parent element
- **Accessibility:** Always pair with text labels or aria-labels

---

## 6. Component Patterns

### Buttons

#### Button Variants

| Variant | Background | Border | Text | Usage |
|---------|------------|--------|------|-------|
| Primary | `#1f883d` | `#1f232826` | `#ffffff` | Main actions, CTAs |
| Default | `#f6f8fa` | `#d1d9e0` | `#25292e` | Secondary actions |
| Outline | `#f6f8fa` | `#d1d9e0` | `#0969da` | Alternative primary |
| Danger | `#f6f8fa` | `#d1d9e0` | `#d1242f` | Destructive actions |
| Invisible | transparent | transparent | `#25292e` | Minimal UI, inline |

#### Button Sizes

| Size | Height | Padding | Font Size |
|------|--------|---------|-----------|
| Small | 28px | 8px 12px | 12px |
| Medium (Default) | 32px | 8px 16px | 14px |
| Large | 40px | 10px 20px | 14px |

#### Button States

```css
/* Default Button */
--button-default-bgColor-rest: #f6f8fa;
--button-default-bgColor-hover: #eff2f5;
--button-default-bgColor-active: #e6eaef;
--button-default-bgColor-disabled: #eff2f5;

/* Primary Button */
--button-primary-bgColor-rest: #1f883d;
--button-primary-bgColor-hover: #1c8139;
--button-primary-bgColor-active: #197935;
--button-primary-bgColor-disabled: #95d8a6;
```

### Form Controls

#### Text Input

| State | Border | Background |
|-------|--------|------------|
| Rest | `#d1d9e0` | `#f6f8fa` |
| Focus | `#0969da` | `#ffffff` |
| Error | `#cf222e` | `#ffffff` |
| Disabled | `#818b981a` | `#eff2f5` |

#### Checkboxes & Radios

```css
--control-checked-bgColor-rest: #0969da;
--control-checked-bgColor-hover: #0860ca;
--control-checked-fgColor-rest: #ffffff;
```

### Labels & Badges

| Type | Background | Text | Border |
|------|------------|------|--------|
| Default | `#818b981f` | `#59636e` | none |
| Primary | `#ddf4ff` | `#0969da` | none |
| Success | `#dafbe1` | `#1a7f37` | none |
| Attention | `#fff8c5` | `#9a6700` | none |
| Severe | `#fff1e5` | `#bc4c00` | none |
| Danger | `#ffebe9` | `#d1242f` | none |
| Done | `#fbefff` | `#8250df` | none |
| Sponsors | `#ffeff7` | `#bf3989` | none |

### State Labels

| State | Background | Icon | Text |
|-------|------------|------|------|
| Open | `#1f883d` | `issue-opened` | White |
| Closed | `#cf222e` | `issue-closed` | White |
| Merged | `#8250df` | `git-merge` | White |
| Draft | `#59636e` | `git-pull-request-draft` | White |

### Avatars

| Size | Dimensions | Border Radius |
|------|------------|---------------|
| Small | 20px | 50% |
| Medium | 32px | 50% |
| Large | 48px | 50% |
| X-Large | 64px | 50% |

### Cards

```css
/* Repository Card */
background: var(--bgColor-default);
border: 1px solid var(--borderColor-default);
border-radius: 6px;
padding: 16px;

/* Hover State */
border-color: var(--borderColor-emphasis);
```

---

## 7. Motion & Animation

### Duration Tokens

| Speed | Duration | Usage |
|-------|----------|-------|
| Fast | 150ms | Micro-interactions, hover states |
| Normal | 200ms | Standard transitions |
| Slow | 300ms | Page transitions, complex animations |

### Easing Functions

```css
/* Standard easing */
--motion-easeInOut: cubic-bezier(0.4, 0, 0.2, 1);
--motion-easeOut: cubic-bezier(0, 0, 0.2, 1);
--motion-easeIn: cubic-bezier(0.4, 0, 1, 1);

/* Linear for progress indicators */
--motion-linear: linear;
```

### Animation Patterns

| Pattern | Duration | Easing | Usage |
|---------|----------|--------|-------|
| Fade In | 200ms | ease-out | Overlays, tooltips |
| Slide Down | 200ms | ease-out | Dropdowns, accordions |
| Scale | 150ms | ease-in-out | Buttons, selection |
| Skeleton Pulse | 2s | ease-in-out | Loading states |
| Spinner | 500ms | linear | Loading indicators |

### Loading Animations

```css
/* Skeleton Loading */
@keyframes skeleton-pulse {
  0%, 100% { opacity: 0.5; }
  50% { opacity: 1; }
}

/* Spinner */
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
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
}
```

---

## 8. Accessibility Standards

### Color Contrast Requirements

| Element | Minimum Ratio | Standard |
|---------|---------------|----------|
| Body text | 4.5:1 | WCAG AA |
| Large text (>18px bold, >24px) | 3:1 | WCAG AA |
| UI components | 3:1 | WCAG AA |
| Chart marks to background | 3:1 | WCAG AA |
| Focus indicators | 3:1 | WCAG AA |

### Focus States

- All interactive elements must have visible focus indicators
- Focus outline: 2px solid `#0969da`
- Focus offset: -2px (inset)
- Never remove focus outlines without providing an alternative

### Keyboard Navigation

| Key | Action |
|-----|--------|
| Tab | Move to next focusable element |
| Shift + Tab | Move to previous focusable element |
| Enter / Space | Activate buttons, links |
| Arrow Keys | Navigate within components |
| Escape | Close overlays, cancel actions |

### ARIA Patterns

```html
<!-- Button with loading state -->
<button aria-busy="true" aria-live="polite">
  <span class="sr-only">Loading...</span>
  Saving
</button>

<!-- Expandable section -->
<button aria-expanded="false" aria-controls="content-id">
  Show more
</button>

<!-- Status labels -->
<span role="status" aria-label="Issue open">
  <svg aria-hidden="true">...</svg>
  Open
</span>
```

### Screen Reader Considerations

- Use semantic HTML elements
- Provide text alternatives for icons
- Announce dynamic content changes
- Maintain logical heading hierarchy
- Label all form inputs

---

## 9. Platform-Specific Guidelines

### Web Application

#### Layout Structure

```
┌─────────────────────────────────────────────────────────┐
│ Header (Navigation, Search, User Menu)                   │
├─────────────┬───────────────────────────────────────────┤
│             │                                           │
│  Sidebar    │  Main Content Area                        │
│  (Nav List) │                                           │
│             │                                           │
│             │  ┌─────────────────────────────────────┐  │
│             │  │ Page Header                         │  │
│             │  ├─────────────────────────────────────┤  │
│             │  │                                     │  │
│             │  │ Content                             │  │
│             │  │                                     │  │
│             │  └─────────────────────────────────────┘  │
│             │                                           │
└─────────────┴───────────────────────────────────────────┘
```

#### Repository Page Pattern

```
Repository Header
├── Owner / Repo Name (breadcrumb)
├── Visibility Badge
├── Watch / Fork / Star Actions
│
UnderlineNav (Code | Issues | Pull Requests | Actions | ...)
│
Content Area
├── File Tree (TreeView component)
├── File Browser / README
└── Sidebar (About, Releases, Contributors)
```

#### Overlays

| Type | Width | Max Height |
|------|-------|------------|
| X-Small | 192px | - |
| Small | 320px | 256px |
| Medium | 480px | 320px |
| Large | 640px | 432px |
| X-Large | 960px | 600px |

### Code & Syntax Highlighting

#### Code Block Styling

```css
/* Code block container */
background: var(--bgColor-muted);
border: 1px solid var(--borderColor-default);
border-radius: 6px;
font-family: var(--fontStack-monospace);
font-size: 13px;
line-height: 1.5;
padding: 16px;
overflow-x: auto;
```

#### Syntax Highlighting Tokens

| Token Type | Light Mode | Dark Mode |
|------------|------------|-----------|
| Comment | `#59636e` | `#8b949e` |
| Keyword | `#cf222e` | `#ff7b72` |
| String | `#0a3069` | `#a5d6ff` |
| Function | `#8250df` | `#d2a8ff` |
| Variable | `#953800` | `#ffa657` |
| Number | `#0550ae` | `#79c0ff` |
| Operator | `#1f2328` | `#e6edf3` |

### Contribution Graph

The signature contribution graph uses a 5-level intensity scale:

| Level | Light Mode | Dark Mode | Meaning |
|-------|------------|-----------|---------|
| 0 | `#ebedf0` | `#161b22` | No contributions |
| 1 | `#9be9a8` | `#0e4429` | 1-3 contributions |
| 2 | `#40c463` | `#006d32` | 4-6 contributions |
| 3 | `#30a14e` | `#26a641` | 7-9 contributions |
| 4 | `#216e39` | `#39d353` | 10+ contributions |

### Markdown Rendering

#### Heading Styles

| Level | Size | Weight | Border |
|-------|------|--------|--------|
| H1 | 2em | 600 | Bottom border |
| H2 | 1.5em | 600 | Bottom border |
| H3 | 1.25em | 600 | None |
| H4 | 1em | 600 | None |
| H5 | 0.875em | 600 | None |
| H6 | 0.85em | 600 | Muted color |

#### Block Elements

```css
/* Blockquote */
border-left: 4px solid var(--borderColor-default);
padding-left: 16px;
color: var(--fgColor-muted);

/* Code inline */
background: var(--bgColor-muted);
border-radius: 6px;
padding: 0.2em 0.4em;
font-size: 85%;

/* Horizontal rule */
border: 0;
border-top: 1px solid var(--borderColor-default);
margin: 24px 0;

/* Table */
border-collapse: collapse;
border: 1px solid var(--borderColor-default);

/* Table cell */
padding: 6px 13px;
border: 1px solid var(--borderColor-default);
```

### Pull Request & Issue UI

#### PR/Issue Header

- State label (Open/Closed/Merged)
- Title with issue/PR number
- Author avatar and metadata
- Labels, assignees, reviewers

#### Timeline Events

```css
/* Timeline item */
position: relative;
padding-left: 60px;
margin-bottom: 16px;

/* Timeline badge */
position: absolute;
left: 0;
width: 32px;
height: 32px;
border-radius: 50%;
background: var(--bgColor-muted);
border: 2px solid var(--bgColor-default);
```

#### Diff View

| Element | Addition | Deletion | Neutral |
|---------|----------|----------|---------|
| Line Background | `#dafbe1` | `#ffebe9` | `#ffffff` |
| Gutter Background | `#aceebb` | `#ffcecb` | `#f6f8fa` |
| Word Highlight | `#4ac26b66` | `#ff818266` | - |

---

## Quick Reference

### Essential CSS Variables

```css
/* Colors */
--fgColor-default: #1f2328;
--fgColor-muted: #59636e;
--fgColor-accent: #0969da;
--fgColor-success: #1a7f37;
--fgColor-danger: #d1242f;

--bgColor-default: #ffffff;
--bgColor-muted: #f6f8fa;
--bgColor-emphasis: #25292e;

--borderColor-default: #d1d9e0;
--borderColor-muted: #d1d9e0b3;

/* Typography */
--fontStack-sansSerif: -apple-system, BlinkMacSystemFont, 'Segoe UI', 
                        'Noto Sans', Helvetica, Arial, sans-serif;
--fontStack-monospace: ui-monospace, SFMono-Regular, SF Mono, Menlo, 
                        Consolas, Liberation Mono, monospace;

/* Spacing */
--base-size-4: 0.25rem;
--base-size-8: 0.5rem;
--base-size-16: 1rem;
--base-size-24: 1.5rem;

/* Borders */
--borderRadius-medium: 6px;
--borderWidth-thin: 1px;

/* Focus */
--focus-outlineColor: #0969da;
```

### Resources

- **Primer Documentation:** https://primer.style
- **Octicons:** https://primer.style/octicons
- **Primer React:** https://primer.style/react
- **Primer ViewComponents (Rails):** https://primer.style/view-components
- **Figma Libraries:** https://primer.style/product/getting-started/figma
- **GitHub Brand Guidelines:** https://brand.github.com

---

*Based on GitHub's Primer Design System. For the most current specifications, always refer to the official Primer documentation.*
