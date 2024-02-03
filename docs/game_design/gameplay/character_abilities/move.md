# Character Movement

## Input
### Direction
**Gamepad Control:** Left Stick

**Keyboard & Mouse Control:** TBD

**Input Type**: Vector2

### Description

The character moves according to the input direction.

## Exposed Parameters
- MaxSpeed: The max speed the character can reach while normalling running
- AccelerationTime: The time it takes for the character to get from 0 to MaxSpeed when the input is uninterruptedly pressed at max
- BrakeTime: The time it takes for the character to get from MaxSpeed to 0 when no input is recorded
- TurnTime: The time it takes for the character to get from MaxSpeed to MaxSpeed in the opposite direction

## Additional Requirements
- Movement speed should scale according to the input value. If the player sends (0.5, 0) the character should move at half the MaxSpeed
- The movements should be relative to the camera rotation. If the input says left, character should move to what the player perceives as left
- When the player quickly change sends an opposite direction (going from (1, 0) (-1, 0)) the character should perform a quick turn and should take the TurnTime parameter into account
