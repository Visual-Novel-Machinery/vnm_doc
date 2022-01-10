---
layout: default
title: Initial Setup
parent: Project Setup
grand_parent: Get Started
nav_order: 1
---

# Initial Setup
1. Download the plugin from Gumroad or the Unreal Marketplace
2. Create a Project in Unreal Engine 4. Use the blank template.
3. Copy the plugin in the Plugins folder in the root folder of the project.
    - Path should then be \<path to root\>/Plugins/VisualNovelMachinery/
    
    ![Plugin Folder location and content]({{ site.baseurl }}/assets/images/InitialSetup/PluginFolder.png)
4. Compile and start up the project.
5. Create the following folders in the root folder: Art, Blueprints, Data, Dialogs, Maps
    - You don't need to use the proposed structure mentioned above, the rest of the guide will however use it.
    
    ![Project Folder Structure]({{ site.baseurl }}/assets/images/InitialSetup/ProjectFolderStructure.png)

You should now have the absolute base setup for the project. Next step is to setup all the data tables used, as Visual Novel Machinery is setup in a data-driven way. Let's move on to [setting up the data tables]({{ site.baseurl }}{% link get-started/project-setup/setup-data-tables.md %}).