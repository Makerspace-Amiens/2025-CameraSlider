---
layout: default
title: Préparation des Matériaux
parent: Etapes de fabrication
nav_order: 1
---

# Préparation des Matériaux

Dans cette partie vous pouvez trouver la liste des matériaux utilisés pour la construction de notre rail, ainsi que les pièces que nous avons modélisés sur le logiciel **Onshape**. 

## Liste des Matériaux

Voici la liste complète des composants nécessaires pour construire le rail de travelling motorisé :

- Une carte **ESP-WROOM-32** (microcontrôleur avec Bluetooth intégré)
- Un **rail profilé** en aluminium de 1m20
- Une courroie de 4 mètres (transmission du mouvement)
- 3 roues **V-Slot**, adaptées aux rainures du rail
- Un moteur pas à pas **17HE15-1504S**
- Un **driver TMC2209** pour piloter le moteur en silence et précision
- Une alimentation secteur 

En complément des composants principaux, il est indispensable de prévoir :

- Des vis, boulons et écrous variés pour l’assemblage de l’ensemble
- Des écrous freinés pour éviter le desserrage progressif 
- Des entretoises excentrique si nécessaire, cela sera principalement utilisé avec les roues et le plateau. En effet, comme les entretoises sont légèrement excentriques, nous allons pouvoir régler la distance entre les roues et le rail. Les entretoises seront au niveau du plateau, dans les différents troues de celui-ci. 

## Modélisation 3D
Les pièces suivantes ont été modélisées sur Onshape pour répondre aux besoins spécifiques du projet :

- Les pieds : permettent de surélever légèrement le rail et d’assurer sa stabilité sur n’importe quelle surface.
- Un carter de fin de rail : conçu pour protéger le mécanisme et empêcher un éventuel déraillement de la caméra en fin de course.
- Une boîte de rangement : cette boîte accueille l’ensemble des composants électroniques :
    - le moteur pas à pas
    - le driver
    - la carte ESP32
    - les câbles de connexion
Elle permet de centraliser l’électronique et d'assurer une protection mécanique.
- Un plateau universel : permet de fixer différents types de caméras ou de supports selon les besoins des utilisateurs.
Les pieds, le carther ainsi que la boite de rangement ont été imprimé à l'imprimante 3D. Quant au plateau universel, il a été imprimé grâce à une imprimante laser. Il est en acrylique 5mm.   


---

Une fois cette étape terminée, passez à l'[Assemblage](/assemblage).
