# Challenge-3-Balloon-GameUp24

## Overview
**Challenge-3-Balloon-GameUp24** is a Unity-based game project where the player controls a balloon, navigating through the sky while avoiding obstacles and collecting items. The challenge involves using Unity physics to create smooth, floating gameplay with gravity, upward forces, and collisions.

This project is a part of the GameUp24 series, where each challenge builds on different game mechanics, improving coding and game development skills in Unity.

## Features
- **Player Control:** Move the balloon upward by pressing the spacebar, navigating through various objects.
- **Gravity Simulation:** Simulates the balloon's floating behavior with custom gravity modifiers.
- **Collision Detection:** Interact with in-game objects like obstacles and collectibles .
- **Particle Effects:** Uses particle systems for visual effects like explosions on impact and fireworks for rewards.
- **Sound Effects:** Includes custom sounds for game events such as collisions, power-ups, and explosions.

## How to Play
1. **Start the Game:** Upon starting, the balloon will float gently with gravity pulling it down.
2. **Use the Spacebar:** Press the **spacebar** to apply an upward force to keep the balloon floating. The longer you hold, the higher the balloon goes.
3. **Avoid Obstacles:** Navigate through obstacles without hitting them to avoid game over.
4. **Collect Items:** Grab special items for points or bonuses, such as speed boosts or extra lives.

## Game Controls
- **Move Up:** Hold the **spacebar** to apply force to the balloon and float upwards.
- **Collect Items:** Move the balloon into collectible objects like coins to earn points.

## Code Snippets
### Player Movement
```csharp
if (Input.GetKey(KeyCode.Space) && !gameOver)
{
    playerRb.AddForce(Vector3.up * floatForce, ForceMode.Impulse);
}
