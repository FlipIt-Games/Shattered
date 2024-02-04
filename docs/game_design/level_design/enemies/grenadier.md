# Grenadier Enemy

This enemy throws grenades over his allies, creating an area of effect at the point of impact, dealing more damage if the projectile is a direct hit.

## Behaviour

- If the character is out of range, he will walk toward him until the character is at 75% of his max range.
- If the character is in range of attack he will charge, then launch a grenade at the character position, then wait for a bit
- If the character enters its avoidance radius 

## Exposed Parameter
- DirectHitDamage
- AoeDamage
- ExplosionRadius: The range in which the player take damage from the explosion
- ProjectileSpeed
- ProjectileRange
- FireRate
- AvoidanceRadius