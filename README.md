# Snake

A modern, responsive Snake game built with pure HTML, CSS and JavaScript. No frameworks, no build step, no dependencies. Just open `index.html` and play.

![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)
![Dependencies: none](https://img.shields.io/badge/dependencies-none-brightgreen.svg)

### Features

- **Clean, modern UI**: dark theme, checkerboard grid, rounded gradient snake with eyes, glowing food
- **Responsive**: scales to fit phones, tablets and desktops, and stays sharp on high-DPI screens
- **Multiple controls**: arrow keys, `WASD`, or touch swipes
- **Smooth gameplay**: input buffering so quick key presses never make the snake reverse into itself
- **Progressive difficulty**: the game speeds up as your score grows
- **Best score**: saved in your browser with `localStorage`
- **Pause, resume and auto-pause** when you switch tabs
- **Sound effects** with a mute toggle, generated with the Web Audio API, so there are no audio files
- **Win condition** when the snake fills the whole board

### How to play

| Action | Keyboard | Touch |
| --- | --- | --- |
| Move | Arrow keys or `W` `A` `S` `D` | Swipe |
| Start / restart | `Space` or `Enter` | Tap **Play** |
| Pause / resume | `Space` | Tap the pause button |

Eat the glowing food to grow and score points. Hitting a wall or your own body ends the game.

### Run it

**Option 1: open the file**

Download or clone the repo and double-click `index.html`.

**Option 2: local server**

```bash
git clone https://github.com/walidwh21/Snake-Game
cd Snake-Game
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

**Option 3: GitHub Pages**

Push the repo, then go to **Settings → Pages**, choose the `main` branch and the `/ (root)` folder, and save. Your game will be live at `https://[username].github.io/snake-game/`.

### Project structure

```
snake-game/
├── index.html   # markup, styles and game logic in one file
├── LICENSE
└── README.md
```

### Customize

All settings are at the top of the script in `index.html`:

- `N`: board size in cells (default `20`)
- `speed`: starting delay in milliseconds between moves (default `130`; lower is faster)
- `Math.max(65, speed - 3)`: the speed limit and how fast the game accelerates
- Colors: edit the CSS variables in `:root` and the colors in `draw()`

### License

Released under the [MIT License](LICENSE). © 2026 [Walid Hattaoui]
