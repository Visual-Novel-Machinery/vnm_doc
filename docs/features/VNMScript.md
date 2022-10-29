---
layout: single
title: VNM Script
permalink: /docs/features/vnm-script
toc: true
sidebar:
  nav: "docs"
---

If the node-based approach is nothing for you, then you can also use the scripting language of Visual Novel Machinery, called VNM Script

## Basics

To use VNMScript you need to create a file called "\<name\>.vnm". It is vital that the file ends if ".vnm". If you don't do this then the Unreal Engine will fail to import the file.

In the file you can copy the snippet from below:
```
dialog.text "Hello World!"
dialog.end
```

This will generate the following node-based dialog in Unreal Engine:
![Hello World Example Node-Based]({{ site.baseurl }}/assets/images/VNMScript/HelloWorldExample.png)

To import the VNMScript file drag and drop it into your Content Browser. After importing, don't forget to add the new dialog to the Dialog Definitions Data Table, so that you can use it.

For reference how to use all features in VNMScript check their respective documentation page. They always contain the example as both a Blueprint Image and in form of VNMScript.

## Important Notes

If you are using Ids in your script, make sure you have added them to the respective data table before you import the file.

For example:
```
dialog.text -character=cube "Hello World as Cube!"
dialog.end
```

Make sure you have added a character with the id cube to the Character Definitions Data Table.