# Descript Design System

> AI video and podcast editing design with warm green identity, timeline-first surfaces, word-based editing clarity, and creator-friendly UX.

---

## 1. Visual Theme & Atmosphere

Descript should feel creative, approachable, and magically simple. The design language communicates video editing through a text transcript, AI voice cloning, screen recording, and podcast production in a single tool.

- Mood: creative, approachable, modern, magically simple
- Density: medium, with transcript editor, timeline scrubber, media library, and AI-tool panels
- Character: warm green brand, off-white editor canvas, dark timeline surface, transcript-first editing

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--des-green` | `#1DB954` | Primary brand CTA and active state |
| `--des-green-dark` | `#169C44` | Hover and active states |
| `--des-purple` | `#7C3AED` | AI voice and Overdub accent |
| `--des-blue` | `#3B82F6` | Screen recording and clip accent |
| `--des-amber` | `#F59E0B` | Processing and rendering state |
| `--des-red` | `#EF4444` | Recording active and delete action |
| `--surface-editor` | `#FAFAFA` | Transcript editor background |
| `--surface-timeline` | `#1A1A2E` | Timeline and media player surface |
| `--surface-sidebar` | `#F4F4F6` | Media library sidebar |
| `--text-primary` | `#111827` | Transcript body text |
| `--text-speaker` | `#6B7280` | Speaker label above transcript |
| `--border-default` | `#E5E7EB` | Panel and clip borders |

Green is the primary action color. Purple is strictly for AI-powered features (Overdub, AI voices). Red signals active recording — use it prominently when the mic is live.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-transcript: "Georgia", "Palatino", serif;
--font-mono: "JetBrains Mono", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 28px | 700 | 1.1 |
| Section Title | 20px | 600 | 1.2 |
| Transcript Body | 17px | 400 | 1.85 |
| Speaker Label | 12px | 600 | 1.3 |
| Timeline Clip | 12px | 500 | 1.3 |
| Body | 15px | 400 | 1.6 |
| Label | 12px | 600 | 1.35 |

Transcript text uses a slightly larger size and generous line-height — it is the primary editing surface and must be supremely readable.

## 4. Component Stylings

```css
.button-primary {
  min-height: 38px;
  padding: 0 18px;
  border: none;
  border-radius: 8px;
  background: #1DB954;
  color: #FFFFFF;
  font: 600 14px/1 Inter, sans-serif;
}

.transcript-word {
  cursor: text;
  border-radius: 3px;
  transition: background 0.1s;
}

.transcript-word:hover    { background: #F3F4F6; }
.transcript-word.selected { background: #DCFCE7; }
.transcript-word.deleted  { text-decoration: line-through; color: #9CA3AF; }

.timeline-clip {
  border-radius: 6px;
  background: #3B82F6;
  color: #FFFFFF;
  padding: 4px 8px;
  font: 500 11px/1.3 Inter, sans-serif;
  overflow: hidden;
  white-space: nowrap;
}

.recording-dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #EF4444;
  animation: pulse 1.2s ease-in-out infinite;
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `8px` | Speaker-to-transcript spacing |
| `--space-4` | `16px` | Transcript paragraph gap |
| `--space-6` | `24px` | Section padding |
| `--space-10` | `40px` | Panel separation |

Transcript editor occupies the main canvas. Timeline is pinned to the bottom (collapsible). Media library and AI tools are in side panels. The word-click-to-seek behavior must be instantly responsive.

## 6. Depth & Elevation

```css
.shadow-card     { box-shadow: 0 1px 4px rgba(17, 24, 39, 0.06); }
.shadow-timeline { box-shadow: 0 -4px 20px rgba(26, 26, 46, 0.24); }
.shadow-modal    { box-shadow: 0 20px 50px rgba(17, 24, 39, 0.16); }
```

The timeline panel at the bottom uses an upward shadow to separate it from the transcript editor above.

## 7. Do's and Don'ts

Do make word-level transcript selection the primary editing interaction. Do highlight deleted words with strikethrough rather than removal. Do make the recording button impossible to miss when live. Do not use green for AI-feature accents — that dilutes the brand. Do not let the timeline compete visually with the transcript editor.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | Playback and basic clip trim only |
| Tablet | `768px` | Transcript editor with collapsed timeline |
| Desktop | `1200px` | Full editor: transcript + timeline + media library + AI panel |

Editing is a desktop workflow. Mobile supports review and approval.

## 9. Agent Prompt Guide

Design like Descript: warm green CTAs, word-level transcript editing surface, dark timeline panel, purple AI-voice accents, generous line-height for transcript readability, red recording indicator, and creator-friendly media editing hierarchy.
