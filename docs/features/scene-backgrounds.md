---
layout: single
title: Scene Backgrounds
permalink: /docs/features/scene-backgrounds
toc: true
sidebar:
  nav: "docs"
---



In every Visual Novel, it is important to set the scene, to know where the characters currently are. For this the plugin offers the system of scene backgrounds. In terms of layering, they are always in the complete background. All other systems are displayed in front of it.

## Basics

Visual Novel Machinery contains two nodes for working with scene backgrounds. These are [Scene Background Show Node]({{ site.baseurl }}{% link docs/nodes-reference/scene-background-show.md %}) and [Scene Background Hide Node]({{ site.baseurl }}{% link docs/nodes-reference/scene-background-hide.md %}). As the names suggest, they are used for showing or hidding the scene background images. The scene backgrounds available are defined in the Scene Background Definitions Data Table, and can be selected in the [Scene Background Show Node]({{ site.baseurl }}{% link docs/nodes-reference/scene-background-show.md %}).

![Scene background nodes in action]({{ site.baseurl }}/assets/images/SceneBackgrounds/SceneBackgroundNodes.png)

There are also nodes for using image layering, but more about in the [scene background image layering feature documentation]({{ site.baseurl }}{% link docs/features/layering-system.md %}).