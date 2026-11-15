For this plug in to work, there is a few steps the user must take: Go to Edit > Project Settings and search "Tag". This will bring up the gameplay tag section where you need to click "Manage Gameplay Tags..." and add a new one called "Movable".

![[NewTag.png]]

Once you have made this tag, go to the actor component: "AC_Movable" and open up the event graph. Here, you want to ensure the "TagContainer" variable is holding the "Movable" tag you just made. Also, in the "ADD" node, double check that it also holds the "Movable" tag.

![[TagChecks.png]]

Then head to the main blueprint, "BP_WindFan" and go to this area. Just ensure that the "Actor Has Tag" node is holding the correct "Movable" tag. Once this is done, you should be good to go!

![[ActorHasTagCheck.png]]