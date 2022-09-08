---
layout: single
title: CG Definition
permalink: /docs/data-definitions/cg-definition
toc: true
sidebar:
  nav: "docs"
---



The class name for this definition is **DialogImageDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialog Image Id | FName | The internal ID identifying the CG |
| Dialog Image | UTexture2D* | The actual CG texture |
| Dialog Image Layers | TMap\<FName, FImageLayerDefinition\> | Array of Layer information for this specific CG |
