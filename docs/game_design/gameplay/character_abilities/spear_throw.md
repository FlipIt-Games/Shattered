# Character's Spear Throw

## Inputs
### Aim

**Gamepad Control:** Button East

**Keyboard & Mouse Control:** TBD

**Type:** Button

### Direction

**Gamepad Control:** Left Stick

**Keyboard & Mouse Control:** TBD

**Type:** Vector2

## Description

This action is performed when the character holds its spear. Otherwise see [Spear Recall](spear_recall.md)

The character throws its spear in the direction he is looking, snapping to the enemy closest to its aiming direction. The spear then falls on the ground behind the affected enemy.

The throw is composed of two stages:
1. Aiming
- The character stays into this stage while the aim input is pressed
- The [Direction](#direction) is recorded
- The character [movement speed](move.md) gets multiplied by a factor
- If the player only performs a quick tap on the Aim input, the character skips this stage and goes straight to the throwing stage
- If the player keeps pressing the button for a certain amount of time, he will perform a heavy shot, dealing more damage and throwing the spear farther
1. Throwing
- The character enters this stage upon releasing the Aim input
- The spear gets thrown according to the Direction input
- The spear distance and damage are relative to the time the character stayed in aiming phase

## Exposed Parameters
- Light Shot Distance
- Light Shot Damage
- Heavy Shot Distance
- Heavy Shot Damage
- Travel Speed
- ChargeTime: The time the player must keep the input pressed in order to perform a heavy shot 