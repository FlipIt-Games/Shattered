# Gunner Enemy

An enemy holding a range weapon. He tries to find a line of sight to the player (where he would not shoot his friends) using a grappling hook to quickly reposition then loads his weapon and shoot.

## Behaviour

- If he has a line of sight onto the character he will load his weapon
- Once he started loading his shot, he won't stop
- If he doesn't have a line of sight he will move and use his grappling hook to reposition
- If there are no los available because the player is surrounded he will stay in idle

- If the character enters is avoidance radius, he will move to a safer spot 

## Exposed Parameters
- Damage
- ProjectileSpeed
- ChargeTime: The time it takes to load is shoot
- Hitscan/Projectile Toggle
- Avoidance Range