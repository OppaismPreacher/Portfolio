---
layout: page
title: "UE5 Modular Weapon Modding Plugin"
description: "A modular UE5 plugin for real-time weapon customization using stackable behavior mods."
image: /assets/images/projects/WeaponModding/CardHand.png
permalink: /projects/WeaponModding/
status: in-progress
priority: 400
tags:
  - plugin
  - UE5
  - c++
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="Inventory System Screenshot" class="project-hero">

This plugin is a flexible weapon modification system built for Unreal Engine 5, designed to allow real-time, in-game customization of weapons using stackable "mod cards". These mods are gameplay components that players can attach to their base weapon to dynamically alter its behavior.

Examples of mods include:

+1 Projectile

Bouncy Projectiles

Change Firing Pattern to Shotgun

Exploding Bullets

Charge-based Firing

The system is fully Blueprint-driven, allowing designers to create and test new mods quickly without writing C++ code. It was architected using Actor Components to ensure modularity and reusability, with a clean separation between weapon logic and mod behavior.

This project taught me a lot about data-driven design, component-based architecture, and building tools that are intuitive for other developers or designers to use. It’s ideal for games with roguelike, arena shooter, or sandbox elements where players can experiment with builds and combinations.

## Gallery

<div class="project-gallery">
  <img src="{{ '/assets/images/projects/WeaponModding/CardHand.png' | relative_url }}" alt="Scene 1">
</div>