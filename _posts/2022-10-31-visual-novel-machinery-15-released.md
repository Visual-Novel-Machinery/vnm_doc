---
layout: posts
title:  "Visual Novel Machinery 1.5 Released"
excerpt: Visual Novel Machinery 1.5 has been released
categories:
  - release
tags:
  - release
---

Hello everyone,

Today marks the release of Version 1.5, and with it the release of VNMScript. It's a scripting language made just for Visual Novel Machinery, which you can use to also write your texts in a text editor, instead of the node-based approach. Hope you enjoy it!

Changelog:

- Fixed issue in Choice Graph that led to choice graph not being constructed properly in UI
- Fixed crash on trying to save the game while no dialog is running in Visual Novel Machinery
- On loading a save, the characters will now no longer hide behind the scene background
- Added support for image choices
- Added support for 3D choices
- Added support for adding layers directly to a character on using the Character Show Node
- Experimental: Added support for VNMScript, a scripting language that allows you to write dialogs for Visual Novel Machinery in your favorite text editor and then import it to Unreal Engine.