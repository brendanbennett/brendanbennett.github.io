# Design System

Reference document for brendanbennett.github.io. Use these tokens to keep related projects visually consistent.

## Colour Palette

The site uses a single **dark theme** with a green-tinted palette. No light mode.

| Token | Hex | Usage |
|-------|-----|-------|
| `--bg` | `#111a14` | Main background |
| `--bg-sidebar` | `#0d140f` | Sidebar / secondary background |
| `--surface` | `#182119` | Raised surfaces, cards |
| `--text` | `#c8d5cb` | Body text |
| `--text-muted` | `#7a8f7e` | Secondary / caption text |
| `--accent` | `#5a9e6f` | Links, primary accent |
| `--accent-dim` | `#3d6b4a` | Dimmed accent, secondary elements |
| `--border` | `#243328` | Borders and dividers |

**Additional values:**

- Heading text: `#dce8df`
- Link hover: `#7ec492`
- Code background: `rgba(90, 158, 111, 0.15)`

## Typography

### Font Families

| Role | Stack | CSS Variable |
|------|-------|-------------|
| Content / headings | Libre Baskerville, Georgia, serif | `--font-serif` |
| UI / navigation | Inter, system-ui, sans-serif | `--font-sans` |

Google Fonts import:

```
Libre Baskerville: 400, 400 italic, 700
Inter: 300, 400, 500, 600
```

### Type Scale

| Element | Family | Size | Weight | Line Height |
|---------|--------|------|--------|-------------|
| h1 | serif | 2rem | 700 | 1.3 |
| h2 | serif | 1.4rem | 700 | 1.3 |
| h3 | serif | 1.15rem | 700 | 1.3 |
| Body | sans | 1rem (16px) | 300 | 1.7 |
| Prose (articles) | serif | 1.05rem | 400 | 1.8 |
| Nav links | sans | 0.9rem | 400 | — |
| Section headers (CV) | sans | 1.3rem | 600 | — |
| Date stamps | sans | 0.8rem | 400 | — |
| Subtitle / intro | serif | 1.1rem | 400 | — |

### Letter Spacing

- Site name: `0.02em`
- Nav links: `0.01em`
- Section headers / date stamps: `0.05em`

## Borders and Radii

| Element | Radius |
|---------|--------|
| Buttons, tags | `12px` |
| Avatars | `50%` (circle) |
| Inline code | `3px` |

Border style is consistently `1px solid var(--border)`.

## Shadows

None. The design is flat throughout.

## Transitions

Standard transition: `0.15s ease` on hover states (links, nav items, buttons).

## Spacing

| Context | Value |
|---------|-------|
| Sidebar width | `220px` |
| Main content padding | `3rem 4rem` |
| Section gap | `1.25rem – 2.5rem` |
| Nav gap | `0.25rem` |
| Nav link padding | `0.5rem 0.75rem` |
| List item gap | `0.75rem` |

## Responsive Breakpoint

Single breakpoint at **768px**:

- Layout switches from sidebar + content row to stacked column
- Main content padding reduces to `2rem 1.5rem`

## Links

- Default: `var(--accent)` with underline (`text-underline-offset: 2px`)
- Hover: `#7ec492`

## Lists

- No bullets; custom marker `">"` in `var(--accent-dim)`
- Padding-left: `1rem`

## Icons

- Size: `14px × 14px` inline SVGs
