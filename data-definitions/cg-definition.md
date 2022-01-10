---
layout: default
title: CG Definition
parent: Data Definitions
nav_order: 3
---

# CG Definition

The class name for this definition is **DialogImageDefinition**. It is used with a Data Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| Dialog Image Id | FName | The internal ID identifying the CG |
| Dialog Image | UTexture2D* | The actual CG texture |
| Dialog Image Layers | TMap\<FName, FImageLayerDefinition\> | Array of Layer information for this specific CG |
