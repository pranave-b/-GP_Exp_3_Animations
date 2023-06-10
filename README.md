# GP_Exp-3_Animations
# Experiment:03 – Change the third person character mesh and add animations.
### AIM:
To Change the third person character mesh and add animations.
### ALGORITHM(for change the third person character mesh):
```
step1. Import the new character mesh:
o	Open your project in Unreal Engine.
o	Go to the Content Browser.
o	Right-click in the desired folder and select Import.
o	Locate and select your new character mesh file.
o	Configure the import settings as needed.
o	Click Import to bring the mesh into your project.
step 2.	Create a new Blueprint based on the Third Person Character template:
o	In the Content Browser, right-click in the desired folder.
o	Select Create Basic Asset > Blueprint Class.
o	In the Class Settings window, search for "Third Person Character" and select it as the parent class.
o	Name the Blueprint and click Create.
step 3.	Set up the character skeleton and mesh:
o	Open the newly created Blueprint.
o	In the Blueprint editor, find the Components panel on the left.
o	Locate the Mesh component.
o	In the Details panel on the right, under the Mesh section, click the dropdown menu for Skeletal Mesh.
o	Select your imported character mesh from the list.
step 4.	Adjust the collision capsule:
o	In the Components panel, find the Capsule Component.
o	Adjust the Capsule Half Height and Radius properties to fit your new character mesh.
o	This ensures that the character's collision capsule matches the new mesh.
step 5.	Test the character:
o	Compile and save the Blueprint.
o	Drag and drop the character Blueprint into the level or set it as the default character in your game mode.
o	Play the game to test the character with the new mesh.
```



 
### ALGORITHM(for adding animation):
```
step 1.	Import the animation assets:
o	Open your project in Unreal Engine.
o	Go to the Content Browser.
o	Right-click in the desired folder and select Import.
o	Locate and select your animation files.
o	Configure the import settings as needed.
o	Click Import to bring the animations into your project.

step 2.	Create an Animation Blueprint:
o	In the Content Browser, right-click in the desired folder.
o	Select Animation > Animation Blueprint.
o	In the Pick Parent Class window, search for "ThirdPersonCharacter" and select it as the parent class.
o	Name the Animation Blueprint and click Create.

step 3.	Open the Animation Blueprint:
o	Double-click the Animation Blueprint you just created to open it in the Animation Blueprint editor.

step 4.	Set up the Event Graph:
o	In the Animation Blueprint editor, locate the Event Graph tab.
o	Right-click in the graph and search for "Update Animation."
o	Add the Update Animation node to the graph.

step 5.	Set up the Anim Graph Update:
o	Drag off the Update Animation node and search for "Set Anim Graph Update Rate."
o	Connect the Set Anim Graph Update Rate node to the Update Animation node.

step 6.	Create animation states:
o	Right-click in the graph and search for "Add State."
o	Create animation state nodes for each animation you want to use (e.g., Idle, Walk, Run, Jump, etc.).

step 7.	Connect the animation states:
o	Connect the animation state nodes to the output of the Update Animation node.
o	Use appropriate transitions between the animation states to define the character's animation flow.

step 8.	Assign animation assets:
o	In the Animation Blueprint editor, switch to the AnimGraph tab.
o	Drag and drop your imported animation assets into the graph.
o	Connect the animation assets to the appropriate animation state nodes.

step 9.	Test the character animations:
o	Compile and save the Animation Blueprint.
o	Go back to the character Blueprint.
o	In the Components panel, find the Mesh component.
o	In the Details panel, under the Mesh section, find the Anim Class property.
o	Assign the Animation Blueprint you created to the Anim Class property.

step 10.	Create a state diagram (optional):
•	To visualize the animation state flow, you can create a state diagram.
•	In the Animation Blueprint editor, go to the AnimGraph tab.
•	Right-click in the graph and select Create State Machine.
•	Name the state machine and click Create.
•	Drag and drop the animation state nodes onto the state machine graph.
•	Connect the nodes with transitions to represent the animation flow.

step 11.	Test the character with animations:
•	Compile and save both the character Blueprint and Animation Blueprint.
•	Drag and drop the character Blueprint into the level or set it as the default character in your game mode.
•	Play the game to test the character with the new mesh and animations.

```
 


### Result:
Thus, third person character mesh has been changed and added animations.
