---
layout: page
title: "Modular Inventory System Plugin for Unreal Engine"
description: "A modular and Blueprint-friendly inventory system plugin for UE5 with automatic saving and item templates."
image: /assets/images/projects/inventory/inventory.png
permalink: /projects/InventoryPluginUE5/
status: done
priority: 400
tags:
  - plugin
  - UE5
  - c++
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="Inventory System Screenshot" class="project-hero">

This project is a modular, extensible inventory system plugin for Unreal Engine 5. Designed to be lightweight yet powerful, it provides a flexible structure for item management, storage containers, and automatic state saving — all through customizable components and templates.

The system is fully integrated into UE5's Blueprint system, allowing users to create unique item behaviors and inventory types with minimal setup.

Key Components:
1. Item Template Base Class
    - Serves as the foundation for all inventory items.
    - Can be extended via Blueprints to create different item types with custom visuals, behavior, or metadata.
2. Inventory Component
    - A reusable component that handles all inventory logic: adding, removing, transferring, and stacking items.
    - Can be attached to characters, containers, or world objects.
3. UI Integration
    - Supports custom drag-and-drop functionality.
    - Inventory and storage grids are dynamically displayed and fully interactive.
4. Automatic Saving
    - All inventory contents are automatically saved and loaded, making it seamless to persist state between sessions or level transitions.
5. Modularity & Extensibility
    - Built with modularity in mind — systems can be extended in C++ or Blueprint.

This system is ideal for games that need flexible item storage, whether it’s for characters, shops, chests, crafting stations, or world pickups.

## Gallery

<div class="project-gallery">
  <img src="{{ '/assets/images/projects/inventory/inventory.png' | relative_url }}" alt="Scene 1">
</div>