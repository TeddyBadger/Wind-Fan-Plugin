
The first part of the event graph is this small section that simply takes whatever actor has entered the collision box, checks if it has the appropriate tag, and then adds it to the array to be affected. Although it is quite simple, something to look out for is if there are any spelling errors in the tag name, as if it doesn't exactly match, it will not add the actor to the array.
![[AddingToArray.png]]

---

Something else that is needed at the start is the handling of the particle effects: the initial state of particles is set at the start of the game, and then it is set again when force is applied to make sure it matches the appropriate force that the fan is outputting.
![[ParticleSystemSetup.png]]

---
The main section begins with re-setting the state of the particles to match the force applied, then it uses a for loop to affect the whole array and only the objects in the array.
![[ForceAppliedSetup.png]]

---
Once it is set to cycle through the array, it checks if the object is a character: This part is if it wants to push or pull the character.
![[TheActorIsPlayer.png]]

---
If the "IsCharacter?" check is false, it turns to this section to push whatever other objects are in the array. The difference is needed as pushing an object requires a different component reference than pushing the character.
![[TheActorIsNOTPlayer.png]]