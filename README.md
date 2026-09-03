# UE5 Technical Art & UI Showcase 🎨🎮

> **Production Technical Art, VFX, Shading & UI Systems in Unreal Engine 5**  
> Technical breakdown of custom visual and gameplay feedback pipelines developed within a team environment using **Perforce (Helix Core)**.

[![Engine](https://img.shields.io/badge/Engine-Unreal%20Engine%205-0E1128?logo=unrealengine)](https://www.unrealengine.com/)
[![Tech Art](https://img.shields.io/badge/Focus-Tech%20Art%20%26%20UI-FF69B4)](#)
[![Version Control](https://img.shields.io/badge/VCS-Perforce%20%2F%20Helix%20Core-00A4EF)](#)

---

## 📽️ Visual Summary

![Project Showcase Reel](./media/tech-art-reel.gif)  
*HD Video Breakdown with Audio & UI Navigation available on [My Visual Portfolio](#).*

---

## 🛠️ Key Technical Systems & Art Pipeline

### 🎨 1. Post-Process Cel Shader & Material Pipeline
* **Custom Lighting & Edge Detection:** Engineered a post-process material using HLSL logic and Material Graphs to calculate scene depth gradients, world normals, and binary lighting thresholds.
* **Inverted Hull Outlines:** Set up dynamic mesh pass outlines to deliver crisp, styled art directions without post-process screen-edge distortion.
* **Dynamic Material Instances (DMI):** Exposed scalable parameters (outline weight, light threshold steps, color tinting) for real-time artist control and runtime feedback triggers.

### 💥 2. Niagara Visual Effects (VFX)
* **Modular Emitter Systems:** Designed dynamic Niagara particle systems for interactive environmental feedback, hit impacts, and hazard visual cues.
* **Runtime Parameter Driving:** Tied particle intensity, color shifts, and spawn rates directly to player proximity and gameplay state events using Blueprints.

### 💃 3. Animation Blueprints & State Machines
* **Anim State Machine Architecture:** Built modular Animation Blueprints handling locomotion blending, pose transitions, and montage overlays.
* **Anim Notifies & Sync:** Driven precise gameplay feedback loops by triggering Niagara VFX spawns and audio events directly through Animation Notifies.

### 🖥️ 4. UI Architecture & HUD Systems
* **Modular UMG Interfaces:** Designed decoupled UI widgets, HUD elements, and menu structures using Blueprints.
* **Dynamic Gameplay Binding:** Interfaced HUD updates (stamina, interaction prompts, environmental indicators) dynamically with underlying game state drivers.

---

## ⚙️ Source Control & Production Workflow

* **Version Control:** Managed across team streams via **Perforce (Helix Core)** with strict asset locking protocols (`.uasset`, `.umap`).
* **Performance Optimization:** Profiled material instruction counts, texture sample limits, and particle draw calls using Unreal's Shader Complexity.

*(Note: Full project repository is maintained on a private team Perforce server. Interactive node breakdowns and code logic are available upon request.)*
