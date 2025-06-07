# Space Shooter Game
![]([https://github.com/fmtvp/spacefighter/image.png](https://github.com/fmtvp/spacefighter/blob/main/assets/image.png)

A Python-based space shooter game with enemy fighter planes, player movement controls, and shooting mechanics.

## Game Features

- **Player Spaceship**: Move left, right, forward (max 2 units), and backward
- **Enemy Types**:
  - Regular enemies (5 points): Appear frequently
  - Special enemies (10 points): Appear randomly, move faster
- **Power-ups**:
  - Extra Life: Randomly spawns, gives +1 life when collected
- **Difficulty Levels**:
  - Easy: Fewer enemies, slower movement, rare special enemies, more frequent life power-ups
  - Normal: Balanced gameplay
  - Hard: More enemies, faster movement, frequent special enemies, rare life power-ups
- **Combat**: Shoot lasers to destroy enemy ships
- **Scoring**: Earn points based on enemy type (5 or 10 points)
- **Lives System**: Player has three lives before game over, can collect more
- **Visual Effects**: Explosions when enemies are destroyed
- **Dynamic Background**: Scrolling star field for immersion
- **Responsive Design**: Game elements automatically resize based on window dimensions

## Controls

- **Left Arrow**: Move left
- **Right Arrow**: Move right
- **Up Arrow**: Move forward (limited to 2 units)
- **Down Arrow**: Move backward (only after moving forward)
- **Space**: Fire weapon
- **R**: Restart game after game over
- **Q**: Quit game after game over
- **E/N/H**: Select difficulty (Easy/Normal/Hard) at the start screen

## Requirements

- Python 3.x
- Pygame

## Installation

1. Make sure you have Python installed
```
git clone https://github.com/fmtvp/spacefighter
cd spacefighter
pip install -r requirements.txt
python3 spcae_shooter.py
```
## Custom Graphics

The game will look for image assets in an `assets` folder. If you want to add custom graphics, create the following files:
- `player_ship.png`: Player's spaceship
- `enemy_ship.png`: Regular enemy fighters (5 points)
- `special_enemy_ship.png`: Special enemy fighters (10 points)
- `life.png`: Extra life power-up

If these files are not found, the game will use colored shapes as placeholders.

## Responsive Design

The game automatically adjusts all elements based on the window size:
- Images are scaled proportionally to the screen dimensions
- UI elements (score, lives) adjust to fit the screen
- Game objects maintain proper proportions regardless of window size
- Window can be resized during gameplay
