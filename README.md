Flappy Bird Evolution - Maliyo Games Assignment
This project is a playable prototype recreated for the Maliyo Games Unity Developer assignment. It features the core mechanics of Flappy Bird with added progressive difficulty and a unique special ability.

1. Technical Approach
The game was developed with a focus on Clean Architecture and Separation of Concerns:

Game Management: Uses a Singleton Pattern (GameManager.cs) to manage game states (Menu, Play, Game Over) and ensure seamless scene transitions.

Player Control: Physics-based movement using Unity's Rigidbody2D, with optimized collision detection for obstacles and kill zones.

Progressive Difficulty: The ObstacleManager scales the game challenge by increasing the pipes' movement speed based on the player's current score.

Optimization: Implemented a DestroyOnExit system to clear off-screen objects, maintaining a high and stable frame rate for WebGL performance.

2. Bonus Feature: Shrink Ability
To differentiate the game from the original reference, I implemented a Shrink Mechanic:

How it works: After passing a set number of pipes (charge phase), the player turns Magenta.

Activation: The player can press Spacebar or Right-Click to shrink to 60% of their original size for 2 seconds.

Strategic Value: This allows players to navigate tight gaps more easily during high-speed phases, adding a tactical layer to the traditional gameplay.

3. Generative AI Usage Disclosure
In line with modern development workflows, Google Gemini (AI) was used strategically during the prototyping phase:

Code Refactoring: Assisted in updating obsolete methods (e.g., migrating to Object.FindFirstObjectByType) to ensure the project aligns with the latest Unity 6 standards.

Logic Optimization: Used to brainstorm the "Shrink" cooldown routine and ensure the progressive difficulty math was balanced.

Documentation & Comments: AI helped generate clear, educational comments within the scripts to ensure maintainability and readability.

4. WebGL & Build Instructions
Platform: WebGL

Resolution: Portrait (9:16 Aspect Ratio)

Target Performance: 60 FPS (exceeding the 30 FPS requirement)

Unity Version: 6000.0.35f1 LTS
