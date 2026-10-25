# Shikaku

A browser Shikaku puzzle (四角に切れ, "divide by squares"). Split the grid into rectangles so that each rectangle holds exactly one number, and that number is the rectangle's area.

**Play:** https://dqyi11.github.io/shikaku/

## Levels

| Level  | Grid  | Largest rectangle | Notes |
|--------|-------|-------------------|-------|
| Easy   | 8×8   | 10 | |
| Medium | 16×16 | 20 | |
| Hard   | 32×32 | 28 | |
| Expert | 40×40 | 32 | Always needs overlap reasoning |
| Master | 50×50 | 36 | Always needs overlap reasoning, often more |

Every puzzle is generated fresh in the browser and checked by an exact-cover solver to have exactly one solution. When a layout has a second solution, only the clues where the two solutions differ are moved (or the two tied rectangles are merged), so even a 50×50 board with about 200 clues is ready in well under a second.

## Controls

- Drag across the grid to draw a rectangle; tap a rectangle to erase it.
- Keyboard: arrow keys move, Enter starts and finishes a rectangle, Delete erases, Ctrl/Cmd+Z undoes.
- Hint places one correct rectangle and adds 15 seconds.
- Pause hides the board and stops the clock.
- Big boards scroll inside their frame. Zoom with the − / Fit / + buttons, pinch, Ctrl/Cmd + scroll, or the + and − keys. On touch screens, drag with two fingers to move around; while drawing near an edge, the board scrolls with you.

## Records

The five best times per level are saved in the browser's local storage, so they stay on the device and browser you play on.

## Development

Everything is in `index.html`: plain HTML, CSS and JavaScript with no build step. Fonts load from Google Fonts. To update the site, edit `index.html` and push to `main`; GitHub Pages redeploys in about a minute.
