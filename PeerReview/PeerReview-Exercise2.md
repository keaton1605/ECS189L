# Peer-Review for Programming Exercise 2 #

# Solution Assessment #

## Peer-reviewer Information

* *name:* [Keaton Elliott] 
* *email:* [kecelliott@ucdavis.edu]

## Solution Assessment ##

### Stage 1 ###

- [x] Perfect
- [ ] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justifaction ##### 
The camera locks on the player as they move around. The correct lines are displayed when draw logic is true, and there are no serialized fields.

___
### Stage 2 ###

- [ ] Perfect
- [ ] Great
- [x] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justifaction ##### 
The DrawLogic and serialized fields work as they should. If the player hits the edge of the screen, they move at the same speed as the screen. However, the player can still move past the edge of the screen if they attempt to move in the opposite direction of the screen motion. They will get moved back if they stop pressing the left direction. Also the natural movement at this edge is slightly jerky, meaning the speed of the target and camera are probably slightly different.

___
### Stage 3 ###

- [ ] Perfect
- [x] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justifaction ##### 
The camera lerps behind the player as the player moves. It catches up with the player after the lerp duration. The movement of the camera takes a second to update, but this seems to just when the update function is called.

___
### Stage 4 ###

- [x] Perfect
- [ ] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justifaction ##### 
The player follows the camera correctly, and it takes the lerp duration to get back. The lerp also successfully only affects the x and y axes.

___
### Stage 5 ###

- [ ] Perfect
- [ ] Great
- [x] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justifaction ##### 
At small push ratios, the speed up push box works, but the edges of the box are inside the actual Draw Logic. When the push ratio is increased, the camera essentially lerps behind the player until it hits the edge, and at that point the player sticks to the edge. Also, the camera lerps back to centered on the player when the player stops moving, which is a nice extra feature.

___
# Code Style #


### Description ###
The style overall in this code follows the guide very well. There are plenty of examples of good use of (var) instead of setting the variable to something, like the following.
* [good variable description](https://github.com/ensemble-ai/exercise2-cameracontroller-MichaelCordero98/blob/5e88de534819b87e3453640b21f469b3bc0cdd1a/Obscura/Assets/Scripts/TargetFocusLerpCamera.cs#L31)
* [another good variable](https://github.com/ensemble-ai/exercise2-cameracontroller-MichaelCordero98/blob/5e88de534819b87e3453640b21f469b3bc0cdd1a/Obscura/Assets/Scripts/FourWaySpeedupPushZoneCamera.cs#L30)

Also the functions are described well and the spacing is uniform throughout all the code. This can be seen with the indentation and the location of the brackets in the functions, like here.
* [correct bracket](https://github.com/ensemble-ai/exercise2-cameracontroller-MichaelCordero98/blob/5e88de534819b87e3453640b21f469b3bc0cdd1a/Obscura/Assets/Scripts/TargetFocusLerpCamera.cs#L30)

___

# Best Practices #

### Description ###

The comments about this code are well placed and do a good job of conveying the meanings of the simple functions and variable definitions. They are also well spaced and don't contribute too much clutter in their concise natue.
* [short/helpful comment](https://github.com/ensemble-ai/exercise2-cameracontroller-MichaelCordero98/blob/5e88de534819b87e3453640b21f469b3bc0cdd1a/Obscura/Assets/Scripts/TargetFocusLerpCamera.cs#L40) Although this comment is misspelled, it conveys what it is trying to say very well.

The spacing between and surrounding parentheses is uniform and makes if statements and other functions easy to follow.
* [uniform parentheses](https://github.com/ensemble-ai/exercise2-cameracontroller-MichaelCordero98/blob/5e88de534819b87e3453640b21f469b3bc0cdd1a/Obscura/Assets/Scripts/FrameAutoScrollCamera.cs#L30)

