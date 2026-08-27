# 🤖 Autonomous Search & Rescue Rover

[![ROS 2](https://img.shields.io/badge/ROS_2-Humble-blue)](https://docs.ros.org/en/humble/)
[![Simulation](https://img.shields.io/badge/Simulation-Gazebo-orange)](http://gazebosim.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

**Projet de robotique autonome** - Système de rover autonome pour la recherche et le sauvetage en environnement complexe.

## 🎯 Objectifs
- ✅ Exploration et cartographie autonome (SLAM)
- ✅ Détection de victimes par vision par ordinateur (OpenCV)
- ✅ Navigation autonome avec évitement d'obstacles (Nav2)
- ✅ Architecture modulaire et extensible

## 🏗️ Architecture du Système

```mermaid
graph TD
    A[Gazebo Simulation] --> B[LiDAR & Camera]
    B --> C[SLAM Toolbox]
    B --> D[OpenCV Detection]
    C --> E[Carte 2D]
    D --> F[Position Victime]
    E --> G[Nav2 Stack]
    F --> G
    G --> H[Commandes Robot]
### Phase 2 - Cartographie SLAM (Complétée ✅)
![Carte SLAM complète](slam_map_complete.png)
*Carte 2D générée en temps réel par le SLAM Toolbox. Le robot a exploré toutes les pièces de la maison.*
