Stealth Detection Example
=============

This is a simple example project which could be used as a starting point for a stealth game where the player hides from AIs in shadowed areas.
For nostalgic fun, the project includes a light gem showing how visible the player would be to enemy threats.

The project contains two light blueprints and a modified third person player blueprint. When the player enters a light source (spot or point) the light is registered with the player. The player then determines how much light is at his current position based on the lights he is intersecting. An accumulation of light is made, and a final output float between 0.0 and 1.0 is set, 0.0 being darkness, and 1.0 being fully lit. The HUD then updates the alpha of the gem to show the player his current light level.

This project does not contain any AIs to test the detection with, as that is more of a game specific mechanic. A simple implementation however could be made with a simple pawn and a pawn sensing component. When a pawn is sensed, have detection timers which increase depending on light levels.

![alt tag](/ContentSrc/Screenshots/less_light.jpg?raw=true "Low Light Area")
![alt tag](/ContentSrc/Screenshots/more_light.jpg?raw=true "High light area")
