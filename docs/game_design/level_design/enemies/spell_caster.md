# Spell Caster Enemy

This enemy throws various buffs and healing to his allies. 
Certain buffs and healing can be intercepted when damaging the receiver in a short time frame
Intercepting the spell reverts the effect on the original receiver and applies it to the character

He can only use one spell at a time and has to refill his energy between spells. In order to cast a spell he has to have a line of sight onto the target and the target must be in range.

## Spells

There are two types of spells:
- Continuous: A link between the caster and its target. The effect applies until LOS is broken or the max duration is exceeded. Continuous spells can't be intercepted.
- Trigger: The caster has to have los in order to cast it. But the effect remains if the LOS is broken once casted. Can be intercepted. Triggered spells also have a cast time.

The caster can't move both when he his casting or holding a continuous spell.

### Heal

**Type:** Trigger

- Used on allies that are damaged and not in contact with the player
- Gives back healing to the receiver

#### Parameters
- HealPoint:

### Shield

**Type:** Continuous

- Used on allies that are in contact with the character
- Wraps the receiver in a protective bubble, denying every damage
- The shield has an health value. When it reaches 0, the spell is broken and both the target and the caster gets stunned.

#### Parameters
- MaxDuration
- StunDuration
- ShieldHealth

### Speed Boost

**Type:** Trigger

- Used on allies that are either trying to fly from the character or to get in attack/ability range
- Increases the move speed of the target

#### Parameters
- Value: The pourcentage of speed gained 
- Duration

### Damage Boost

**Type:** Trigger

- Used on allies that are either in contact with the player or are close to get in range of attack/ability
- Increases the damage dealt by the target

#### Parameters
- Value: The pourcentage of damage gained 
- Duration

### Sacrifice

**Type:** Continuous

- Used on basic enemies when there are many enemies around the character
- After a certain amount of time the target explodes creating an area of effect at the position of the target

#### Parameters
- LoadDuration
- ExplosionRadius
- Damage

## Behaviour
- If the player enters his avoidance range, he will try to find a safe spot.
- If he is safe he will move to find LOS to cast spells

## Exposed Parameters
- SpellCooldown
- SpellRange
- InterceptionWindow: The time after which an interceptable spell can't be intercepted anymore 