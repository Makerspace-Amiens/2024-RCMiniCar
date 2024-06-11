---
layout: default
nav_order: 6
title: Conception et prototypage
---

# Conception et prototypage
**Chassîs** 

  
Nous avons tout d’abord élaboré un plan sur papier pour estimer approximativement les tailles de nos composants ainsi que leurs emplacements. Après avoir eu une idée générale de la forme et des dimensions de notre châssis, Jules s'est chargé de le réaliser en 3D. Dans un premier temps, il a conçu un châssis très simple afin de tester les composants, commencer le câblage, le codage et vérifier le fonctionnement de la crémaillère.

Ensuite, nous avons développé un châssis plus opérationnel, avec des emplacements spécifiques pour chaque composant et des moyens de fixation adaptés. Pour ce faire, nous avons réalisé un assemblage sur SolidWorks, incluant tous les composants modélisés en 3D, afin d'obtenir les dimensions exactes de chaque élément. Cette étape nous a permis d’assurer une précision optimale dans la disposition et la fixation de chaque composant.

<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>

<model-viewer id="viewer" alt="Modèle 3D du châssis" src="images/chassis3d.gltf" poster="images/Capture2.PNG" shadow-intensity="1" camera-controls touch-action="pan-y" style="width: 100%; height: 500px;">
</model-viewer>

**Crémaillère**
  
En ce qui concerne la crémaillère, nous avons d'abord effectué des recherches approfondies sur Internet pour comprendre les différents types de crémaillères utilisées dans les voitures réelles, le modélisme et les voitures radiocommandées. Ces informations nous ont permis de concevoir notre propre crémaillère sur SolidWorks.

Après avoir finalisé la conception, nous avons procédé à l'impression 3D de la crémaillère. Cependant, après plusieurs tentatives d'impression infructueuses, nous avons opté pour une impression en résine, beaucoup plus précise pour les petites pièces comme la nôtre. Cette technique nous a permis d'obtenir une crémaillère de haute qualité et adaptée à nos besoins spécifiques.

<model-viewer id="viewer" alt="Modèle 3D de la crémaillère" src="images/AssemblageCremaillere.gltf" poster="/docs/images/capture.jpg" shadow-intensity="1" camera-controls touch-action="pan-y" style="width: 100%; height: 500px;">
</model-viewer>


**Composants/Connectique**

Nous avons choisi divers composants pour réaliser cette voiture RC. Tout d'abord, nous avons fait des recherches pour déterminer quels moteurs étaient les plus propices à notre projet. Finalement, nous avons décidé de prendre des motoréducteurs moins encombrants et moins puissants. Ensuite, nous avons pris un ESP32 pour faire la relation entre les composants et nous permettre de le coder et de le contrôler soit par WiFi ou Bluetooth. D'autre part, pour faire la relation entre l'ESP32 et les motoréducteurs, nous avons pris un driver LN298 qui permet de contrôler les deux moteurs continus. Il peut faire tourner les moteurs à une vitesse continue ou en PWM. De plus, il inclut des diodes pour protéger le circuit, des résistances de rappel et un dissipateur de chaleur en cas de forte charge. Enfin, pour la direction de la voiture, nous avons pris un servo-moteur qui contribue à faire glisser la crémaillère de droite vers la gauche.

<model-viewer id="viewer" alt="Modèle 3D des moteurs" src="images/moteur RC.gltf" poster="images/capture.jpg" shadow-intensity="1" camera-controls touch-action="pan-y" style="width: 100%; height: 500px;">
</model-viewer>
<model-viewer id="viewer" alt="Modèle 3D du driver" src="images/Driver.gltf" poster="images/capture.jpg" shadow-intensity="1" camera-controls touch-action="pan-y" style="width: 100%; height: 500px;">
</model-viewer>
<model-viewer id="viewer" alt="Modèle 3D de l'ESP32" src="images/ESP32.gltf" poster="images/capture.jpg" shadow-intensity="1" camera-controls touch-action="pan-y" style="width: 100%; height: 500px;">
</model-viewer>
<model-viewer id="viewer" alt="Modèle 3D du servomoteur" src="images/Servo.gltf" poster="images/capture.jpg" shadow-intensity="1" camera-controls touch-action="pan-y" style="width: 100%; height: 500px;">
</model-viewer>


Pour la connectivité, nous avons utilisé des fils mâle/femelle et femelle/femelle pour connecter les différents composants entre eux. Cela assure une connexion fiable et flexible pour tous les éléments de la voiture RC.


