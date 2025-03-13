# 🐝 Path Finding

Une simulation 2D utilisant SFML pour animer des abeilles qui doivent butiner des fleurs et les rapporter à leur ruche.

## 📌 Pour commencer

Ce projet a pour objectif de simuler un environnement dans lequel une abeille contrôlée par l'utilisateur et une abeille IA interagissent pour collecter et livrer des fleurs dans une prairie.

### 🔧 Pré-requis

Avant de commencer, assure-toi d'avoir SFML installé sur ton système !

### 💻 Installation

🔹 **Fedora**

Installe SFML avec la commande suivante :

```
sudo dnf -y install SFML
sudo dnf install SFML SFML-devel
```

🔹 **Autres systèmes d'exploitation**

- **Visual Studio (Windows) :** [Installation SFML sur Visual Studio](https://www.sfml-dev.org/tutorials/3.0/getting-started/visual-studio/)
- **Linux :** [Installation SFML sur Linux](https://www.sfml-dev.org/tutorials/3.0/getting-started/linux/)
- **macOS :** [Installation SFML sur macOS](https://www.sfml-dev.org/tutorials/3.0/getting-started/macos/)

## 🚀 Démarrage

Pour compiler et exécuter la simulation, exécute la commande suivante dans un terminal :

```
g++ planning_path_finding.cpp -o planning_path_finding -lsfml-graphics -lsfml-window -lsfml-system && ./planning_path_finding
```

## 🌻 Contexte du projet

Le projet se déroule dans un environnement 2D simulant une prairie parsemée de chemins. Voici les principaux éléments de la simulation :

- **Fleurs :** Placées aléatoirement sur la carte au démarrage, elles peuvent être ramassées par les abeilles.
- **Ruche :** La base où les abeilles doivent livrer les fleurs collectées. Elle est également placées aléatoirement sur la carte au démarrage.
- **Abeille (IA) :** Se déplace de manière autonome en planifiant son chemin pour récupérer une fleur et la rapporter à la ruche.
- **Abeille (joueur) :** Contrôlée par l'utilisateur, elle peut également ramasser des fleurs et interagir avec l'IA (ex : perturber ses déplacements ou sa collecte).

 ## 🔍 Fonctionnalités du projet

 ### 🤖 Abeille IA
 
- **Planification :** L’abeille IA sélectionne la fleur la plus proche à butiner.
- **Path Finding :** Un algorithme de recherche (BFS) calcule le chemin optimal jusqu’à la fleur choisie, puis jusqu’à la ruche.
- **Steering Behaviors :** Des comportements d’orientation (seek, arrival) permettent une animation des déplacements.

### 👾 Abeille joueur et IA

- **Interactions Environnementales :** Les abeilles doivent rester sur les chemins définis et interagir avec les éléments du décor (fleurs et ruche).

## 📷 Aperçu

![Capture d’écran du 2025-03-13 16-27-39](https://github.com/user-attachments/assets/0c2e6e11-5dd0-45ff-b33f-6524b7fdbc0b)
