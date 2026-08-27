# 🤖 Autonomous Search & Rescue Rover

[![ROS 2](https://img.shields.io/badge/ROS_2-Humble-blue)](https://docs.ros.org/en/humble/)
[![Simulation](https://img.shields.io/badge/Simulation-Gazebo-orange)](http://gazebosim.org/)
[![Python](https://img.shields.io/badge/Code-Python-green)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

> **Contexte du projet** : Développement d'un système robotique autonome capable d'évoluer dans un environnement inconnu et complexe pour la recherche et le sauvetage (SAR). Ce projet démontre la maîtrise de la stack complète ROS 2 : de la simulation à la navigation autonome en passant par la vision par ordinateur.

## 🎯 Fonctionnalités Clés

- 🗺️ **Cartographie Temps Réel (SLAM)** : Génération de cartes 2D précises via l'algorithme *Cartographer*.
- 👁️ **Vision par Ordinateur** : Détection de cibles (victimes) par analyse de couleur avec *OpenCV*.
- 🧠 **Navigation Autonome** : Planification de trajectoire et évitement d'obstacles dynamiques via *Nav2*.
- 🐍 **Développement Sur Mesure** : Création de nœuds Python personnalisés pour l'orchestration des missions.
- 🐳 **Environnement Containerisé** : Déploiement reproductible sous Docker (Ubuntu 22.04 / ROS 2 Humble).

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
