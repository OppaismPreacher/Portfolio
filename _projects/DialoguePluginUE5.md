---
layout: page
title: "Custom Dialogue System for Unreal Engine 5"
description: "A custom UE5 node-based dialogue system with support for options, search inputs, branching, and runtime actions."
image: /assets/images/projects/Dialogue/Dialogue.png
permalink: /projects/DialoguePluginUE5/
status: done
priority: 400
tags:
  - plugin
  - UE5
  - c++
  - solo project
---

This project is a fully custom node-based dialogue system for Unreal Engine 5, built from the ground up to support complex branching conversations, player input, and in-game consequences. The system is designed as a reusable custom asset type with a dedicated graph editor UI, allowing writers and designers to visually script dialogue logic without touching code.

Dialogue graphs are assigned via a modular DialogueComponent, which can be attached to any character or object capable of interacting with the player.

Node Types and Behavior:
1. Basic Node
    - Contains an array of text lines.
    - The dialogue system automatically steps through them sequentially.
2. Options Node
    - Functions like a Basic Node, but ends with a set of multiple choice options.
    - Options are defined via a map and presented as interactive buttons for the player to select.
3. Search Node
    - A free-text input version of the Options Node.
    - Ends with a search bar where the player types a response.
    - The system compares input against a set of keywords and routes to the appropriate branch based on matches.
4. Action Node
    - Executes gameplay logic at runtime.
    - Can grant items, trigger events, or unlock/lock dialogue branches in other conversations.
    - Enables dynamic state changes and player influence.

System Highlights:
- Fully custom node graph asset with custom editor UI
- Supports branching paths, player decisions, free input, and game-driven events
- Graphs are modular and can be reused or assigned to multiple actors
- Clean separation between dialogue content and game logic
- Easily extensible for future node types or localization

This system enables the creation of nonlinear conversations, reactive narratives, and player-driven outcomes — making it ideal for RPGs, immersive sims, or story-rich adventure games.