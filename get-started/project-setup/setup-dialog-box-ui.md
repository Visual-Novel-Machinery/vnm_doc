---
layout: default
title: Setting up the Dialog UI
parent: Project Setup
grand_parent: Get Started
nav_order: 3
---

# Setting up the Dialog UI
1. Go to the Blueprints folder and create a folder called UI, and in there a folder called InGame. Enter that folder.
    
    ![UI Folder Structure]({{ site.baseurl }}/assets/images/DialogBoxSetup/UIFolderStructure.png)
2. Create a blueprint class that is based on BaseDialogBoxWidget and call it W_DialogBoxWidget.
    1. Open the widget
    2. Design the widget however you like
        - Add a rich text block to the widget named DialogText
            - Set its text style set to DT_DialogTextStyles
        - Add a rich text block to the widget named CharacterNameText
            - Set its text style set to DT_DialogTextStyles
        
        ![Dialog Box UI Design]({{ site.baseurl }}/assets/images/DialogBoxSetup/DialogBoxDesign.png)
    3. Add a row called "Default" to DT_DialogTextStyles and customize it to your liking. This will be how your dialog text gets displayed without any tags.
        
        ![Dialog Text Default Row]({{ site.baseurl }}/assets/images/DialogBoxSetup/DialogTextCustomizationDefault.png)
3. Create a blueprint class that is based on BaseChoiceButton and call it W_ChoiceButton.
    1. Open the widget
    2. Design the widget however you like
        - Add a button to the widget named ChoiceButton
        - Add a text block to the widget named ChoiceText
        
        ![Choice Button UI Design]({{ site.baseurl }}/assets/images/DialogBoxSetup/ChoiceButtonDesign.png)
4. Create a blueprint class that is based on BaseChoiceWidget and call it W_ChoiceWidget.
    1. Open the widget
    2. Design the widget however you like
        - Add a vertical/horizontal/... box to the widget named ChoiceButtonsList
        
        ![Choice Widget UI Design]({{ site.baseurl }}/assets/images/DialogBoxSetup/ChoicesWidgetDesign.png)
    3. In the settings of the widget set the Choice Button Class to W_ChoiceButton
        - ![Choice Widget Settings]({{ site.baseurl }}/assets/images/DialogBoxSetup/ChoiceWidgetSettings.png)
5. Create a blueprint class that is based on HUD and call it BP_InGameHud.
    1. Open the blueprint
    2. Add the component Dialog Controller
    3. In the settings of the component set the Dialog Box Widget Class to W_DialogBoxWidget
    4. In the settings of the component set the Dialog Box Widget Class to W_ChoiceWidget
    
    ![Dialog Controller Settings]({{ site.baseurl }}/assets/images/DialogBoxSetup/DialogControllerSettings.png)
6. Navigate back up to the Blueprints folder and create a folder called Core. Enter that folder.
    - ![Core Folder Structure]({{ site.baseurl }}/assets/images/DialogBoxSetup/CoreFolderStructure.png)
7. Create a blueprint class that is based on BaseGameMode and call it BP_InGameGameMode
    1. Open the blueprint.
    2. Set the default hud class to W_InGameHud
    
    ![InGame Game Mode Settings]({{ site.baseurl }}/assets/images/DialogBoxSetup/InGameGameModeSettings.png)
8. Navigate to the Maps folder
9. Create a new blank map and call it InGameLevel
    1. Open the level
    2. Open the World Settings Panel
    3. Set the Game Mode Override to BP_InGameGameMode
    
    ![InGameLevel World Settings]({{ site.baseurl }}/assets/images/DialogBoxSetup/InGameMapSettings.png)
10. Create a new blank map and call it MainMenu
11. Go to the project settings and navigate to maps & modes
    - Set the Game Default Map to MainMenu
12. Navigate to the Visual Novel Machinery in the plugins category
    - Set the Main Menu Level Name field to MainMenu
    
    ![Main Menu Level Settings]({{ site.baseurl }}/assets/images/DialogBoxSetup/MainMenuLevelNameSetting.png)

Next up is [setting up the character UI]({{ site.baseurl }}{% link get-started/project-setup/setup-character-ui.md %}).