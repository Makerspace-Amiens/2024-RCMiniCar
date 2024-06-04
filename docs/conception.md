---
layout: default
nav_order: 5
title: Conception et prototypage
---

# Conception et prototypage
# Chassîs
Nous avons tout d’abord élaboré un plan sur papier pour estimer approximativement les tailles de nos composants ainsi que leurs emplacements. Après avoir eu une idée générale de la forme et des dimensions de notre châssis, Jules s'est chargé de le réaliser en 3D. Dans un premier temps, il a conçu un châssis très simple afin de tester les composants, commencer le câblage, le codage et vérifier le fonctionnement de la crémaillère.

Ensuite, nous avons développé un châssis plus opérationnel, avec des emplacements spécifiques pour chaque composant et des moyens de fixation adaptés. Pour ce faire, nous avons réalisé un assemblage sur SolidWorks, incluant tous les composants modélisés en 3D, afin d'obtenir les dimensions exactes de chaque élément. Cette étape nous a permis d’assurer une précision optimale dans la disposition et la fixation de chaque composant.

# Crémaillère 
En ce qui concerne la crémaillère, nous avons d'abord effectué des recherches approfondies sur Internet pour comprendre les différents types de crémaillères utilisées dans les voitures réelles, le modélisme et les voitures radiocommandées. Ces informations nous ont permis de concevoir notre propre crémaillère sur SolidWorks.

Après avoir finalisé la conception, nous avons procédé à l'impression 3D de la crémaillère. Cependant, après plusieurs tentatives d'impression infructueuses, nous avons opté pour une impression en résine, beaucoup plus précise pour les petites pièces comme la nôtre. Cette technique nous a permis d'obtenir une crémaillère de haute qualité et adaptée à nos besoins spécifiques.

# Composants/Connectique

Nous avons choisis divers composants pour réaliser cette voiture RC. Tout d'abord, Nous avons fait des recherches sur quels moteurs étaient les plus propises à notre projet. Finalement nous avons décidé de prendre des motoréducteurs moins encombrants et moins puissants. Ensuite, Nous avons pris un ESP32 pour faire la relation entre les composants et nous permettre de le coder et le controller soit par wifi ou bluetooth. D'autre part, pour faire la relation entre l'ESP32 et les motoréducteurs, nous avons pris en driver LN298 qui permet de contrôler les 2 moteurs continus. Il peut faire tourner les moteurs en vitesse continue ou en PWM. De plus, il inclut des diodes pour protéger le circuit, des résistances de rappel et un dissipateur de chaleur en cas de forte charge.
Enfin, Pour la direction de la voiture, nous avons pris un servo-moteur qui contribu à faire glisser la crémaillère de droite vers la gauche.

Pour la connectivité, nous avons utilisé des fils male/femmelle et femelle/femelle. Pour ce qui concerne la batterie nous avons pris

# Programmation

Pour ce qui est de la programmation, nous avons choisi de piloté la voiture RC sur notre smarphone soit par wifi ou par bluetooth. Nous avons fait des recherches poussées sur internet. Puis nous avons décidé d'utilisé l'interface Blynk qui utilise le wifi et l'interface Dabble qui utilise le Bluetooth.
Nous avons codé sur Arduino le code pour chaque interface puis nous l'avons téléverser dans l'ESP32. Ainsi, nous pouvons controlé l'ESP32 soit par wifi avec Blynk ou par Bluetooth avec Dabble sur notre smarphone.
