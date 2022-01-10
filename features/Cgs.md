---
layout: default
title: CGs
parent: Features
nav_order: 3
---

# CGs

In every Visual Novel, some moments can only be displayed with an image, as an image can say a thousand words. For this the plugin offers the system of CGs. In terms of layering, they are always in front of the scene background and characters. All other systems are displayed in front of it.

## Basics

Visual Novel Machinery contains two nodes for working with CGs. These are [CG Show Node]({{ site.baseurl }}{% link nodes-reference/cg-show.md %}) and [CG Hide Node]({{ site.baseurl }}{% link nodes-reference/cg-hide.md %}). As the names suggest, they are used for showing or hidding the CG. The CGs available are defined in the CG Definitions Data Table, and can be selected in the [CG Show Node]({{ site.baseurl }}{% link nodes-reference/cg-show.md %}).

![CG nodes in action]({{ site.baseurl }}/assets/images/CG/CGNodes.png)

There are also nodes for using image layering, but more about in the [CG image layering feature documentation]({{ site.baseurl }}{% link features/layering-system/layering-cgs.md %}).