# StaticChargeSystem

# Static Charge System

An add-on mechanic for Roll-a-Ball games. The player builds static energy while rolling and releases it to push objects, activate switches, and open gates.

## Features
- **Static Charge:** builds over 5 s of movement, press `E` to release a pulse.  
- **Movable Boxes:** pushed away by the pulse.  
- **Switches:** activate when hit by a pulse (change color).  
- **Gates:** open when linked switches activate.

## Setup
1. Add **StaticCharge.cs** to your Player and assign `mat_Default` + `mat_Charged`.  
2. Place **StaticSwitch**, **StaticGate**, and **StaticMovableBox** prefabs in the scene.  
3. Link each switch’s **Linked Gate** field in the Inspector.  
4. Tag movable cubes as `"Movable"`.  
5. Play → roll for ~5 s → press `E` to pulse.

## Folder Structure
StaticChargSystem/
- Materials/
- Prefabs/
- Scripts/

## Notes
- Pulse range controlled by `pulseRadius` in **StaticCharge.cs**.  
- Pulse affects any collider with the `"Movable"` tag or a `StaticSwitch` script.
