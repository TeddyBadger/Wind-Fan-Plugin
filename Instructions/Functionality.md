
The first part of the event graph is this small section that simply takes whatever actor has entered the collision box, checks if it has the appropriate tag, and then adds it to the array to be affected. Although it is quite simple, something to look out for is if there are any spelling errors in the tag name, as if it doesn't exactly match, it will not add the actor to the array.
![[AddingToArray.png]]

---

Something else that is needed at the start is the 