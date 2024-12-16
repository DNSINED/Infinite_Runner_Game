# Zombie Chase

**Zombie Chase** is a 2D side-scrolling game where the player controls a character that must dodge incoming zombies while navigating through a dynamic environment. Clouds float by to add depth and atmosphere, creating a visually engaging experience.

> **Note:** This game is currently under development and not yet finished.

## Features

- **Dynamic Character Animation**: The player character has running and jumping animations for smooth gameplay.
- **Enemy Zombies**: Zombies with walking animations spawn periodically, adding a challenging obstacle.
- **Floating Clouds**: Clouds drift across the screen, creating a lively background.
- **Collision Detection**: The game ends when the player collides with a zombie.
- **Randomized Elements**: Zombie spawn timing and cloud positions vary, ensuring each playthrough is unique.

## Gameplay

The goal is to avoid zombies and stay alive as long as possible. Use the arrow keys to move the player left and right, and the spacebar to jump. Clouds and zombies move automatically.

## Controls

- **Left Arrow Key**: Move the player left.
- **Right Arrow Key**: Move the player right.
- **Spacebar**: Make the player jump.

## Requirements

- **Python 3.6+**
- **Pygame Library**

Install Pygame by running:
```bash
pip install pygame
```

## Installation

1. Clone or download the repository.
2. Ensure all required image assets (player animations, zombie animations, background, and cloud images) are placed in their respective directories.
   - Player animations should be in a folder named `Player`.
   - Zombie animations should be in a folder named `Zombie`.
   - The background image should be named `Background.png`.
   - The cloud image should be named `cloud.png`.
3. Run the game script:
```bash
python game.py
```

## Assets Structure

Ensure the following folder and file structure for assets:
```
.
├── Player
│   ├── Run__000.png
│   ├── Run__001.png
│   ├── ...
│   ├── Jump__000.png
│   ├── Jump__001.png
│   ├── ...
├── Zombie
│   ├── Walk (1).png
│   ├── Walk (2).png
│   ├── ...
├── Background.png
├── cloud.png
```

## How It Works

1. **Game Initialization**:
   - The Pygame library initializes the game window and assets.
   - Background, player, and sprite groups (clouds and zombies) are set up.

2. **Game Loop**:
   - Events are processed (e.g., spawning clouds and zombies).
   - Sprites update their positions based on their respective logic.
   - The player's movement and animations are updated based on key presses.
   - The game checks for collisions between the player and zombies.

3. **Game Over**:
   - If a collision between the player and a zombie occurs, the game ends.

## License

This project is licensed under the Apache License, Version 2.0. See the [LICENSE](http://www.apache.org/licenses/LICENSE-2.0) for details.

## Acknowledgements

- **Pygame**: For providing the framework to create this game.
- **Assets**: Placeholder assets were used for the player, zombies, and background. Replace these with your own custom graphics if needed.

## Future Enhancements

- Add a scoring system to track how long the player survives.
- Introduce power-ups or additional obstacles.
- Enhance graphics and animations.
- Implement different levels or difficulty modes.

Enjoy the game!
