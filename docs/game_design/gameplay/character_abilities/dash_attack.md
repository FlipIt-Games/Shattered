# Character's Dash Attack

## Input

### Action

**Gamepad Control:** Button South + Button West

**Keyboard & Mouse:** TBD

**Type:** Trigger

### Direction

**Gamepad Control**: Left Stick

**Keyboard & Mouse Control**: TBD

**Type:** Vector2

## Description

The character performs a [Dash](dash.md) towards the most relevant enemy according to its direction and perform a [light attack](light_attack.md) at the same time, inflicting damage upon landing.

- The dash stops in front of the target enemy
- The dash has no recovery phase, allowing the player to chain dash attacks between multiple enemies

- If the system can't find a relevant target the character enters a "stunned" state during which he can't use any of its abilities

## Exposed Parameters
- [Light Attack Parameters](light_attack.md#exposed-parameters)
- [Dash Parameters](dash.md#exposed-parameters)
- Stunt Duration