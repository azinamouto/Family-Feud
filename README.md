# Family Feud — Retro Classroom Edition

A static, offline-capable, keyboard-operated classroom game inspired by Family Feud. Contains all three user-provided energy/environment survey questions and points. No database, WebSockets, npm installation, or remote required.

## Run locally
Open `index.html` in Chrome or Edge. Click **Start Game**, customize team names, then **Begin Round 1**. Press F11 to maximize the browser window, or press `F` in game for the browser fullscreen API.

## Deploy on Vercel
Import the repository in Vercel and select **Other** (static site). Leave the build command empty. Deploy the project directory containing `index.html` as the root. No environment variables are needed. If the build configuration requires an output directory, use the root (`.`), not `dist`.

## Keyboard controls

| Key | Action |
|---|---|
| 1–6 | Reveal corresponding answer (when allowed) |
| S | Start / restart 5-second timer |
| Space | Pause / resume active timer |
| R | Reset timer to 5.0 seconds, without starting |
| X | Wrong answer / strike / unsuccessful steal |
| A / B | Pick team A / B face-off player |
| P / Q | Play / Pass |
| T | Start steal phase after 3 strikes |
| Enter | Award round bank, or continue to the next round |
| N | Next round after awarding |
| M | Toggle background music |
| F | Toggle fullscreen |
| H | Toggle host console and shortcut guide |
| Esc | Close the visible results overlay |

The host reads guesses aloud, then presses the number matching the survey answer. `S` manually starts a fresh countdown on each guess. On timeout the game registers a wrong answer. Reveals never score a team immediately; they add to the round bank, which is awarded after a clean round or the steal attempt. Note: use browser fullscreen with F11 if your keyboard/browser reserves F.

## Survey totals
Round 1: 20; Round 2: 24; Round 3: 21. No artificial normalization or point multipliers.

## Notes
This is an unofficial, classroom-use recreation. There is no multi-device synchronization. Refreshing the browser restarts the game; do not refresh during a round.
