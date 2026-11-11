# Custom Crossword Maker

AppADay 188. Enter a theme and Claude writes a themed word list with clues. The page then lays the words out as an interlocking crossword grid you can solve on screen, print, or save as an image.

## How it works

1. Type a theme, pick a difficulty (Easy, Medium, Hard) and a word count (10, 15, 20, 25), then tap Generate.
2. Claude returns a title plus more candidate words than needed, each with a clue.
3. A layout engine tries hundreds of randomized placements, keeps the most compact grid that interlocks correctly, numbers the squares, and splits the clues into Across and Down.

## Features

- Solve on screen with a tap-to-select grid, a sticky clue bar, Check, Reveal letter, Reveal word, Reveal all, and Clear.
- Words and clues editor: rewrite a clue, drop a word, or add your own, then apply. Clue-only edits keep your progress.
- New layout button reshuffles the same words into a different grid.
- Print a clean puzzle sheet, or print with an answer key on page two.
- Save image makes a PNG of the grid and clues.
- Save puzzles to My puzzles and reopen them later. The current puzzle and your progress are kept automatically.
- Optional solving timer and an audience setting (for example 5th graders) that shapes the clue wording.

## Setup

Add your Claude API key with the gear button. The key stays in your browser and is sent only to api.anthropic.com. The model comes from the AppADay shared models.js, so no model ID lives in this file.

## Notes

Single index.html, no framework, no build step. Layout and clue generation run in the browser. Everything is stored in localStorage on your device.

Back to the [AppADay portfolio](https://augustineiacopelli.github.io/appaday/).
