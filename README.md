# CS330
Portfolio Submission

**2D Animation and Collision Implementation Reflection**

In this project, I enhanced a 2D animation using OpenGL and GLFW by expanding objects behaviors and implementing custom collision mechanics.
In order to improve the visual engagement, I structured the scene with distinct brick types, separating indestructible, reflective surfaces from destructible bricks. Upon the collision with a destructible brick, the system updates the brick’s state by reducing its durability (hit_cout), which then requires it to take multiple hits in order to destroy. Additionally, the brick darkens dynamically upon impact to provide immediate visual feedback.

For circle physics, I updated screen boundary bounce, in order to preserve vector movement and speed across directional state that changes rather than relying on static paths. When circles interact with each other, the distance calculations evaluate bounding overlap; colliding circles then merge into a single, larger gold object while deactivating the consumed entity.

This program modularized into distinct helper methods, such as CheckCollision and CheckCircleCollisions, this keeps execution logical and free from syntax errors. Code readability is maintained through descriptive inline comments, explicit variable typing, and standard indentation practices.
