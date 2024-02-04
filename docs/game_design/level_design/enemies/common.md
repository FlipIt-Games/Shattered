# Common Enemies States and Parameters

*Unless specified, the following applies for every type of enemy*

## Global Parameters
Poise Regen start off: The time before the poise regeneration starts off after not being hit (Being hit resets the timer at 0)

## Common Parameters
- Movement speed
- Max health points
- Weight: A factor multiplying the amount of knockback dealt by player attacks, the higher, the less the enemy will move when hit.
- Poise: The amount of “Stagger Damage” the enemy can handle before being interrupted
- Poise Regeneration Per Second: The amount of poise the enemy regenerates every second after regen starts off
- Staggered Duration: The duration of the staggered state of the enemy

## Core States
- Idle: In this state the enemy stands still and is not doing anything. He can transition
- Dead: In this state the enemy can’t do anything anymore and his body lies down until the end of the wave. The enemy enters this state whenever his health reaches 0.
- Staggered: The enemy enters this state whenever his poise reaches 0. The enemy gets his current action interrupted and is affected by the knockback dealt by the player at full scale (ignoring his knockback resistance). 
