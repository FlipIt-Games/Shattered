# Character Light Attack

## Input

### Action

**Gamepad Control:** Button West

**Keyboard & Mouse Control:** TBD

**Type:** Trigger

### Description

The character gives an horizontal slash attack, swiping its spear from right to left. If he follows up with another light attack, the character then swipes from left to right.

The light attack should be broken in three phase
1. Charging: The character charge its attack. 
2. Attacking: The character swings its spear horizontally
2. Recovering: The character gets it’s spear back in idle state

- While in any of the stages above, the [movement's](move.md) gets scaled by a factor.
- If the player chains multiple attacks, the recovery stage acts as the charging phase for the next one

### Exposed Parameters
- Damage
- ChargeTime
- RecoveryTime
- MovementScale
