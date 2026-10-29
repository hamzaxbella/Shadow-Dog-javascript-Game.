# Shadow Dog

A keyboard-controlled Canvas runner with sprite animation, combat states, and parallax scenery.

## Controls

The current source uses **AZERTY-style keys**, rather than arrow keys.

| Key | Action |
| --- | --- |
| `Q` / `D` | Move left / right |
| `Z` | Jump |
| `S` | Sit on the ground / dive in the air |
| `Space` | Roll attack |
| `E` | Toggle debug display |
| `R` | Restart after game over |

Avoid enemies in normal movement and attack while rolling or diving. Score, remaining lives, and the timer determine the run.

## Run locally

```bash
git clone https://github.com/hamzaxbella/Shadow-Dog-javascript-Game..git
cd Shadow-Dog-javascript-Game.
python3 -m http.server 8000
```

Open <http://localhost:8000> in a modern browser. There is no package installation or build step.

Serve over HTTP: the game uses JavaScript modules, so opening `index.html` directly as a local file can fail.

## Inside the engine

| File | Responsibility |
| --- | --- |
| `game.js` | Game loop, scoring, enemies, and restart |
| `Player.js`, `playerStates.js` | Player animation and state transitions |
| `input.js` | Keyboard input |
| `background.js`, `enemies.Js` | Scenery and enemy behavior |
| `Particles.js`, `collisionAnimation.js` | Visual feedback |
| `UI.js`, `floatingMessages.js` | HUD and score messages |

Built with JavaScript, HTML, CSS, and Canvas 2D. This is a browser game project; the current source does not implement an online leaderboard or an audio system. Included art retains its original ownership.
