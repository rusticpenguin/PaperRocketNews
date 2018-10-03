![PaperRocketLogo](https://user-images.githubusercontent.com/38636581/46249711-d8b05b00-c3ea-11e8-9c22-fb3fb92744ae.png)

___
# Project: PaperRocket
A 3D RPG with paper aesthetics. 

[1-Minute Trailer](https://www.youtube.com/embed/i-gHQyJWCEI)
___

## Table of Contents:
1. [Story](#story)
2. [Gameplay Ideas](#gameplay-ideas)
3. [Characters](#characters) 
4. [Code Meta](#code-meta)
5. [Known Bugs](#known-bugs)
6. [Technologies Used](#technologies-used)
7. [The Team](#the-team)

___

## Story
``` 
Prologue:
    The story starts off with Eden flying through space. His ship is struck by Meteor and they crash land on Vellum. Eden meets Meteor who apologizes for crashing his ship. They set out to find someone to help them. Arriving at a town of Penguins they walk around and talk to different penguins to figure out where they need to go. Next town over lives a Scientist who builds rockets.
    
    With this newfound knowledge Eden and Meteor set out to the next town which has been overrun by Robots. After fending off a few robots, they are challenged by the Lead Robot. Upon defeating the Lead Robot, all the robots flea. They talk to the Scientist who requires a handful of materials. Eden and Meteor set out to retrieve them.
    
    Bringing back the materials the Scientist and the Penguins help rebuild the rocket ship. The Scientist notices that the ship is missing it's main power source (Petals?). Informing Eden and Meteor that the rocket ship will not be able to escape the atmosphere without recovering their lost power source.
    
End of Prologue;

Chapter 1:
---
End of Chapter 1;
```

___

## Gameplay Ideas

#### Turn Based Combat
1. Player selects their move
2. Given a quick time event to decide on damage/effectiveness
3. Enemy now selects a move
4. Player has a small window to parry/block an enemy's attack
 
#### Skill Tree
* Player levels up and can increase Health/Damage/Abilities
* Depending on level/chosen stat augmentations skills will be added

#### Outfits
* Change the player's outfit with costumes that can be bought with nickels
___

## Characters

#### Eden
![Eden](https://user-images.githubusercontent.com/38636581/46249691-a272db80-c3ea-11e8-97f3-fb77c6576690.png)\
An astronaut on his way home from a journey. Hit with a touch of misfortune he now has to get home.

#### Meteor
![Meteor](https://user-images.githubusercontent.com/38636581/46249731-3ba1f200-c3eb-11e8-9a6f-bc9ea57716c7.png)\
Traveling with their family through space, Meteor accidentally strikes Eden's ship from the sky. They desperately wants to get back into space to reunite with their family.
___

## Code Meta
These are rough rules to help keep the code organized so new team members can work on the project without having to decipher other member's code. Will add more as I think of them.
#### Interactions:
```
    Keep all interactions inside of the respectable Object.
        e.g. If the Player is going to take damage, keep the interaction within player.
        Or if the Player wants to TRIGGER an NPC's dialogue, keep the trigger inside of the NPC.
```

#### Update/FixedUpdate:
```
    Anything that has to do with movement/animations should be stored inside the FixedUpdate() method. Everything else should be stored within the Update/LazyUpdate method.
    
    Only methods should be inside of either Update calls to reduce clutter. Refactor your code into functions with descriptive name.
```

#### FindObjectOfType:
```
    This is a taxing call and should ONLY be used in the Start function. Use sparingly and try to find ways around using this method.
    
    Alternatives include:
        1. Creating public variables of the desired object
        2. Using parent/child objects
        3. Sending a message with the desired function (e.g. SendMessage("Destroy") to trigger Destroy()) to the 
            object in a OnTrigger/OnCollision 
```
___

## Known Bugs

* A Button on title screen does not work (Controller)

___

## Technologies Used

* [Unity3D](https://unity3d.com/) - Game Engine
* [Blender](https://www.blender.org/) - 3D Modeling
* [Photoshop CC](https://www.adobe.com/products/photoshop.html) - 2D Art and Textures 

___

## The Team

 - [George Chios (Me)](https://github.com/rusticpenguin/)
