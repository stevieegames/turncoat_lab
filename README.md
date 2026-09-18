# Turncoat — Laboratory

Turncoat — Laboratory is a browser-based playtesting prototype for the abstract strategy game **Turncoat**. It runs entirely from one HTML file, with no build step and no game server required.

## What is included

- Local two-player play or play against Barry, the random-move test AI
- Ivory versus Chestnut pieces
- Cubes, Wedges, Main Pieces, No Go areas, turncoating, shields and optional Gullies
- Downloadable move logs
- An end-of-game feedback form that can send the game log through Formspree
- Responsive layout for desktop and mobile

The current playtest rules are in [RULES.md](RULES.md).

## Run locally

Download the repository and open `index.html` in a modern browser. No installation is needed.

For local development, you can also serve the folder with any static web server. For example:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Files

- `index.html` — complete game, styling and JavaScript
- `README.md` — project and deployment guide
- `RULES.md` — current laboratory ruleset

## Project status

This is an early playtest build, not a finished competitive rules implementation. Barry is intentionally random and exists to exercise the game flow rather than provide strong play.

