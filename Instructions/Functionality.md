
The first part of the event graph is this small section that simply takes whatever actor has entered the collision box, checks if it has the appropriate tag, and then adds it to the array to be affected. Although it is quite simple, something to look out for is if there are any spelling errors in the tag name, as if it doesn't exactly match, it will not add the actor to the array.
![[AddingToArray.png]]

---

Something else that is needed at the start is the handling of the particle effects: the initial state of particles is set at the start of the game, and then it is set again when force is applied to make sure it matches the appropriate force that the fan is outputting.
![[ParticleSystemSetup.png]]