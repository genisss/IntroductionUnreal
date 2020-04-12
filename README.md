# Unreal Engine Introduction Project
[![](https://img.youtube.com/vi/hDTZva9lSno/0.jpg)](https://youtu.be/hDTZva9lSno)


## Implementacions

**Blueprints:**

 - **3rd person controller habilities**
	 - Decrease size and speed to fit in small gaps
	 - Activate RADAR to see invisible force shield obstacles
- **Evolved Moving Platform blueprint** that doesn't stop and restart when the player enters or exits but it has a trigger outside that force the platform to come back in the case you die as you van see in the video.

**Interfaces:**
 - **Respawn System** using two blueprint interfaces
	- BPI_Checkpoint saves the position of the last checkpoint hte player has gone through
	- BPI_DieArea force the player to teleport to the las checkpoint
 - **Zero gravity area** using triggers that calls a function of the interface BPI_SetGravity implemented by the third person controller which reveices an input to set its value

**Custom Materials**
 - **Force shield material** used in the invisible obstacles

**PostProcess Material**

 - **Outline shader**  with a sphere mask to implement the Radar vision of our player

**Material Parameter Collection:**
- To pass parameters to the force shield material and the radar post processing material to enable/disable them and pass the player position to center the sphereMask.

**Personalized Inputs:**
- 1,2,3  buttons to change hability



