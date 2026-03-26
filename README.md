# Snake Game

A classic Snake game built with vanilla HTML, CSS, and JavaScript that runs entirely in the browser — no frameworks or dependencies required.

## What it does

- **Gameplay**: The player controls a snake on a 20×20 grid. The snake moves continuously and the player steers it using the arrow keys to eat food that appears at random positions on the board.
- **Growth & speed**: Each time the snake eats a piece of food it grows longer and the game gradually speeds up, making it progressively more challenging.
- **Collision detection**: The game ends if the snake hits a wall (the edge of the grid) or collides with its own body.
- **Scoring**: The current score (number of food items eaten) is displayed in real time. The all-time high score is stored in `localStorage` so it persists between sessions.
- **Game-over feedback**: When the player loses, a flashing screen animation plays and a short audio clip (`Audio/wrong.mp3`) is triggered before the start screen reappears.
- **Start screen**: An AI-generated snake-themed image and a "Press spacebar to continue" prompt are shown before the game begins. The game can also be started by pressing the `c` key.
- **Responsive design**: The board scales down on smaller screens (≤ 610 px and ≤ 320 px) so the game is playable on mobile devices.

## Project structure

```
Snake-game/
├── index.html   # Game markup – board, score displays, and start screen
├── script.js    # Game logic – snake movement, food, collision, scoring
├── style.css    # Retro Game Boy–inspired styling with responsive breakpoints
├── Audio/
│   └── wrong.mp3        # Sound effect played on game over
└── images/
    └── snake-game-ai-gen.png  # Start-screen artwork
```

## How to run

Open `index.html` directly in any modern browser — no build step or server required.

## Controls

| Key | Action |
|-----|--------|
| Space / `c` | Start / restart the game |
| Arrow keys | Change the snake's direction |
