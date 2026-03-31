# Focus Timer

A neurodivergent-friendly countdown timer designed for children with ADHD and autism. Built as a single HTML file with no dependencies — just double-click to open.

## Features

- **Work/Break cycles** — configurable focus sessions (1-45 min) followed by breaks (1-15 min), auto-cycling through rounds
- **Circular progress ring** — clear visual countdown with smooth animation
- **Gentle alert chimes** — two-tone C5/E5 sine wave dings (1, 3, 5, or 10) with 3-second spacing, generated via Web Audio API
- **Transition messages** — encouraging, predictable messages between phases ("You did it! Time to rest.")
- **Mute toggle** — sound can be toggled on/off at any time, even mid-ding sequence
- **Remembers your choices** — selected presets and mute state persist via localStorage
- **Pause/Resume** — spacebar or button; Stop returns to setup
- **Fully responsive** — works on desktop, laptop, tablet, and phone using `clamp()`, `dvh`, `vmin`, and `aspect-ratio`
- **Dark mode** — automatic via `prefers-color-scheme`

## Neurodivergent Design Principles

- **Predictable structure** — consistent layout, clear phase labels, no surprises
- **Low sensory load** — calming gradient backgrounds (indigo for focus, teal for break), no flashing or harsh colors
- **Large readable fonts** — tabular-nums for stable digit width, generous sizing
- **Reduced motion support** — respects `prefers-reduced-motion` by disabling animations
- **Research-backed ding spacing** — 3-second intervals allow full auditory processing (autism) and distinct attention cues (ADHD)
- **Encouraging language** — transition messages use autonomy-supportive phrasing based on self-determination theory and social stories approach
- **Touch-friendly** — large tap targets, `-webkit-tap-highlight-color: transparent`, `touch-action: manipulation`

## Usage

1. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari)
2. Select a **Focus Time** duration
3. Select a **Break Time** duration
4. Optionally adjust **Alert Dings** count (default: 3)
5. Press **Start**
6. When the timer ends, dings play and a transition message appears, then the next phase begins automatically

### Keyboard Shortcuts

| Key   | Action              |
|-------|---------------------|
| Space | Pause / Resume      |

## Technical Details

- **Single file** — all HTML, CSS, and JavaScript in one `index.html` (no build step, no server, no dependencies)
- **Sound generation** — Web Audio API oscillators (no audio files needed)
- **Responsive layout** — CSS `clamp()` for fluid typography and spacing, `100dvh` for full viewport height, `aspect-ratio: 1` for the timer ring
- **Landscape support** — dedicated `@media (max-height: 500px) and (orientation: landscape)` breakpoint
- **State persistence** — `localStorage` for work/break/dings presets and mute state
- **Accessibility** — `aria-label` on mute button, `focus-visible` outlines, semantic HTML

## Browser Support

Any modern browser released after 2022. Requires support for:
- CSS `dvh` units
- CSS `clamp()`
- CSS `aspect-ratio`
- Web Audio API
- `localStorage`
