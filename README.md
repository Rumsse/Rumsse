# Hi! I'm Maria Wieczorek
**Gameplay Programmer | Unity & Unreal Engine | Tech Art Enthusiast**

I specialize in crafting smooth gameplay mechanics, multiplayer systems, and editor tools that streamline team workflows. I am currently studying Game Development (3rd year) and simultaneously working on three game projects.

I have a strong cross-disciplinary mindset. With a solid foundation in Game Design and a working knowledge of 3D asset pipelines, I seamlessly collaborate with artists and designers to ensure technical blockers never slow down the team.

## 🛠 Tech Stack & Tools
*   **Engines & Frameworks:** Unity 6000+, Unreal Engine 5
*   **Languages:** C# (.NET, LINQ, Events/Delegates, Memory Management), C++, HLSL
*   **Architecture & Systems:** MVC/MVP UI Architecture, JSON Data Persistence, ScriptableObjects Data-Driven Design
*   **Audio & Input:** FMOD, Unity Audio Mixer, New Input System (Event-based input handling)
*   **Animation & UI:** UI Toolkit (Data Binding & Custom Controllers), Unity Animator (State Machines), UE5 MetaHuman Retargeting
*   **Networking & Libraries:** FishNet, PrimeTween (GC-free animations)
*   **Debugging & Profiling:** Unity Profiler, Visual Studio Debugger, Advanced Asset Management (Meta files/GUID recovery)
*   **Workflow & Management:** Git (GitHub/GitLab), Agile (Scrum/Kanban), Jira, ClickUp, Notion, Code Reviews
*   **Tech Art & Editor Tools:** UI Toolkit, Custom Inspectors, Shader Graph, VFX Graph, RenderGraph API, URP Pipeline Configuration

## 🧠 My Coding Standards
I care deeply about code quality, performance, and readability:
*   **Clean Architecture:** Heavy use of interfaces, SOLID principles, and other design patterns.
*   **Readability first:** I prefer inversion / early returns to avoid nesting. Single-line `if` statements are written without brackets, and short methods (like simple `Awake` calls) use expression-bodied members (`=>`). 
*   **No clutter:** I write self-documenting code with English debugs rather than leaving commented-out code or unnecessary comments. I keep enums close to the logic if they are script-specific and use `#region` to organize larger classes.
*   **Optimization:** Minimizing Draw Calls, using Object Pooling, and regular profiling.
*   **Zero-Allocation Mindset:** Replacing standard Coroutines with Unity 6 Awaitables, utilizing PrimeTween for GC-free animations, and strictly minimizing Update() calls to ensure stable frame rates and prevent memory spikes.
*   **UI Architecture:** Strict separation of logic and presentation using MVC/MVP patterns in UI Toolkit. I heavily utilize data binding (`dataSource`) and event delegates to keep the UI decoupled from core gameplay systems.
*   **Deep Engine Mastery:** Strong understanding of Unity's serialization and asset pipeline, including manual recovery of ScriptableObject GUIDs in meta files to prevent data loss during heavy structural refactoring.
*   **Data Management:** Designing robust JSON-based save systems and utilizing ScriptableObjects for flexible, data-driven game architecture.

---

## 🎮 Featured Projects

### 1. Cyberiada 2025/2026 - Rustcrave
**🏆 1st Place Winner of Cyberiada**
*A project initially developed by a 10-person team for the competition. It is a fully finished game, but our core team decided to continue its development for a commercial release. I acted as the Lead Programmer, managing a team of 3 developers (now it's only 2) using ClickUp and onboarded new member mid-development.*

[![Rustcrave Gameplay](https://img.youtube.com/vi/pmjQPBk7nEw/maxresdefault.jpg)](https://youtu.be/pmjQPBk7nEw)

*   **My Role:** Planning the core architecture, conducting code reviews, resolving bugs, and acting as the main point of contact for Game Designers and Artists.
*   **Technical Highlights:** 
    *   **Core Systems:** Developed the procedural tunnel generation (including resource spawning and camera logic), JSON-based Save System, and Asylum mechanics (crafting, swarm management, map path-selection).
    *   **UI Architecture:** Implemented a decoupled, MVC-style UI architecture using UI Toolkit. Utilized Data Binding (`dataSource`) and event delegates to keep the presentation layer strictly separated from gameplay logic.
    *   **Animation & Behavior:** Managed complex character behaviors and animation transitions using code-driven State Machines, integrating them with the Unity Animator.
    *   **Audio & Rendering:** Helped with integrating game audio using FMOD. Deeply configured URP Pipeline Assets (e.g., Global Volumes, render settings) to balance visual fidelity with performance.
* *(Status: Active Development)*
*   [💻 View Code Showcase]

### 2. Purrrifiers: Cleaning Chaos (Rubens Games)
*Commercial internship (Jul - Nov 2025) for a 4-player co-op multiplayer game published by FreeMind S.A. and PlayWay S.A.*

[![Purrrifiers Gameplay](https://img.youtube.com/vi/I9ndQAafPn0/maxresdefault.jpg)](https://www.youtube.com/watch?v=I9ndQAafPn0)

*   **My Role:** I was mainly responsible for creating the "Streamer's House" location and implementing all quests revolving around it. I gained hands-on experience in multiplayer development using **FishNet**.
*   **Technical Highlights:** Implemented animations, worked with the IK Rig system, handled text localization, and debugged/fixed issues in existing codebases.
*   [🎮 Steam Store Page](https://store.steampowered.com/app/2117430/?snr=1_5_9__205)

### 3. Lume Rush
*Space Survival Management Game.*

[![Lume Rush Gameplay](https://img.youtube.com/vi/TJ71BKYtNLw/maxresdefault.jpg)](https://youtu.be/TJ71BKYtNLw)

*   **The Hook:** Inspired by the resource gathering of *60 Seconds!* and ship management of *Fallout Shelter*, the player has a very short time to gather resources on nearby planets and repair a hyperdrive before a radioactive solar explosion destroys the system.
*   **Technical Highlights:** Handled the technical migration of the planet creator asset from Built-in to URP. Wrote a custom Scriptable Renderer Feature using the RenderGraph API to properly render complex ocean shaders in the new pipeline. Developed custom shaders and built custom editor tools/inspectors using UI Toolkit to streamline the team's workflow.
*   [💻 Source Code](https://github.com/Rumsse/lume-rush.git)

### 4. D.O.R.I.A.N.
*Action Platformer & My First Unreal Engine 5 Project.*

[![D.O.R.I.A.N. Gameplay](https://img.youtube.com/vi/g7OnpQLJHdQ/maxresdefault.jpg)](https://youtu.be/g7OnpQLJHdQ)

*   **The Hook:** Set in a monochromatic "digital purgatory" where sterile geometry is disrupted by an anomaly, forcing the player to navigate through corrupted, shifting cubes.
*   **Technical Highlights:** Developed as a university assignment. Handled Blueprint implementation for core mechanics and power-ups, animation retargeting onto a MetaHuman, and custom lighting setups.
*   [💻 Source Code on Gitlab](https://gitlab.com/Rumsse/unrealengineproject.git)

### 5. Eclipse Harmony
*2-Player Co-op Survival Game created during the 2nd semester of university.*

[![Eclipse Harmony Gameplay](https://img.youtube.com/vi/eCVVuBcuY0c/maxresdefault.jpg)](https://youtu.be/eCVVuBcuY0c)

*   **The Hook:** A *Vampire Survivors* inspired game where two players must constantly swap between human and spirit forms to protect each other and survive.
*   **Technical Highlights:** Built with a strict focus on clean architecture (SOLID principles, interfaces, inheritance) and performance optimization using Object Pooling for enemy and projectile spawning. Implemented an instrument upgrade system utilizing ScriptableObjects, and enhanced visuals via Shader Graph and custom post-processing/lighting.
*   [💻 Source Code](https://github.com/Rumsse/eclipse-harmony.git)

### 6. Beavers Game (work title) - Project I am currently working on.
*Mobile Multiplayer Game developed in Unreal Engine 5.*

*   **The Hook:** It's a game inspired by a combination of Bomberman/Bomb it and Agar.io, where 4 players play as beavers and try to eat as much wood as possible so they can eventually eat other players and win.
*   **Technical Highlights:** Architected and implemented the multiplayer system using a **Listen Server** model in Unreal Engine. Currently focusing on network replication, bandwidth optimization, and adapting controls and performance (UI, rendering) strictly for mobile platforms.
*   *(Status: Active Development)*

### 7. Fantasy Game (work title) - Project I am currently working on. 
*Multiplayer Fantasy RPG Game (Listen Server)*
*   **The Hook:** It's a game for 3 players, set in a Fantasy world, where as the King's guardians, players have to save him.
*   **Technical Highlights:** Implemented Visual Effects for the game. Currently focusing on Mage's Spells.
*   *(Status: Active Development)*

---

## 🥽 VR Games | Dance Mat Game | Game Jams

### QLaRat - Dance Mat (PogJam2026)
*A rhythm game created during a 40-hour game jam, designed specifically for a dance mat controller (with keyboard fallback).*
*   **Technical Highlights:** Developed the entire BPM synchronization system from scratch, alongside animations and VFX.
*   [▶️ Watch Gameplay](https://youtu.be/mKOJdjjvRRw) | [💻 Source Code on Gitlab](https://gitlab.com/Rumsse/grzmotobirds.git)
  
### VR - Devouring Sandworm
*A VR cooking game where you prepare meals for a worm in a post-apocalyptic wasteland.*
*   [▶️ Watch Gameplay](https://youtu.be/_vJdlf8kqKY) | [💻 Source Code](https://github.com/Rumsse/vr-cooking-game.git)

### VR - PO.ZIOMku (PogJam2025)
*My very first VR game, created during a 40-hour game jam. The player must maintain an optimal intoxication level while surviving hallucinations, a police drone, the White Lady, and their own homie.*
*   [▶️ Watch Gameplay](https://youtu.be/PFTHNRm1wHk) | [💻 Source Code](https://github.com/Rumsse/poziomku-vr-gamejam.git)

### No Shit (Cyberiada Gamejam 2026)
*A 24-hour game jam, on which worked 10 team members. The player has to constantly repair a bathroom that keeps breaking down while waiting for the plumber.
*   [🎮 Itch.io](https://3pieczarkis.itch.io/no-shit) | [💻 Source Code](https://gitlab.com/Rumsse/cyberiada-gamejam.git)

--- 

## 🎨 Tech Art & Visuals
*Enhancing the game's visual fidelity and ensuring rendering performance across multiple projects.*

*   **Shaders & Rendering Pipeline:** Successfully migrated legacy assets from the Built-in Render Pipeline to URP. Extended the rendering pipeline using modern RenderGraph API and Scriptable Renderer Features to fix and integrate custom effects (e.g., Ocean rendering). Developed optimized custom shaders using both HLSL and Shader Graph.
*   **Pipeline Optimization:** Deeply configured URP Pipeline Assets (e.g., adjusting rendering settings, shadow cascades, and global volumes) to achieve an optimal balance between visual fidelity and performance targets in projects like Rustcrave.
*   **VFX & Lighting Automation:** Designed dynamic particle systems and Visual Effect Graph setups across all my projects, including commercial implementation of some effects in *Purrrifiers: Cleaning Chaos*. Configured global illumination, lightbaking, and post-processing volumes to establish strong visual identities.

---

## 🛠 Unity Editor & Workflow Automation
*Developing custom editor extensions to accelerate team velocity, prevent human error, and empower Game Designers.*

*   **Dynamic UI Tooling:** Built a foolproof *Dynamic Event Inspector* using UI Toolkit. Implemented nested lists and conditional field rendering (showing/hiding fields based on checkbox states) to keep the designer's interface clean and intuitive.
*   **Pipeline Automations:** Scripted a *Bulk Renamer*, *Global Font Changer*, and a *Quick Scene Selection* window. These tools eliminated repetitive manual tasks and significantly sped up global project refactoring.
*   **Level Design Helpers:** Programmed a custom *Snap to Ground* utility equipped with physics raycasting, drastically reducing environment blockout and prop placement times for the level design team.

---

## 🌱 Currently Exploring & Learning
*I am always looking to expand my technical skill set. Right now, I am heavily focused on deepening my knowledge in:*

*   **Advanced Optimization:** Mastering deep profiling (CPU/GPU), strict memory management (zero-allocation patterns), and asset pipeline optimization to squeeze maximum performance and stable frame rates across different platforms.
*   **Tech Art & Rendering:** Expanding my knowledge in Unity's rendering pipelines (URP, RenderGraph API) and writing more complex custom shaders (Compute, HLSL) to push visual boundaries without breaking performance budgets.
*   **Unreal Engine 5 & C++:** Expanding my core engine expertise by learning UE5 and C++. Within this ecosystem, I am actively implementing multiplayer systems, diving deep into Network Replication, RPCs, and Listen Server architecture tailored for mobile devices.

---

## 📫 Let's Connect!
I'm always open to discussing clean code architecture, editor tools, or VR development.
*   **LinkedIn:** [Maria Wieczorek](https://www.linkedin.com/in/maria-wieczorek-9669b241b)
*   **GitLab:** [Rumsse](https://gitlab.com/Rumsse) *(My main platform I use for projects)*
*   **Email:** [wieczorekmaria.m@gmail.com](mailto:wieczorekmaria.m@gmail.com)
