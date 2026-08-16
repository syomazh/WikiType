# WikiType

a typing practice website where you can practice typing any wikipedia page you want



## Features

- Paste a Wikipedia URL, search by title, or load a random article
- Clicking a link inside an article loads it in-app instead of navigating away
- Strict mode (must fix typos to advance) or Forgiving mode (marks errors, keeps going)
- Live WPM, accuracy, time, and progress
- Stop anytime with the Stop button or `Esc` to see your results early
- Accented characters (é, è, ñ, ü, …) count as their base letter
- Dark mode, following your system preference by default

## Usage

open https://syomazh.github.io/WikiType/

or 

Open `index.html` in any browser — double-click works, no server needed. Since it's fully client-side, it also runs fine from GitHub Pages, Cloudflare Pages, or any static host.

## How it works

Fetches article HTML and images from Wikipedia's public API (`action=parse`, anonymous CORS) and loads Wikipedia's real stylesheet (`w/load.php?...&skin=vector-2022`) so it looks like the genuine site. Each typable paragraph is split into per-character spans; keystrokes are checked against the expected character and styled live (dimmed → correct/incorrect → cursor). Only paragraph prose is typable — headings, lists, tables, and captions are shown but not typed.

## Attribution

Article text and images are © their Wikipedia contributors, [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Not affiliated with the Wikimedia Foundation.

