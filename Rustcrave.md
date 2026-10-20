[⬅️ Back to Main Portfolio](README.md)

# 🏆 Rustcrave - Development Overview

**1st Place Winner of Cyberiada 2025/2026**

**Role:** Lead Programmer & Tech Art | **Team Size:** 10 | **Status:** Active Development (Commercial Release)

[![Rustcrave Gameplay](https://img.youtube.com/vi/pmjQPBk7nEw/maxresdefault.jpg)](https://youtu.be/pmjQPBk7nEw)

## Project Overview
A project initially developed by a 10-person team for Cyberiada (National Computer Game Development Championships), where it secured 1st place. Due to its immense potential, the core team decided to continue development toward a commercial release. The project is a roguelite game with RTS elements, focusing on time pressure, swarm management, and procedural exploration.

## Leadership & Project Management
As the **Lead Programmer**, I was responsible for the overall technical architecture and managing the programming team, emphasizing code quality, readability, and optimization.
- **Team Management:** Coordinated the development cycle using ClickUp: managing task creation, sprint planning, priority tagging, time estimation, and team assignments.
- **Code Quality:** Conducted rigorous Code Reviews, ensuring adherence to SOLID principles and performance standards.
- **Onboarding:** Authored technical documentation and successfully onboarded new programmers mid-development, ensuring a seamless transition into the team's workflow and core systems.
- **Cross-Discipline Bridge:** Collaborated closely with Game Designers and Artists to define tasks, project scope, establish development priorities, and seamlessly integrate mechanics and visual assets.


---

## Core Architecture & Deep Dive

### 1. Decoupled UI Architecture (MVC & UI Toolkit)
Engineered a fully event-driven UI utilizing the **MVC (Model-View-Controller)** pattern, ensuring complete separation between business logic and presentation.
- Integrated **UI Toolkit** with Data Binding (`dataSource`), drastically reducing the need for manual view updates.
- Built an Event Delegate system, guaranteeing high scalability and ease of adding new UI panels.
<p align="center">
  <img src="https://github.com/user-attachments/assets/851a6cde-3d34-40a6-b975-2a0ed02ceb40" width="47.72%" />
  <img src="https://github.com/user-attachments/assets/dd9279e6-04ab-4b7a-afd2-5833701cb599" width="50%" />
</p>

### 2. Core Gameplay Systems & Generation Mechanics
Implemented the primary systems driving the gameplay loop:
- **Procedural Tunnel Generation:** Engineered a robust procedural generation system using predefined prefabs. Developed complex logic to seamlessly connect chunks (including two-way tunnels), randomized resource and enemy spawn points, and dynamic camera zooms. Integrated a modifier system to inject controlled randomness and alter tunnel parameters.
<p align="center">
  <img src="https://github.com/user-attachments/assets/0edb5307-f7bc-4dae-a40b-cdf992fd8fdd" width="40%" />
  <img src="https://github.com/user-attachments/assets/a357f8d2-4f8d-4be5-935d-0dd227e3a312" width="53.6%" />
</p>

- **Roguelite Map & Progression:** Architected a procedural map system that generates interconnected nodes across dynamic columns and rows, culminating in a boss node. Programmed node-specific modifiers that directly influence gameplay within the corresponding tunnels (e.g., increased resource yields, altered enemy spawn rates, or unstable camera effects).
<p align="center">
  <img src="https://github.com/user-attachments/assets/39a0e98b-4781-4f7b-90ff-e23163e9e091" width="48%" />
  <img src="https://github.com/user-attachments/assets/68451e7a-8118-4f06-8fba-c9a9f0f5ec4f" width="48%" />
</p>

- **Swarm Management & Asylum Mechanics:** Built a comprehensive management interface allowing players to craft units and stat-boosting gadgets. Programmed detailed unit overviews displaying stats, names, and abilities, complete with dynamic camera framing focusing directly on the selected unit. Implemented quick-action buttons for restoring health/energy and smooth contextual animations for UI panels and crafting actions.
<video src="https://github.com/user-attachments/assets/cdae5f1a-b48b-44ef-81ed-e791a6e7c478" autoplay loop muted playsinline width="100%"></video>

- **Data-Driven Random Events:** Developed and heavily refactored a scalable Random Events system, optimized for designer readability. The system handles complex text and gameplay effects based on player choices and the specific units assigned to tasks (incorporating unique success rate percentages). Outcomes range from standard resource collecting or energy/health modifications to altering unit stats, granting overpowered units, or triggering easter eggs.
<video src="https://github.com/user-attachments/assets/27c22622-c591-43b5-ab6a-b4514150f507" autoplay loop muted playsinline width="100%"></video>

- **Fool-Proof Interactive Tutorial:** Created a context-aware, step-by-step tutorial system that introduces movement, hazards, and Asylum mechanics without breaking immersion. Engineered strict progression locks to prevent players from skipping steps, guaranteeing a soft-lock-free experience.




### 3. Modular Save System (JSON)
- Developed a lightweight and flexible save system based on **JSON**, allowing for easy serialization of complex gameplay data (swarm state, map progression, resources, and random event states).

---

## Performance & Data-Driven Optimization
Eliminating stuttering and ensuring smooth gameplay is a priority in games. I conducted strict A/B testing using the Unity Profiler to eliminate major bottlenecks:

- **UI Memory Allocations (-98.3%):** Reduced UI allocations from 39.36 kB/s to just **0.656 kB/s** by implementing a custom caching system.
- **Zero-Allocation Object Pooling:** Extended the Object Pooling system to command indicators. This completely eliminated runtime GC allocations and reduced initialization costs by **76.6%**.
- **VFX & Rendering Optimization (-59.6% GPU Time):** Optimized dust VFX rendering. Replacing expensive Mesh particles with oriented Billboards reduced the triangle count by **99.35%**, cutting GPU render time by **59.6%**.


---

## Links
- [💻 View Full Source Code](https://github.com/Rumsse/rustcrave.git)
