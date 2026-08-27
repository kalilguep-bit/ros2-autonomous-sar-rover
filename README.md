# 🤖 Autonomous Search & Rescue Rover

[![ROS 2](https://img.shields.io/badge/ROS_2-Humble-blue)](https://docs.ros.org/en/humble/)
[![Simulation](https://img.shields.io/badge/Simulation-Gazebo-orange)](http://gazebosim.org/)

**Projet de robotique autonome** - Système de rover autonome pour la recherche et le sauvetage.

## 🎯 Objectifs
- ✅ Exploration et cartographie autonome (SLAM)
- ✅ Détection de victimes par vision par ordinateur (OpenCV)
- ✅ Navigation autonome avec évitement d'obstacles (Nav2)

## 🏗️ Architecture
```mermaid
graph TD
    A[Gazebo] --> B[LiDAR & Camera]
    B --> C[SLAM Toolbox]
    B --> D[OpenCV]
    C --> E[Carte 2D]
    D --> F[Position Victime]
    E --> G[Nav2]
    F --> G
