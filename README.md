# FlappyBirdGame
A Unity-based implementation of the classic Flappy Bird game. This project serves as a practice and demonstration of Unity game development skills.

## Project Structure

- `Assets/`
  - `Scenes/`
    - `SampleScene.unity`: The main game scene containing the game objects and components.
  - `Scripts/`
    - `BirdScript.cs`: Controls the bird's movement and handles collision detection.
    - `PipeMoveScript.cs`: Handles the movement of the pipes.
    - `PipeSpawnScript.cs`: Manages the spawning of pipes at regular intervals.
    - `LogicScript.cs`: Contains the game logic, including scoring and game state management.
    - `PipeMiddleScript.cs`: Manages the middle section of the pipes for collision detection.

## Hierarchy Overview

- `SampleScene`
  - `Main Camera`
  - `Bird`: The player-controlled bird object.
  - `Pipe Spawner`: The object responsible for spawning pipes.
  - `EventSystem`
  - `Canvas`
    - `Text (Legacy)`: Displays the score.
    - `Game Over Screen`: Displays the game over message.
  - `Logic Manager`: Manages the game logic and state.
  - `Pipe`
    - `Top Pipe`: The top part of the pipe obstacle.
    - `Bottom Pipe`: The bottom part of the pipe obstacle.
    - `Middle`: The middle section of the pipe for collision detection.

## Scripts Overview

### BirdScript.cs

This script controls the bird's movement and handles collision detection with pipes and the ground. It includes logic for jumping and responding to player input.

### PipeMoveScript.cs

This script manages the movement of the pipes from right to left, creating the obstacles for the bird to navigate through.

### PipeSpawnScript.cs

This script is responsible for spawning pipes at regular intervals to maintain a consistent challenge for the player.

### LogicScript.cs

This script contains the core game logic, including:
- Scoring
- Game state management (e.g., starting, playing, game over)
- Restarting the game

### PipeMiddleScript.cs

This script manages the middle section of the pipes, primarily for collision detection to track when the bird passes through the pipes for scoring.

