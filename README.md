# Grid & Clue — Nonogram Library

A standalone, dependency-free nonogram site designed for GitHub Pages.

## Features
- 24 starter puzzles with titles, difficulty labels, and black-and-white or colour styles.
- Grid sizes of 5×5, 10×10, and 15×15. Both dimensions are multiples of five.
- Search by title, filter by height/width ranges, style, difficulty, and personal progress.
- Solve in the browser using row and column clues.
- Reveal/hide a puzzle's solution while viewing it.
- Check a solution, clear the board, mark puzzles finished or printed, and print a clean puzzle sheet.
- Saves solve progress and marks in browser local storage; no account required.
- Admin panel can hide puzzles locally and export a catalogue backup.

## Publish on GitHub Pages
1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch **main** and folder **/(root)**, then save.
4. After the Pages build completes, the site should be available at https://reem-masalha.github.io/nonogram/.

## Important limitation: shared admin deletion
This is a static site. The admin panel's **Hide locally** action only hides puzzles in the current browser, and browser progress is local to that browser. A public static page cannot securely restrict administrator actions or permanently remove a puzzle for every visitor. Shared deletion and shared puzzle catalogue updates require an authenticated backend (for example, a Cloudflare Worker with a database and admin authentication). Do not treat the current local admin panel as secure access control.

## Content
Starter puzzles are generated from small hand-authored patterns and expanded to larger grid sizes. The catalogue is self-contained; no external images are loaded. The puzzle library can be expanded by editing the patterns array and generation logic in index.html.
