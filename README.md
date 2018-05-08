This is a basic boiler plate repository, containing scripts intended for game development in C Sharp, using UnityEngine. Scripts will be added as I learn to write them, along with a description here in the readme.

### ColorChanger
- Allows the user to change the color of the object that the script is attached to.

### Movescript
- This is the beginnings of a basic move script, allowing the user to move a game object using input keys.

### WorldInteraction
- Allows the player to move their character based on where they click on the map. Assuming the area clicked is "walkable allowed", the object will move to the designated area.
- It also allows the user to interact with the objects in a game world. if a game object with an interaction script is clicked, the moving object will interact with it. (if the player clicks an NPC, Treasure Chest, etc.)

### Interactable
- This is a script that does not get directly attached to any game objects, but is referenced by most if not all of the direct interaction scripts, such as NPC or SignPostInteract. It is the first in a series of functions that denotes which actions lead to which results.

### ActionItems
- The next function in the interaction chain, this function allows interaction with the base class of an interactable object. It helps to denote which interaction script is next in the chain.

### PickUpItem and NPC
- Both of these scripts are, as of now, almost identical. Both of them currently just print a Debug Log denoting which object was selected for interaction.
both of these functions require Interactable after the class is declared, thus denoting their locations in the interaction function chain.


### 
