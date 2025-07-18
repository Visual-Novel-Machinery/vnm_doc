---
layout: single
title: Global Memory Get
permalink: /docs/nodes-references/global-memory-get
toc: true
sidebar:
  nav: "docs"
---


![Global Memory Get Node Visual]({{ site.baseurl }}/assets/images/NodeReference/global-memory-get.png)

## Pins

### Input

| Name | Type | Description |
| --- | --- | --- |
| Global Memory Id | Name | The ID of the global memory variable to retrieve (only shown when "Use Pins For Ids" is enabled) |

### Output

| Name | Type | Description |
| --- | --- | --- |
| Value | Variable | The value of the global memory variable (type depends on the memory type) |

## On-Node Properties

| Name | Description |
| --- | --- |
| Memory | Name | The ID of the global memory variable to retrieve (only shown when "Use Pins For Ids" is disabled) |

## Additional Properties

| Name | Type | Description |
| --- | --- | --- |
| Use Pins For Ids | Boolean | If set to true, the Global Memory Id will be available as an input pin instead of a property |

## Script Reference
```
<variable name>=global.memory.get <global memory id>
```