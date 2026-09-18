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

## Publish with GitHub Pages

1. Create a GitHub repository.
2. Put `index.html`, `README.md`, and `RULES.md` in the repository root.
3. Commit and push the files to the `main` branch.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**, choose `main` and `/ (root)`, then save.
6. GitHub will show the public site URL after deployment completes.

See the [GitHub Pages quickstart](https://docs.github.com/en/pages/quickstart) for GitHub's current instructions.

## Connect playtest feedback with Formspree

The feedback UI is already included, but it will not transmit anything until you add your own Formspree endpoint.

1. Create a form at [Formspree](https://formspree.io/).
2. Copy its endpoint. It will look like `https://formspree.io/f/abcdefgh`.
3. In `index.html`, find:

   ```js
   const FEEDBACK_ENDPOINT = "https://formspree.io/f/YOUR_FORM_ID";
   ```

4. Replace the placeholder URL with your endpoint.
5. Commit the change and test one completed game on the published site.

When a tester clicks **Send playtest**, the form sends:

- Their optional free-text feedback
- The game version and date
- Game settings and player types
- The result and complete move log

The game does not ask for a name or email, and it does not submit automatically. Formspree may still process technical request data such as an IP address, so add an appropriate privacy notice and retention policy before inviting public playtests. Review Formspree's terms and privacy settings for the account you use.

## Files

- `index.html` — complete game, styling and JavaScript
- `README.md` — project and deployment guide
- `RULES.md` — current laboratory ruleset

## Project status

This is an early playtest build, not a finished competitive rules implementation. Barry is intentionally random and exists to exercise the game flow rather than provide strong play.

