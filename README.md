# Phaser 3 Project

This project is a small Phaser 3 platformer demo created as an internship game prototype. The goal is to move the player around the level, collect every star, and avoid the bombs that appear after each full collection cycle.

## Game purpose

The game is a simple arcade survival challenge:

- Collect stars to increase the score.
- When all stars are collected, they respawn and a bomb is spawned.
- Each bomb makes the game more dangerous.
- If the player touches a bomb, the game pauses and `GAME OVER` is shown.
- A timer counts how long the run lasts.

## Controls

- Left arrow: move left
- Right arrow: move right
- Up arrow: jump

## Project structure

- `Phaser_3_Projet/index.html`: main HTML page that loads the game
- `Phaser_3_Projet/javascript/script.js`: Phaser game logic, physics, scoring, bombs, and timer
- `Phaser_3_Projet/css/style.css`: basic page styling
- `Phaser_3_Projet/assets/`: game images and sprites
- `Phaser_3_Projet/lib/phaser.js`: Phaser library used by the project

## How it works

The game uses Phaser Arcade Physics. The player stands on platforms, jumps across the level, and collects star items. The score increases by 10 points per star. Once all stars are collected, the game respawns the stars and creates a bomb at a random side of the map.

## Run the project

Do not open `Phaser_3_Projet/index.html` directly with `file://`. Phaser loads images through XHR, and browsers block those requests from local files.

Run a local web server from the project folder instead:

```bash
cd /Users/tompalazzolo/git/phaser/Phaser_3_Projet
python3 -m http.server 8000
```

Then open `http://localhost:8000/` in your browser.

If you want, I can also rewrite the HTML and in-game labels so the project title, page text, and file naming are more consistent.
