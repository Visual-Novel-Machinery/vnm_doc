---
layout: posts
title:  "Visual Novel Machinery 1.7 Released"
excerpt: Visual Novel Machinery 1.7 has been released
categories:
  - release
tags:
  - release
---

Changelog:
- Added Auto Mode so that text can be played automatically
  -Added a slider to the options widget to configure the auto forward time
- Added option to the asset creation browser for ingame widgets and main menu widgets
  -This will only generate the layout for now. The animations and the blueprint graph are not generated yet. 
    -The blueprint graph can be duplicated from the widgets contained in the plugin.
- VNM Tab in Dialog Blueprint should (hopefully) be automatically visible now
- Added player input system
  -Added Dialog Input Node
    - Added dialog input system to VNMScript
- Added option to memory nodes to have pins for getting the character/scene id and memory id
- Refactored buttons and added menu text button and menu icon button
  - Added more customization options to buttons
    - Added system of selecting buttons
    - Added system for locking buttons
- Added Activatable Widgets. These widgets can be displayed using Widget Show/Hide nodes.
  - Also added support for that in the VNMScript
- Added character rename/interactive rename to VNMScript
- Cleaned up and refactored widget blueprints