---
layout: default
nav_order: 10
title: Notice
has_children: true
---

# Notice de Construction de la Voiture RC

## 1. Préparation des Matériaux
### Matériaux nécessaires :
Pour la réalisation de cette voitute RC il va imperativement vous falloir une Imprimate 3D ansi que des bobines de PLA et de TPU pour pouvoir imprimer les pieces neccessare a la creation de celle-ci.
Pour la fixation de certaine pieces il va aussi falloir vous munir de tournevis, filde fer, rondelle,roulement boulon et de la colle forte.

## 2. Conception et Prototypage
### Téléchargement des fichiers :
Pour réaliser la voiture RC la premiere étape est d'imprimer les chassis qui permettra de poser, de fixer les differents éléments de la voiture.
Pour cela voici le fichier en stl, mais libre a vous de modifier celui ci a votre convenance pour de potentiel amélioration, et si l'envie vous prend de faire le chassis vous meme de A à Z voici aussi les fichier stl des composants pour pouvoir faire votre chassis aux dimension de ceux-xi:
fichiers stl

La seconde etape consiste a imprimer les differents éléments de la crémaillere de direction qui permettra d'orienter les roues avant en fonction de la direction voulu.
Pour cela il vous faudra imprimer uen fois la rampe cranté, une fois l'engrenage, deux coude et deux axe de direction, vous pouvez modifeir les diametre des axes en fonction du diametre interireur de vos roulements. La crémaillère se deplace grace a l'engrenage qui entraine la rampe cranté, mais celle glisse sur une glissière de la marque igus, vous pouvais donc acheter une glissière sur le site igus ou alors imprimer la votre grace au fichier stl fourni:
fichier stl

Pour finir vous pouvez imprimer les roues qui sont separer en deux partie, la gente qui est en TPU pour une tenue rigide et le pneu en TPU pour une meilleure aderence au sol, il ya a deux gente differente celle qui vont a l'arriere de la voiture sure les axes des moteurs et deux a l'avant qui permettent de se mettre sur les roulements de la cremaillere, vous pouvez d'ailleur adapter le dimatre du trou interieur de la roue en fonction de la taille de vos roulements.
ficher stl

## 3. Assemblage du Châssis et de la crémaillère
Une fois tous les elements imprimer et nettoyer nous allons pouvoir passer a l'assemblage de tout cela, nous allons tout d'abord commencer par fixer les differents elements de la cremaillere entre eux a l'aide de fil de fer que vous couperez et plierais au dimension voulue, il permettent une fixation solide et une bonne rotation des differents elements de la cremaillere. nous allons ensuite coller la rampe cranté au centre de la glissiere
(imprimer ou acheter sur le site igus) prealablement fixer sur le chassis a l'aide des deux tous prevue a cette effet a l'aide de boulon. Vous pouvez ensuite venir fixer vos deux roulement sur les axes de la cremaillere. Ensuite il ne reste plus qu'a mettre les roues sur les roulements.

## Étape 2 : Installation des Composants sur le Châssis

**Assemblage du châssis :**

Installez la crémaillère et assurez-vous qu'elle est bien en place et fonctionne correctement.
Fixer la crémaillère à l'aide de vises et d'écrous

**Montage des motoréducteurs :**

Placez les moteurs DC dans les supports prévus à cet effet sur le châssis.
Fixez les moteurs solidement pour éviter qu'ils ne bougent pendant le fonctionnement.

**Installation du module ESP32 :**

Montez le module ESP32 sur le châssis.
Placez l'ESP32 sur son support et fixez-le.

**Installation du module L298N :**

Prendre le module L298N sur le châssis.
Placez le module L298N sur son support et fixez-le.

**Installation du servo-moteur :**

Placer le servo-moteur sur son support créer sur le chassis.
Mettre l'écrou sur le palonier et placer installer l'écrou sur la denture de la crémaillère.

## Étape 3 : Connectique entre les Composants

**Connexion du module L298N aux moteurs :**

Connectez les bornes de sortie du module L298N aux bornes des moteurs DC (OUT1 et OUT2 pour un moteur, OUT3 et OUT4 pour l'autre).

**Connexion du module ESP32 au module L298N :**

Connectez les pins IN1, IN2, IN3, et IN4 du module L298N aux GPIOs appropriés de l'ESP32.
Connectez les pins ENA et ENB du module L298N aux GPIOs de l'ESP32 pour contrôler la vitesse des moteurs.

**Connexion du servo moteur :**

Connectez le servo moteur à un autre GPIO de l'ESP32.
Connectez le fil de signal du servo au GPIO choisi, et les fils d'alimentation et de masse aux pins 3V3 et GND de l'ESP32.

**Alimentation :**

Connectez une source d'alimentation appropriée au module L298N pour alimenter les moteurs (Vs=7,5V).
Assurez-vous que l'ESP32 est alimenté correctement via le module L298N sur l'entrée (Vss=5V).


## Étape 4 : Programmation de l'ESP32 avec Dabble

Programmation de l'ESP32 :

Téléchargez et installez l'IDE Arduino si ce n'est pas déjà fait.
Installez les bibliothèques nécessaires pour l'ESP32 et Dabble.
Allez dans la rubrique code pour accéder au programme Arduino.


Téléversement du code :

Connectez l'ESP32 à votre ordinateur via un câble USB.
Sélectionnez le bon port COM dans l'IDE Arduino et téléversez le code.

Installation de Dabble :

Téléchargez l'application Dabble sur votre smartphone depuis le Google Play Store ou l'App Store.
Suivez les instructions pour installer et configurer l'application.

Test et calibration :

Allumez la voiture RC et ouvrez l'application Dabble.
Testez les contrôles pour vous assurer que les moteurs et le servo fonctionnent correctement.
Ajustez le code si nécessaire pour améliorer la réactivité et la précision des contrôles.

