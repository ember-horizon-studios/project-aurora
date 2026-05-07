### 1. Mechanical (The "Verb" Layer)

These are the most important for your **Gray Box**. If these don't feel good with a cube, the game fails.

- **Locomotion:** Walking, dashing, climbing, swimming, or vehicle handling.
    
- **Combat:** Melee swings, projectile logic, hit detection, or combo systems.
    
- **Interaction:** Generic systems for "using" things (buttons, doors, picking up items).
    
- **Abilities/Skills:** Active powers with cooldowns or resource costs (e.g., "Fireball," "Stealth").
    

### 2. Systems (The "Logic" Layer)

These are the invisible rules that govern the world.

- **Economy:** Shops, currency types, and resource scaling.
    
- **Progression:** XP, leveling, talent trees, or unlockable upgrades.
    
- **AI/Behavior:** Enemy pathfinding, state machines (Idle/Alert/Attack), or boss patterns.
    
- **Inventory/Storage:** How items are held, stacked, and discarded.
    

### 3. Environmental (The "Space" Layer)

This is where you define the world the player inhabits.

- **Level Design:** Specific room layouts, hazards (lava, spikes), or platforming challenges.
    
- **Hazard/Obstacle:** Static or moving objects that hinder the player.
    
- **Wayfinding:** Map systems, compasses, or environmental cues (lighting/breadcrumbs).
    
- **World State:** Day/night cycles, weather effects, or destructible environments.
    

### 4. Technical (The "Engine" Layer)

These often stay "under the hood" but are vital for an **MVP** to be playable.

- **Save/Load:** Persistence of player data and world state.
    
- **Input/Control:** Controller support, remapping, and sensitivity settings.
    
- **Performance:** Optimization systems (LODs, culling, loading screens).
    
- **Integrations:** Steam API, Achievements, or multiplayer networking.
    

### 5. Sensory (The "Polish" Layer)

These are strictly **MVP** and beyond. If you find yourself working on these during the Gray Box phase, you're "scope creeping."

- **Visual FX (VFX):** Particles, screen shakes, and post-processing.
    
- **Audio (SFX):** Sound triggers, spatial audio, and background music.
    
- **Narrative/Writing:** Dialogue systems, lore entries, and quest text.
    
- **User Interface (UI):** Health bars, menus, and inventory screens.