---
layout: default
nav_order: 2
title: Cahier des charges 
---

# Cahier des charges 
**1- Contexte et définition du projet**

À UniLaSalle Amiens, et plus précisément dans le Makerspace, se trouve une salle dédiée à la production audiovisuelle : le MédiaLab. Cette salle dispose de caméras fixes permettant de réaliser des captations simples.
Afin d’offrir plus de flexibilité dans les mouvements de caméra, l'idée de concevoir un rail de travelling motorisé a été proposée.

C’est dans ce cadre que notre projet prend forme : concevoir un système de travelling motorisé, facile d’utilisation, et accessible à tous les utilisateurs du MédiaLab.

**2 - Objectif du projet**

L'objectif du projet est de rendre ce rail polyvalent et utilisable dans divers contextes.

- <u>Rail 1m20 :</u> Nous avons choisi une longueur de 1,20 mètre, car elle correspond à la taille d’un bureau standard. Cela permet une installation simple, sans encombrement, tout en étant suffisant pour effectuer des mouvements de caméra significatifs.
L’utilisateur pourra définir le parcours exact que suivra la caméra sur ce rail.

- <u>Compatibilité avec différents types de caméras :</u> Utilisable pour tout type de caméra disponible dans le médiaLab

- <u>Simplicité d'utilisation :</u> L’un des enjeux majeurs du projet est l’accessibilité.
Le rail doit pouvoir être utilisé sans formation technique préalable. L’interface de commande est intuitive, et le système ne nécessite aucune connaissance particulière en électronique ou en programmation.

- <u>Système de commande à distance :</u>  Le contrôle du rail se fait à distance via un smartphone, grâce à l’application RemoteXY.

    Il suffit de télécharger l’application (disponible sur Android et iOS).

    Une fois connectée au microcontrôleur via Bluetooth, l’interface présente des boutons directionnels (gauche/droite) ainsi qu’une barre de réglage de la vitesse du moteur.

    Cela permet un pilotage en temps réel, simple et efficace. 

**3 - Description fonctionnelle des besoins**

| **Fonction 1 :** |          Déplacer une caméra                            |
|------------------------------------|--------------------------------------|
| **Objectif**                      | Réaliser un rail de travelling qui peut se déplacer |
| **Description**                    | Le rail doit pouvoir se déplacer horizontalement |
| **Contraintes**                    | Avoir un déplacement fluide |
| **Niveau de priorité**             | Très haute priorité. |

| **Fonction 2 :** |          Support adaptatif                           |
|------------------------------------|--------------------------------------|
| **Objectif**                      | réaliser un support de caméra universel |
| **Description**                    |Le support doit être réaliser de sorte que n'importe quelle caméra du Médialab puisse s'installer sur le rail. Pouvoir visser la caméra afin d'assurer une stabilité. |
| **Contraintes**                    | Avoir un support assez robuste, résistant, simple et rapide d'utilisation |
| **Niveau de priorité**             | Haute priorité. |

| **Fonction 3 :** |          Programmation des déplacements          |
|------------------------------------|--------------------------------------|
| **Objectif**                      | Déplacement Bluetooth grâce au téléphone.   |
| **Description**                    | Application connectée par Bluetooth permerttant de gérer le déplacement de la caméra sur le rail. |
| **Contraintes**                    | Intégration du système Bluetooth relié au rail.  |
| **Niveau de priorité**             | Haute priorité. |

| **Fonction 4 :** |          Développement d'un plug in de commande système OBS           |
|------------------------------------|--------------------------------------|
| **Objectif**                      | Automatisation des déplacements du rail de traveling grâce à des raccourcis de scènes OBS (Depuis un stream Deck ?) |
| **Description**                    | Un plug in OBS permettant de géer un type de déplacement (en avant, en arrière, de X centimètre, à une vitesse Y) uniquement grâce à un raccourci déini en amont sur OBS. |
| **Contraintes**                    | Le temps de développement et les compétences actuelles pour développer cela. |
| **Niveau de priorité**             | Faible priorité. |

**4 - Enveloppe budgétaire**
- 250 euros de budget 
- Matériel fourni par le Makerspace

**5 - Délais de réalisation**
- 75h de projet jusqu'au mois de juin 