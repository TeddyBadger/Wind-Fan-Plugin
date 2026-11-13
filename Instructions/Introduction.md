This plug-in contains an actor blueprint; an actor component and a Niagara particle system that gives the wind fans the appropriate wind effect.

---

The main actor: "BP_WindFan" has many variables that allows the user to control parts of it without going into detail of how the graph works etc. These variables are:

| **Variable Name** | **Variable Type** | Read Only? |                                         **What it does**                                          |
| :---------------: | :---------------: | :--------: | :-----------------------------------------------------------------------------------------------: |
|      Length       |       Float       |     No     |                    This controls the length of the area that force is applied                     |
|     Strength      |       Float       |     No     |                          This controls the strength of the force applied                          |
| CharExtraStrength |       Float       |     No     | This is a separate strength that only applies to the player on top of the other strength variable |
|        On?        |      Boolean      |     No     |                          This controls whether the wind fan is on or off                          |
|       Push?       |      Boolean      |     No     |                       This controls whether the force is pushing or pulling                       |
|     Direction     |      Vector       |    Yes     |  This cannot be changed as it is set to be changed to whatever value is perpendicular to the fan  |
There are two other variables used in this blueprint, however these cannot be seen in the engine as they are only used within the event graph to allow them to work as intended. These are: "Negative" which is a constant set to -1, used in some of the equations; and "OverlappingActors" which is an array that contains all the actors within the collision box that have the "Movable" tag.