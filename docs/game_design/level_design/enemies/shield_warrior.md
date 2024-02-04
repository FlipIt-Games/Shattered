# Shield Warrior Enemy

This enemy is a variant of the [Warrior](warrior.md) carrying a shield. 

## Behaviour
- If there are [grenadiers](grenadier.md) or [spell casters][spell_caster.md] in the arena he try to protect one of them, placing himself between the character and the selected ally.
- If his selected allies dies, he will select the nearest one if applicable
- If he is not protecting anyone, he will chase the player until reaching shield bash range
- He will shield bash the player if in range and has Los
- He will attack the character if he is in range of melee weapon


## Exposed Parameters
- ShieldBashDamage
- ShieldBashDistance
- PlayerStunDuration