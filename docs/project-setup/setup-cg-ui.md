---
layout: single
title: Setting up the CG UI
permalink: /docs/project-setup/setup-cg-ui/
toc: true
sidebar:
  nav: "docs"
---


1. Go to the Blueprints folder into the folder UI, and in there in the folder called InGame
2. Create a blueprint class that is based on BaseCgDisplayWidget and call it W_CgDisplayWidget.
    1. Open the widget
    2. Design the widget however you like
        - Add a image block to the widget named CgImage.
        - Add a image block to the widget named CgImageForTransition.
3. Open the blueprint BP_InGameHud.
    1. Add the component Dialog Image Controller
    2. In the settings of the component set the Cg Display Widget Class to W_CgDisplayWidget

Everytime a CG is displayed, the above created widget will be used to display the CG. If you intend to always display something additional with a CG, this can be used to set this up as well.

Next up is [setting up the scene background UI]({{ site.baseurl }}{% link docs/project-setup/setup-scene-background-ui.md %}).