# Jumper Enemy

This is enemy takes leaps over his allies to get close to the character. He creates an area of effect at the point of impact, dealing more damage if it is a direct hit.

This enemy is particularly agressiv and will attack the character even if he is already in contact with many enemies. 
He leap also affects nearby allies pushing them away.

## Behaviour

- He will perform a melee attack if the player is in range of melee attack
- Otherwise he will either move of take a leap depending of the distance to the character 
- Otherwise he move toward the character until being in leap range

## Exposed Parameters
- MeleeDamage
- LeapAoeDamage
- LeapDirectHitDamage
- MaxLeapRange
- MinLeapRange
- LeapSpeed