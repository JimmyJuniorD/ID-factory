# vr_physicSim_ID-factory
![Unreal Engine](https://img.shields.io/badge/Unreal_Engine-5.7-blue?logo=unrealengine)
![Language](https://img.shields.io/badge/Language-Blueprints%20%2F%20C%2B%2B-orange)
![Platform](https://img.shields.io/badge/Platform-Meta_Quest_2-green)

## 📖 Introduction

This project is an interactive VR simulation system developed using **Unreal Engine 5**. Unlike traditional industrial simulations, it constructs an automated flexible production line composed of “non-standard components” (such as household goods).

Main purpose are：
1.Stability and Optimization of Complex Rigid Body Dynamics in VR Environments.
2. **Modularity** of reusable interactive components.
3. **Industrial Data Visualization** in Immersive Environments.

## 🎮 Demo

![项目演示动图](https://你的GIF链接.gif)

> *上图展示了原料称重与自动熔炼的物理交互过程。*

## 🛠️ Tech Stack

- **Engine Core:** Unreal Engine 5.7 (Chaos Physics System)
- **Scripting:** Blueprints & C++
- **Optimization:** LOD Automation, Texture Atlassing, Draw Call Batching
- **Tools:** Git, RenderDoc , Blender 

## 🚀 Key Features

###1. Physics-Driven Weighing System
- Emulates authentic scale logic using physics constraints.
- Triggers “valve open” events in real time by detecting rigid-body mass, rather than through simple animation playback.

### 2. Flexible Pipeline Logic
- **Modular Design:** All transport units (e.g., conveyor belts, chutes) inherit from `BP_Transport_Base`, enabling logical reuse.
- **Automatic Error Correction:** Implements Trigger Box-based anomaly detection, automatically resetting positions when objects become stuck.
  
### 3. Performance Optimization
- Deeply optimized for Oculus Quest 2:
    - Renders large quantities of repetitive debris using **Instanced Static Meshes (ISM)**.
    - Reduced Draw Calls from over 2000 to approximately **150**, achieving stable **72 FPS** performance.

## 📦 Installation

1. clone this repo：
   ```bash
   git clone [https://github.com/你的用户名/vr-smart-factory.git](https://github.com/你的用户名/vr-smart-factory.git)
