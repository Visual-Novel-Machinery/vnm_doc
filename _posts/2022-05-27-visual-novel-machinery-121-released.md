---
layout: posts
title:  "Visual Novel Machinery 1.2.1 Released"
excerpt: Visual Novel Machinery 1.2.1 has been released
categories:
  - release
tags:
  - release
---

Changelog:

- Fixed bug with camera setting only being shown on Dialog Scene Show node if a Dialog Scene Switch Camera Node has been changed
- Refactored system for getting in level actors for cameras and spawn locations to factor in the new system from UE5, where Actor Instances don't get renamed anymore on a low level, but only a Actor Label is modified