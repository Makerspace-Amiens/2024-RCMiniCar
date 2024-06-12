

# Notice de Création d'une Voiture RC

## Étape 1 : Téléchargement des Pièces 3D
Téléchargement des fichiers STL :

téléchargez les fichiers STL pour les composants suivants :

-Châssis
-Crémaillère

Préparation des fichiers pour l'impression :

Importez les fichiers STL dans un logiciel de découpe comme Cura.
Configurez les paramètres d'impression en fonction de votre imprimante 3D (matériau, résolution, etc.).

Impression des pièces :

Lancez l'impression des pièces une par une.
Vérifiez chaque pièce après impression pour s'assurer qu'elle est correctement imprimée et sans défauts.

## Étape 2 : Installation des Composants sur le Châssis

Assemblage du châssis :

Installez la crémaillère et assurez-vous qu'elle est bien en place et fonctionne correctement.
Fixer la crémaillère à l'aide de vises et d'écrous

Montage des motoréducteurs :

Placez les moteurs DC dans les supports prévus à cet effet sur le châssis.
Fixez les moteurs solidement pour éviter qu'ils ne bougent pendant le fonctionnement.

Installation du module ESP32 :

Montez le module ESP32 sur le châssis.
Placez l'ESP32 sur son support et fixez-le.

Installation du module L298N :

Prendre le module L298N sur le châssis.
Placez le module L298N sur son support et fixez-le.

Installation du servo-moteur :

Placer le servo-moteur sur son support créer sur le chassis.
Mettre l'écrou sur le palonier et placer installer l'écrou sur la denture de la crémaillère.

## Étape 3 : Connectique entre les Composants

Connexion du module L298N aux moteurs :

Connectez les bornes de sortie du module L298N aux bornes des moteurs DC (OUT1 et OUT2 pour un moteur, OUT3 et OUT4 pour l'autre).

Connexion du module ESP32 au module L298N :

Connectez les pins IN1, IN2, IN3, et IN4 du module L298N aux GPIOs appropriés de l'ESP32.
Connectez les pins ENA et ENB du module L298N aux GPIOs de l'ESP32 pour contrôler la vitesse des moteurs.

Connexion du servo moteur :

Connectez le servo moteur à un autre GPIO de l'ESP32.
Connectez le fil de signal du servo au GPIO choisi, et les fils d'alimentation et de masse aux pins 3V3 et GND de l'ESP32.

Alimentation :

Connectez une source d'alimentation appropriée au module L298N pour alimenter les moteurs (Vs=7,5V).
Assurez-vous que l'ESP32 est alimenté correctement via le module L298N sur l'entrée (Vss=5V).


ChatGPT
Notice de Création d'une Voiture RC
Étape 1 : Téléchargement des Pièces 3D
Téléchargement des fichiers STL :

Allez sur un site de partage de fichiers 3D comme Thingiverse ou MyMiniFactory.
Recherchez et téléchargez les fichiers STL pour les composants suivants :
Châssis
Crémaillère
Supports de moteur
Support pour ESP32
Support pour le module L298N
Préparation des fichiers pour l'impression :

Importez les fichiers STL dans un logiciel de découpe comme Cura.
Configurez les paramètres d'impression en fonction de votre imprimante 3D (matériau, résolution, etc.).
Générez le fichier G-code et transférez-le sur votre imprimante 3D.
Impression des pièces :

Lancez l'impression des pièces une par une.
Vérifiez chaque pièce après impression pour s'assurer qu'elle est correctement imprimée et sans défauts.
Étape 2 : Installation des Composants sur le Châssis
Assemblage du châssis :

Fixez les supports de moteur sur le châssis avec des vis et des écrous.
Installez la crémaillère et assurez-vous qu'elle est bien en place et fonctionne correctement.
Montage des moteurs :

Placez les moteurs DC dans les supports prévus à cet effet sur le châssis.
Fixez les moteurs solidement pour éviter qu'ils ne bougent pendant le fonctionnement.
Installation du module ESP32 :

Montez le support du module ESP32 sur le châssis.
Placez l'ESP32 sur son support et fixez-le avec des vis.
Installation du module L298N :

Fixez le support du module L298N sur le châssis.
Placez le module L298N sur son support et fixez-le avec des vis.
Étape 3 : Connectique entre les Composants
Connexion du module L298N aux moteurs :

Connectez les bornes de sortie du module L298N aux bornes des moteurs DC (sortie A pour un moteur, sortie B pour l'autre).
Connexion du module ESP32 au module L298N :

Connectez les pins IN1, IN2, IN3, et IN4 du module L298N aux GPIOs appropriés de l'ESP32.
Connectez les pins ENA et ENB du module L298N aux GPIOs de l'ESP32 pour contrôler la vitesse des moteurs.
Connexion du servo moteur :

Connectez le servo moteur à un autre GPIO de l'ESP32.
Connectez le fil de signal du servo au GPIO choisi, et les fils d'alimentation et de masse aux pins 5V et GND de l'ESP32.
Alimentation :

Connectez une source d'alimentation appropriée au module L298N pour alimenter les moteurs.
Assurez-vous que l'ESP32 est alimenté correctement via une batterie ou une autre source d'alimentation.


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

