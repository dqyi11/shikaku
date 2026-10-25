# Shikaku

A browser Shikaku puzzle (四角に切れ, "divide by squares"). Split the grid into rectangles so that each rectangle holds exactly one number, and that number is the rectangle's area.

**Play:** https://dqyi11.github.io/shikaku/

## Levels

| Level  | Grid  | Largest rectangle | Notes |
|--------|-------|-------------------|-------|
| Easy   | 8×8   | 10 | |
| Medium | 10×10 | 12 | |
| Hard   | 13×13 | 16 | |
| Expert | 16×16 | 20 | Always needs overlap reasoning |
| Master | 20×20 | 24 | Needs overlap reasoning or deeper |

Every puzzle is generated fresh in the browser and checked by an exact-cover solver to have exactly one solution.

## Controls

- Drag across the grid to draw a rectangle; tap a rectangle to erase it.
- Keyboard: arrow keys move, Enter starts and finishes a rectangle, Delete erases, Ctrl/Cmd+Z undoes.
- Hint places one correct rectangle and adds 15 seconds.
- Pause hides the board and stops the clock.

## Records

The five best times per level are saved in the browser's local storage, so they stay on the device and browser you play on.

## Development

Everything is in `index.html`: plain HTML, CSS and JavaScript with no build step. Fonts load from Google Fonts. To update the site, edit `index.html` and push to `main`; GitHub Pages redeploys in about a minute.
