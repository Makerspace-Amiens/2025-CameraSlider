---
layout: default
nav_order: 4
title: Études et choix techniques
---

# choix des composants 

**Un rail profilé de 1m20**
Nous avons choisi un rail profilé en aluminium de 1,20 mètre, car cette longueur correspond à celle d’un bureau standard. Cela permet d’installer facilement le rail sur une table dans le médiaLab de l'école, sans nécessiter d’installation fixe au sol. Ce format est à la fois pratique, stable et adapté à la majorité des plans de tournage en intérieur.

**3 roues V-Slot**
Les roues V-Slot ont été retenues car elles sont spécialement conçues pour s'adapter aux rainures en "V" des rails profilés en aluminium que nous utilisons.
Nous avons choisi d'en installer trois (et non quatre), pour plusieurs raisons :
    - Réduction des frottements : avec trois roues, le contact avec le rail est optimal et il y a moins de risques de désalignement ou de blocage.
    - Meilleure facilité de réglage : cela simplifie l'ajustement du plateau roulant, car trois points définissent toujours un plan stable (contrairement à quatre qui peuvent générer du jeu ou des tensions mécaniques).
    - Montage plus simple et fluide, particulièrement adapté à une structure légère comme celle que nous construisons.

**ESP-WROOM-32**
Nous avons opté pour le microcontrôleur ESP-WROOM-32 car il est disponible à l'école et dispose de fonctionnalités sans fil intégrées, notamment le Bluetooth.
Ce choix nous permet de contrôler le rail à distance via un smartphone, ce qui est idéal puisque de nos jours tout le monde a facilement accès à un téléphone.
Nous utilisons l’application RemoteXY, qui permet de créer une interface de contrôle personnalisée pour piloter le moteur à partir du téléphone, en tirant parti des capacités Bluetooth de l’ESP32.

**Moteur pas à pas 17HE15-1504S**
Nous avons choisi un moteur pas à pas NEMA 17 (modèle 17HE15-1504S) pour motoriser le déplacement du chariot sur le rail.
Ce moteur offre plusieurs avantages :
    - Précision de mouvement : il fonctionne par pas fixes, ce qui permet un contrôle très précis de la position et de la vitesse.
    - Couple suffisant : d'après nos calculs nous avons besoin d'un couple de 45 Ncm, celui du Nema 17 est de 42Ncm. Cependant pour l'utilisation que nous allons faire du moteur, celui-ci devrait être suffisant.
    - Compatibilité courante : le NEMA 17 est un format très répandu, ce qui facilite son intégration mécanique et électrique avec les pièces imprimées ou standards.
Grâce à ce moteur, le système peut effectuer des mouvements fluides, linéaires et répétables, ce qui est essentiel pour obtenir des plans de travelling professionnels.

**Un driver TMC2209**
Pour piloter le moteur pas à pas, nous utilisons un driver TMC2209, reconnu pour son silence de fonctionnement et sa haute précision.
Les avantages que nous avons retenus :
    - <u>Mode de pilotage silencieux :<u/> idéal pour un usage en environnement audiovisuel où le bruit est un problème.
    - <u>Prise en charge du microstepping :<u/> permet des mouvements ultra-fluides et précis, en subdivisant chaque pas moteur en micro-pas.
     - <u>Faible échauffement :<u/> gestion intelligente du courant, ce qui évite la surchauffe du moteur et du driver.
     - <u>Communication UART :<u/> possibilité de configurer dynamiquement certains paramètres depuis l'ESP32, pour plus de flexibilité dans le code.

Ce driver est donc parfaitement adapté pour notre usage, car il combine performance, fiabilité et silence, ce qui est indispensable pour un système de travelling utilisé en tournage.
