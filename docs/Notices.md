---
layout: default
nav_order: 10
title: Notice de Construction de la Voiture RC
has_children: true
---

# Notice de Construction de la Voiture RC

## 1. Préparation des Matériaux

### Matériaux nécessaires
Pour la réalisation de cette voiture RC, il vous faudra impérativement :

- Une imprimante 3D
- Des bobines de PLA et de TPU pour imprimer les pièces nécessaires
- Tournevis
- Fil de fer
- Rondelles
- Roulements
- Boulons
- Colle forte

![Image des matériaux nécessaires](path/to/image)

## 2. Conception et Prototypage

#### Impression du châssis
La première étape consiste à imprimer le châssis qui permettra de poser et fixer les différents éléments de la voiture.

![Image du châssis imprimé](path/to/image)

#### Impression de la crémaillère de direction
La deuxième étape consiste à imprimer les différents éléments de la crémaillère de direction.

- Une rampe crantée
- Un engrenage
- Deux coudes
- Deux axes de direction

Vous pouvez modifier les diamètres inttérieurs des des axes en fonction du diamètre exterieur de vos roulements.


![Image de la crémaillère de direction](path/to/image)

#### Impression des roues
Pour finir, vous pouvez imprimer les roues, composées de deux parties : la jante en PLA et le pneu en TPU.

- Deux jantes pour l'arrière (pour les axes des moteurs)
- Deux jantes pour l'avant (pour les roulements de la crémaillère)

![Image des roues](path/to/image)

## 3. Assemblage du Châssis et de la Crémaillère

### Assemblage de la crémaillère
1. Fixez les différents éléments de la crémaillère entre eux à l'aide de fil de fer.
2. Collez la rampe crantée au centre de la glissière (achetée ou imprimée).
3. Fixez la glissière sur le châssis à l'aide de boulons.
4. Fixez vos deux roulements sur les axes de la crémaillère.
5. Mettez les roues sur les roulements.

![Image de l'assemblage de la crémaillère](path/to/image)

## 3. Placement des composants sur le Châssis 

### Montage des motoréducteurs
1. Placez les moteurs DC dans les supports prévus à cet effet sur le châssis.
2. Fixez les moteurs solidement pour éviter qu'ils ne bougent pendant le fonctionnement.

### Installation du module ESP32
1. Montez le module ESP32 sur le châssis.

### Installation du module L298N
1. Montez le module L298N sur le châssis.

### Installation du servo-moteur
1. Placez le servo-moteur sur son support créé sur le châssis.
2. Fixez l'écrou sur le palonnier et installez l'écrou sur la denture de la crémaillère.

![Image de l'assemblage final](path/to/image)

## 5. Connectique entre les Composants

### Connexion du module L298N aux moteurs
Connectez les bornes de sortie du module L298N aux bornes des moteurs DC (OUT1 et OUT2 pour un moteur, OUT3 et OUT4 pour l'autre).

### Connexion du module ESP32 au module L298N
Connectez les pins IN1, IN2, IN3 et IN4 du module L298N aux GPIOs appropriés de l'ESP32.
Connectez les pins ENA et ENB du module L298N aux GPIOs de l'ESP32 pour contrôler la vitesse des moteurs.

### Connexion du servo-moteur
Connectez le servo-moteur à un autre GPIO de l'ESP32.
Connectez le fil de signal du servo au GPIO choisi, et les fils d'alimentation et de masse aux pins 3V3 et GND de l'ESP32.

### Alimentation
Connectez une source d'alimentation appropriée au module L298N pour alimenter les moteurs (Vs=7,5V).
Assurez-vous que l'ESP32 est alimenté correctement via le module L298N sur l'entrée (Vss=5V).

![Image du câblage des composants](path/to/image)

## 6. Programmation de l'ESP32 avec Dabble

### Programmation de l'ESP32
1. Téléchargez et installez l'IDE Arduino.
2. Installez les bibliothèques nécessaires pour l'ESP32 et Dabble.

### Téléversement du code
1. Connectez l'ESP32 à votre ordinateur via un câble USB.
2. Sélectionnez le bon port COM dans l'IDE Arduino et téléversez le code.

### Installation de Dabble
1. Téléchargez l'application Dabble sur votre smartphone depuis le Google Play Store ou l'App Store.
2. Suivez les instructions pour installer et configurer l'application.

### Test et calibration
1. Allumez la voiture RC et ouvrez l'application Dabble.
2. Testez les contrôles pour vous assurer que les moteurs et le servo fonctionnent correctement.
3. Ajustez le code si nécessaire pour améliorer la réactivité et la précision des contrôles.

![Image du test et calibration](path/to/image)
