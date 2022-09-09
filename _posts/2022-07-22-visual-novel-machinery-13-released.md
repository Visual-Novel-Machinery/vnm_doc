---
layout: posts
title:  "Visual Novel Machinery 1.3 Released"
excerpt: Visual Novel Machinery 1.3 has been released
categories:
  - release
tags:
  - release
---

Changelog:

- Added support for using voice overs, background music, and sound effects during dialogs
- Character now move properly when moving to a new location
- Added events for when Typewriting starts and Ends to BaseDialogBoxWidget
- Added setting to transitionable nodes that allows them to specify the playback rate of animations
- Added flag to Dialog Scene Switch Camera Node which makes it possible to not wait on the camera transition to finish before the next node starts
- Filter out Dialogs in the Scene Graph that are not referenced by any other dialog in their Dialog End Nodes
- Added setting to project settings to allow disabling auto start of dialogs on switching into a level that has the Dialog Controller Component attached to the HUD
- Added support for starting a dialog with the dialog object class and exposed that to the blueprint
- The color and opacity setting for dialog images is now actually used by BaseCharacterDisplayWidget/BaseCgDisplayWidget/BaseSceneBackgroundDisplayWidget
- Added flags to Dialog Text Node to typewrite faster or not typewrite at all for this node
- Shortened the names in the Visual Novel Machinery Tab to not occupy so much space