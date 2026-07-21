---
layout: post
title: ECS-Based C++ Game Engine Framework
subtitle: Personal C++ Systems and Game Engine Project
categories:
  - game-xr
tags:
  - game-development
  - C++
  - ECS
  - SDL3
  - ImGui
  - Design Patterns
comments: false
published: true
---

Developed a modular game engine framework in C++ using an **Entity Component System**, or **ECS**, architecture. The project focuses on scalable engine design, reusable systems, and maintainable C++ code.

**My Role :** *Engine Developer*

**Tech Stack :** *C++, SFML, SDL3, ImGui, CMake*

**Platform :** *Cross-Platform Desktop*

<a href="https://github.com/ImtiazEvan720/iEngineV2"
   target="_blank"
   rel="noopener noreferrer"
   style="display:inline-block; padding:10px 18px; background:#24292f; color:#fff; text-decoration:none; border-radius:6px; font-weight:600;">
  View Project on GitHub
</a>

![ECS Engine Editor](/assets/img/ecs_game_engine_editor.webp)
The ECS architecture separates entities, data components, and systems, allowing features such as rendering, input, animation, collision, and UI to remain independent and composable.

The framework uses design patterns including **Factory** for object creation, **Observer** for event communication, **Command** for input and editor actions, and **Strategy** for interchangeable subsystem behavior.

External libraries are used mainly for platform abstraction and development tools, while the core engine architecture, resource management, and system interactions are implemented in modern C++ using RAII, smart pointers, and clear ownership boundaries.

The project also includes ImGui-based tools for inspecting entities, editing components, managing assets, and previewing animations.
