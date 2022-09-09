---
layout: posts
title:  "Visual Novel Machinery 1.4 Released"
excerpt: Visual Novel Machinery 1.4 has been released
categories:
  - release
tags:
  - release
---

Changelog:

- Documentation link found in the plugins tab of Unreal Engine now points to the correct documentation url again
- Support link found in the plugins tab of Unreal engine now points to the discord
- Confirmed plugin works on Android
- fixed a bug that if you pressed too quickly while typewriting with tags, it always showed an endtag
- Improved dialog text node so that you can now specify the localization settings directly on the node
- Dialog Start Nodes can no longer be duplicated
- The Diffing Tool in the Unreal Engine now supports Dialog Blueprints
- Added more safety checks to ensure that nothing bad happens
- Registered changes to all nodes in Visual Novel Machinery with the Unreal Engine Transaction system, so you can also undo/redo changes to character ids/text/... on nodes
- Dialog Scenes Data for the Dialog Scenes Graph is now no longer saved to the DefaultGame.ini but into its own DataAsset. The Dialog Scenes Graph Widget will new require you to set the data asset containing the data
- Spine 2D support (plugin for it can be found here)