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




## 📦 Installation Rapide

```bash
docker start ros2_gazebo
docker exec -it ros2_gazebo bash
source /opt/ros/humble/setup.bash
export DISPLAY=host.docker.internal:0
export TURTLEBOT3_MODEL=waffle_pi
ros2 launch turtlebot3_gazebo turtlebot3_house.launch.py




### 📝 Ce que tu dois faire :
1. Copie le bloc gris ci-dessus.
2. Va dans ton fichier `README.md` sur GitHub, clique sur le crayon (✏️).
3. Clique avec ta souris **tout en bas** de ton texte actuel.
4. Colle le bloc.
5. Descends tout en bas de la page et clique sur le bouton vert **"Commit changes..."**.

Une fois que tu as cliqué sur le bouton vert, ton README sera **100% terminé et parfait**. Dis-moi "C'est fini" et on passe à la Phase 3 ! 💪
