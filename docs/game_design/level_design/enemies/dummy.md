# Dummy Enemy

This enemy is just wandering in the arena and serves as a waypoint for the player to chain dash attacks.

He is not agressive and will only attack if the character stands still next to him.

The dummy gets assigned to an area in which he wanders randomly. When he dies, another one will respawn after a short amount of time.


## Behaviour
- The dummy walks to a random point inside of his affected area, when he reaches it, he rests for a bit then walks towards another random point
- When the player stays within attack range for a certain amount of time, the dummy then performs a slow attack. When the player leaves his affected area, the dummy exits its attacking state and goes back to wandering

## Parameters
- Damage
- RespawnTime: The time after which a new dummy will respawn when one dies in the assigned area
- AttackDelay