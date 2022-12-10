---
layout: single
title: CGs
permalink: /docs/features/cgs
toc: true
sidebar:
  nav: "docs"
---



In every Visual Novel, some moments can only be displayed with an image, as an image can say a thousand words. For this the plugin offers the system of CGs. In terms of layering, they are always in front of the scene background and characters. All other systems are displayed in front of it.

## Basics

Visual Novel Machinery contains two nodes for working with CGs. These are [CG Show Node]({{ site.baseurl }}{% link docs/nodes-reference/cg-show.md %}) and [CG Hide Node]({{ site.baseurl }}{% link docs/nodes-reference/cg-hide.md %}). As the names suggest, they are used for showing or hiding the CG. The CGs available are defined in the CG Definitions Data Table, and can be selected in the [CG Show Node]({{ site.baseurl }}{% link docs/nodes-reference/cg-show.md %}).

![CG nodes in action]({{ site.baseurl }}/assets/images/CG/CGNodes.png)
```
cg.show -id=cg1
dialog.text -character=cube "Look! It is CG1"
cg.hide
dialog.text -character=cube "Where did it go?"
dialog.end -nextdialog=start
```

There are also nodes for using image layering, but more about in the [CG image layering feature documentation]({{ site.baseurl }}{% link docs/features/layering-system.md %}).
