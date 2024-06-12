---
layout: default
nav_order: 4
title: Études et choix techniques
---

# Études et choix techniques

## 1. Étude de différentes voitures RC

Nous avons étudié différents types de voitures RC DIY pour déterminer les caractéristiques souhaitées telles que la taille, le type (tout-terrain, course, drift, etc.), et la gamme de prix.

## 2. Conception et spécifications

La conception de la voiture RC est définie, incluant :

- **Châssis** : Forme, fonctionnalité, capacité a accueillir les differents composants.
- **Crémaillère** : Design, fonctionnalité.
- **Roue** : Fonctionnalité et capacité a se fixer sur les roulements et les axes des moteurs
- **Dimensions et échelle** : Nous avons choisi une longueur de 20 cm et une largeur de 10 cm en fonction de l'usage.
- **Matériaux** : Sélection des matériaux pour le châssis, batterie, moteur, driver, ESP32, servo-moteur, etc.

## 3. Système de propulsion

Le choix du système de propulsion comprend :

- **Moteurs électriques** : Plus courants, offrant différentes gammes de puissance et de performance.
- **Moteurs thermiques** : Pour les modèles plus spécialisés, offrant une expérience plus authentique mais requérant plus d'entretien.

Finalement, nous avons choisi deux motoréducteurs de 3V chacun avec une vitesse de rotation de 500 RPM, correspondant à notre couple et à une puissance suffisante pour atteindre 1,5 m/s.

## 4. Électronique et contrôle

L'électronique embarquée joue un rôle crucial dans la performance et les fonctionnalités de la voiture :

- **Récepteur et émetteur (carte ESP32)** : Pour la communication entre la voiture et la télécommande.
- **Servomoteurs** : Pour la direction de la voiture.
- **Driver L298n** : Pour faire la liasion entre l'ESP32 et les moteurs

## 5. Pneus et roues

Les pneus et les roues sont adaptés au type de surface (asphalte, terre, herbe), influençant fortement l'adhérence et la maniabilité. Nous avons choisi de concevoir nos propres roues 3D avec une adhérence conséquente pour une meilleure maniabilité.

## 6. Programmation

Le codage sur Arduino permet d'établir toutes les fonctions de paramétrage dans l'ESP32 et de contrôler notre voiture soit par WiFi, soit par Bluetooth, à partir de notre téléphone.

## 7. Prototypage et tests

La fabrication du prototype sera suivie de tests nécessaires pour valider la conception, la durabilité et les performances. Cela peut inclure des ajustements et des modifications durant le projet.
