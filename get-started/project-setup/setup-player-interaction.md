---
layout: default
title: Setting up Player Interaction
parent: Project Setup
grand_parent: Get Started
nav_order: 7
---

# Setting up Player Interaction
1. Navigate to the project settings, and then the Input settings in the Engine category.
2. In the action mappings add an action called NextDialog.
    - Set the key bindings to Space Bar/Enter/Left Mouse Button. You can also set it to something completely different if you want.
3. Go to the Blueprints folder into the folder Core.
4. Create a blueprint class that is based on PlayerController and call it BP_IngamePlayerController.
    1. Open the blueprint.
    2. Navigate to the Event Graph
    3. Add the nodes displayed below
    ![Nodes to allow the player to navigate to the next elements in the dialog]({{ site.baseurl }}/assets/images/PlayerController/Next_Dialog_Nodes.png)
5. Open the blueprint BP_InGameGameMode.
    1. Set the Default Player Controller Class to BP_IngamePlayerController.

Now the player should be able to navigate through the visual novel if the key mapping defined above.

The final step is [setting up the memory system]({{ site.baseurl }}{% link get-started/project-setup/setup-memory-system.md %}).