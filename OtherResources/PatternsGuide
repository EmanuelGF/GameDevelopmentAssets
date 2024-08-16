### **Game Coding Patterns Guide**

#### **1. **Observer Pattern**

**Use When:**
- **Event Handling:** When you need to notify multiple systems or objects about state changes or events, such as player actions, score updates, or UI changes.
- **Loose Coupling:** When you want to decouple the sender and receiver, making your code more modular and easier to maintain.

**Common Scenarios:**
- **Input Handling:** Detecting player input and notifying other systems (like animation or movement).
- **UI Updates:** Updating HUD elements (e.g., health bars, score counters) in response to game events.
- **Game State Changes:** Notifying different systems of game state changes (e.g., level completion, player death).

**Example:**
- In a platformer, when the player collects a coin, an event can notify the score system to update the player’s score and the UI to reflect the new score.

---

### **2. Command Pattern**

**Use When:**
- **Action Encapsulation:** When you need to encapsulate actions as objects, which can then be executed, queued, or undone.
- **Input Handling:** When managing complex input handling systems, especially for command-based games or undo/redo functionality.
- **AI Behavior:** When AI behavior can be broken down into discrete actions that need to be queued or executed sequentially.

**Common Scenarios:**
- **Player Input:** Mapping player inputs to commands that can be executed in the game world.
- **Action Queues:** Handling a sequence of actions, such as in a turn-based strategy game.
- **Undo/Redo Systems:** Allowing players to undo or redo actions, like in a level editor.

**Example:**
- In a strategy game, player commands (like moving units) are encapsulated in command objects that can be stored, executed, or undone if the player changes their mind.

---

### **3. State Pattern**

**Use When:**
- **Complex Object States:** When an object has multiple states that affect its behavior, such as a character with different movement states (e.g., idle, running, jumping).
- **Finite State Machines:** When implementing finite state machines (FSMs) to manage character behavior, AI, or game states.
- **Behavioral Variations:** When you need to change an object’s behavior dynamically based on its state.

**Common Scenarios:**
- **Character States:** Managing player or enemy states like idle, attacking, or fleeing.
- **AI Behavior:** AI enemies with different states (patrolling, chasing, attacking).
- **Game States:** Managing different game states like menu, playing, paused, or game over.

**Example:**
- In a fighting game, the player character's state determines whether they can perform certain actions, like blocking or attacking.

---

### **4. Strategy Pattern**

**Use When:**
- **Behavior Switching:** When you need to switch between different algorithms or behaviors at runtime.
- **AI Decision Making:** When AI entities need to choose different strategies based on the situation (e.g., aggressive vs. defensive behavior).
- **Behavior Customization:** When different objects need to exhibit similar behaviors but with different implementations.

**Common Scenarios:**
- **Enemy AI:** Switching between different AI strategies (e.g., ranged attack vs. melee attack) based on distance from the player.
- **Pathfinding Algorithms:** Choosing between different pathfinding strategies depending on the environment or the character's abilities.
- **Movement Patterns:** Applying different movement behaviors to characters (e.g., walking, flying, swimming).

**Example:**
- In a real-time strategy game, units may switch between different movement strategies depending on whether they are on land, in water, or in air.

---

### **5. Singleton Pattern**

**Use When:**
- **Global Access:** When you need a single instance of a class to be globally accessible, such as for game managers, configuration settings, or audio systems.
- **Resource Management:** When you need to manage shared resources, like a texture cache or an object pool.

**Common Scenarios:**
- **Game Managers:** Centralized game management (e.g., handling game state, level transitions).
- **Audio Systems:** Managing background music or sound effects that need to be accessed globally.
- **Configuration Settings:** Accessing game settings that should be consistent throughout the game.

**Example:**
- In an open-world game, a `GameManager` singleton might handle saving and loading game states, ensuring only one instance is used across the entire game.

---

### **6. Factory Pattern**

**Use When:**
- **Object Creation:** When you need to create objects but want to keep the creation logic separate from the client code.
- **Dynamic Object Creation:** When the types of objects that need to be created aren’t known until runtime.
- **Object Pooling:** When creating objects in bulk, such as in an enemy spawning system.

**Common Scenarios:**
- **Item Creation:** Creating game items (e.g., weapons, potions) dynamically based on player input or game events.
- **Enemy Spawning:** Generating different types of enemies at runtime, especially in wave-based games.
- **Projectile Creation:** Handling different types of projectiles (e.g., bullets, rockets) with different behaviors.

**Example:**
- In a tower defense game, a `TowerFactory` might be responsible for creating different types of towers based on player selection and placement.

---

### **7. Composite Pattern**

**Use When:**
- **Hierarchical Structures:** When you need to treat individual objects and compositions of objects uniformly, such as in an inventory system.
- **Complex Object Management:** When managing complex objects that can contain other objects, like a scene graph or UI components.
- **Recursive Structures:** When you need to work with recursive structures where objects contain other objects of the same type.

**Common Scenarios:**
- **Inventory Systems:** Handling nested items, like a backpack containing potions and weapons.
- **UI Components:** Building a UI system where UI elements can contain other UI elements.
- **Scene Graphs:** Managing a scene graph where objects can contain child objects (e.g., a tree structure for game objects).

**Example:**
- In an RPG, the inventory system might use the Composite Pattern to handle containers like bags or chests that can hold other items.

---

### **8. Decorator Pattern**

**Use When:**
- **Adding Behavior Dynamically:** When you need to add responsibilities or modify the behavior of objects dynamically, such as enhancing a character’s abilities.
- **Flexible Extension:** When you want to add features to objects without altering their class definitions.
- **Layered Functionality:** When features can be layered onto objects, such as adding status effects to characters.

**Common Scenarios:**
- **Character Abilities:** Adding power-ups or buffs/debuffs to characters dynamically (e.g., speed boost, shield).
- **Weapon Enhancements:** Modifying weapon properties with attachments (e.g., scopes, silencers).
- **Skill Systems:** Enhancing player skills with modifiers (e.g., increased range or damage).

**Example:**
- In a shooter game, a weapon might be decorated with different attachments (e.g., scopes, silencers) that modify its behavior.

---

### **9. Flyweight Pattern**

**Use When:**
- **Memory Optimization:** When you need to manage a large number of similar objects efficiently by sharing common data.
- **Resource Sharing:** When many objects share the same data, like textures or mesh data in a game.
- **Reducing Overhead:** When reducing memory usage and overhead is critical, especially in resource-constrained environments.

**Common Scenarios:**
- **Particle Systems:** Managing large numbers of particles that share common properties like texture and color.
- **Tile-Based Games:** Handling game tiles where many tiles share the same texture but have different states or positions.
- **Text Rendering:** Efficiently rendering large amounts of text where characters share common font data.

**Example:**
- In a 2D platformer, a tilemap might use the Flyweight Pattern to manage tiles efficiently, reducing the memory footprint by sharing texture data among similar tiles.

---

### **10. Prototype Pattern**

**Use When:**
- **Object Cloning:** When you need to create new objects by copying existing ones rather than instantiating them from scratch.
- **Configuration Preservation:** When creating objects that share the same configuration but may differ slightly in state.
- **Avoiding Expensive Creation:** When the cost of creating a new object is high, and copying an existing object is more efficient.

**Common Scenarios:**
- **Character Creation:** Cloning character presets to quickly create multiple instances of similar characters with minor differences.
- **Level Design:** Creating variations of level elements (e.g., obstacles, platforms) by cloning existing templates.
- **Enemy Spawning:** Spawning waves of enemies based on prototypes rather than configuring each one from scratch.

**Example:**
- In an RTS game, units may be created by cloning a prototype, allowing for quick and efficient creation of multiple units with similar configurations.

---

### **11. Object Pooling**

**Use When:**
- **High-Frequency Object Creation/Destruction:** When you have objects that are frequently created and destroyed, like bullets, enemies, or particles.
- **Performance Optimization:** When you need to optimize performance by reusing objects instead of continuously allocating and deallocating memory.

**Common Scenarios:**
- **Projectile Systems:** Reusing bullets or projectiles in a shooter game to minimize memory allocations.
- **Enemy Management:** Reusing enemy objects in games with frequent spawning and destruction, such as in wave-based shooters.
- **Particle Systems:** Reusing particles in effects like explosions or smoke

 to improve performance.

**Example:**
- In a top-down shooter, bullets might be pooled so that when they go off-screen, they are returned to the pool instead of being destroyed and recreated.

---

### **12. Factory Method Pattern**

**Use When:**
- **Object Creation Control:** When you need to delegate the responsibility of creating objects to subclasses or encapsulate object creation.
- **Object Creation Flexibility:** When you want to provide subclasses with a way to choose the type of objects that will be created.

**Common Scenarios:**
- **Weapon Systems:** Creating different types of weapons (e.g., melee, ranged) based on player choice or game events.
- **NPC Generation:** Generating NPCs with different characteristics depending on the game level or environment.
- **Quest Items:** Dynamically creating quest items or objectives based on the current quest stage or player progress.

**Example:**
- In an RPG, a `WeaponFactory` might generate different weapons based on the player’s level or class, encapsulating the creation logic in a single location.

---

### **13. Builder Pattern**

**Use When:**
- **Complex Object Creation:** When you need to create complex objects with many optional parameters or configurations.
- **Object Construction Separation:** When you want to separate the construction of an object from its representation, allowing for different representations of the same construction process.

**Common Scenarios:**
- **Character Creation:** Allowing players to build characters with different attributes, skills, and equipment.
- **Level Generation:** Building complex levels or environments with multiple layers of detail.
- **Dialog Systems:** Constructing complex dialog trees where different responses lead to different outcomes.

**Example:**
- In a character creation system, a `CharacterBuilder` might allow the player to choose attributes, appearance, and skills in a step-by-step process, culminating in the creation of a complex character object.

---

### **Conclusion**

This guide provides a comprehensive overview of when and how to use various game coding patterns depending on common game development requirements. By understanding the strengths and appropriate use cases for each pattern, you can create more maintainable, flexible, and efficient game systems.

**How to Use This Guide:**
- **Identify the Requirement:** Determine the specific game development requirement or problem you're facing.
- **Match the Requirement to a Pattern:** Use this guide to find the most appropriate pattern(s) for that requirement.
- **Implement the Pattern:** Apply the pattern according to the specific scenario in your game, referencing the example scenarios provided.

By keeping this guide handy, you can quickly reference it during your game development process to ensure you're using the right pattern for the job.
