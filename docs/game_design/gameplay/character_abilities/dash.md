# Character Dash

## Inputs

### Action
**Type:** Trigger

**Gamepad Control:** Button South

**Keyboard & Mouse:** TBD


### Direction
**Type:** Vector2

**Gamepad Control:** Left Stick

**Keyboard & Mouse:** TBD

## Description
The character gets a burst of speed and performs a quick forward movement, allowing him to dodge enemy attacks or reposition himself

The dash ability is made up of 3 stages: 

1. ### Charging 
- The character enters this stage when the Action is triggered
- The character's [movement abilities](move.md) gets locked (he doesn't move anymore). 
- Direction is recorded, if no direction is provided the current orientation of the character is used
- If the player press the [light attack](light_attack.md#action) action he then performs a [dash attack](dash_attack.md)

2. ### Dashing
- Direction gets locked and the input is no longer recorded
- The character is invulnerable
- The player moves according to the direction

3. ### Recovering
- The momentum of the character gradually slows down to reach [movement's MaxSpeed](move.md)
- The player gradually recovers control over the [character's movement](move.md)

## Exposed Parameters

- ChargeTime
- DashTime
- RecoveryTime
- Distance: The distance travelled during the dashing stage