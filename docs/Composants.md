---
layout: default
nav_order: 9
title: Les Composants
---

# Composants

## Module L298N
<div style="text-align: center;">
  <img src="https://github.com/Makerspace-Amiens/2024-RCMiniCar/assets/119036120/4caf6cfc-dca9-463f-9fda-d6230316d020" alt="Module L298N" style="max-width: 100%; height: auto;">
</div>
<div style="text-align: left;">
  Le module L298N est un pont en H double qui permet de contrôler deux moteurs à courant continu ou un moteur pas à pas.

  Les Caractéristiques Techniques du Module L298N sont: Au niveau de l'Alimentation, Nous avons une Tension d'alimentation (Vss) de 5V, une Tension d'alimentation du moteur (Vs) : 5V à 35V
  un Courant de sortie maximal par canal : 2A

  Pour le Contrôle des Moteurs, il y a deux canaux : 2 (peut contrôler 2 moteurs DC ou 1 moteur pas à pas)
  avec une Puissance de sortie totale : 25W

  Les Connexions et les Broches :
  Les Broches IN1, IN2, IN3, IN4 : Entrées de contrôle pour les deux moteurs
  Les Broches ENA, ENB : Broches d'activation pour les moteurs A et B (permettent le contrôle de la vitesse avec PWM)
  Les Broches OUT1, OUT2, OUT3, OUT4 : Sorties vers les moteurs
  Les Broches Vss et GND : Connexion à l'alimentation logique
  La Broche Vs : Connexion à l'alimentation des moteurs

  Les Fonctionnalités
  Il est capable de contrôler la direction et la vitesse de rotation des moteurs.
  Il permet d'utiliser des signaux PWM pour contrôler la vitesse des moteurs.
  Il peut être utilisé pour contrôler des moteurs à courant continu, des moteurs pas à pas bipolaires ou unipolaires.
</div>

## ESP32
<div style="text-align: center;">
  <img src="https://github.com/Makerspace-Amiens/2024-RCMiniCar/assets/119036120/ad03aea4-64e6-4665-afeb-1f5298d81053" alt="ESP32" style="max-width: 100%; height: auto;">
</div>
<div style="text-align: left;">
  L'ESP32 est une série de microcontrôleurs. Nous l'avons choisi en raison de ses caractéristiques avancées et de sa polyvalence.

  Les Caractéristiques Principales

  Une Connectivité Sans Fil :

  Avec le Wi-Fi, il permet la connexion à des réseaux sans fil pour la communication et l'échange de données.
  Avec le Bluetooth et BLE (Bluetooth Low Energy) qui supporte les communications Bluetooth classiques et basse consommation, permettant une large gamme d'applications sans fil.

  De Nombreuses Interfaces de Communication :

  -GPIO : Plusieurs broches d'entrée/sortie générales.
  -ADC (Convertisseur Analogique-Numérique) : Permet de lire des signaux analogiques.
  -DAC (Convertisseur Numérique-Analogique) : Génère des signaux analogiques.
  -PWM (Modulation de Largeur d'Impulsion) : Contrôle de la luminosité des LEDs, moteurs, etc.
  -I2C, SPI, UART : Protocoles de communication pour interfacer divers capteurs et périphériques.

  Prototypage Rapide :

  Nous l'avons utilisé pour programmer sur Arduino IDE pour ainsi piloter notre voiture RC.

  Les avantages de l'ESP32 sont:
  La polyvalence avec une large gamme de fonctionnalités et de périphériques intégrés.
  Une connectivité Wi-Fi et Bluetooth intégrés.
  Une performance avec Processeur puissant capable de gérer des tâches complexes.

  En résumé, l'ESP32 est un microcontrôleur très polyvalent et puissant, grâce à ses capacités de connectivité sans fil et ses fonctionnalités, il nous a permis de développer notre projet.
</div>

## Motoréducteurs
<div style="text-align: center;">
  <img src="https://github.com/Makerspace-Amiens/2024-RCMiniCar/assets/119036120/f5f1fc59-07f4-4a66-be3b-e9adf92d67cb" alt="Motoréducteurs" style="max-width: 100%; height: auto;">
</div>
<div style="text-align: left;">
  Un motoréducteur est un dispositif qui combine un moteur électrique avec un réducteur de vitesse. Ce composant est utilisé pour faire déplacer notre voiture RC.
  Le moteur fournit la puissance de rotation initiale.
  Ce sont des moteurs à courant continu (DC).
  Le réducteur de vitesse est constitué d'un ensemble d'engrenages qui réduisent la vitesse de rotation du moteur tout en augmentant le couple.
  Pour le Fonctionnement,
  Le moteur électrique génère une vitesse de rotation élevée mais avec un couple relativement faible. Le réducteur de vitesse, à travers son système d'engrenages, réduit cette vitesse de rotation tout en augmentant le couple. La sortie de cette combinaison est une vitesse de rotation plus basse mais avec un couple plus élevé.
</div>

## Servo moteur
<div style="text-align: center;">
  <img src="https://github.com/Makerspace-Amiens/2024-RCMiniCar/assets/119036120/433fb176-6166-40e2-983d-1432308893cb" alt="Servo moteur" style="max-width: 100%; height: auto;">
</div>
<div style="text-align: left;">
  Un servo moteur est un type de moteur électrique qui est spécialement conçu pour permettre un contrôle précis de la position angulaire, de la vitesse et du couple. Notre servo moteur, nous sert pour la direction de notre voiture.
  Il est doté d'un moteur à courant continu (DC), d'un ensemble d'engrenages  permettant un contrôle plus précis des mouvements.
  Un circuit électronique intégré qui reçoit les signaux de commande de l'ESP32 et ajuste la position.

  Un potentiomètre mesure la position actuelle de l'axe du moteur.Le retour de ce capteur est utilisé pour ajuster la position en fonction de l'utilisation. Pour nous 45° pour tourner à droite et -45° pour tourner à gauche.

  Un signal de commande (généralement un signal PWM - Pulse Width Modulation) est envoyé au servo moteur.
  Ce signal détermine la position cible de l'axe du moteur.
  Le capteur de position mesure la position actuelle de l'axe et envoie cette information au circuit de contrôle.

  Le servo peut tourner sur un angle limité généralement 180 degrés ou moins.

  En résumé, un servo moteur est un dispositif essentiel pour un contrôle précis de la direction de notre voiture.
</div>
