---
layout: default
title: Code
parent: Notices
nav_order: 1
---
 # Code 

```
#include <DabbleESP32.h>
#include <ESP32Servo.h>

Servo myServo;

// Définir les broches de l'ESP32 connectées au module L298N
#define ENA 21  // Broche pour le PWM du moteur A
#define IN1 4  // Broche pour la direction du moteur A
#define IN2 5 // Broche pour la direction du moteur A
#define ENB 23  // Broche pour le PWM du moteur B
#define IN3 12  // Broche pour la direction du moteur B
#define IN4 13  // Broche pour la direction du moteur B

const int servoPin = 32;

// Angles pour le contrôle du servo
const int angleCentre = 133;  // Position centrale (neutre)
const int angleDroite = 180; 
const int angleGauche = 90;  
void setup() {
  // Initialiser les broches comme sorties
  pinMode(ENA, OUTPUT);
  pinMode(IN1, OUTPUT);
  pinMode(IN2, OUTPUT);
  pinMode(ENB, OUTPUT);
  pinMode(IN3, OUTPUT);
  pinMode(IN4, OUTPUT);
  
  // Initialiser la communication série pour le débogage
  Serial.begin(115200);
  myServo.attach(servoPin);
  
  // Mettre le servo en position neutre
  myServo.write(angleCentre);
  // Initialiser Dabble
  Dabble.begin("Nom_Bluetooth");  
  }

void loop() {

  Dabble.processInput();
  

  if (GamePad.isUpPressed()) {
    avancer();
  } else if (GamePad.isDownPressed()) {
    reculer();

 
  } else {
    arreter();
  }
  if (GamePad.isTrianglePressed()) {
    tournerDroite();
  } 
  
  // Vérifier si le bouton Y est pressé
  if (GamePad.isCirclePressed()	) {
    tournerGauche();
  }
  
  // Vérifier si aucun bouton n'est pressé
  if (!GamePad.isTrianglePressed() && !GamePad.isCirclePressed()) {
    arreterservo();
  }
}

void avancer() {
  // Avancer le moteur A
  digitalWrite(IN1, HIGH);
  digitalWrite(IN2, LOW);
  analogWrite(ENA, 155);  // Vitesse maximale pour le moteur A

  // Avancer le moteur B
  digitalWrite(IN3, HIGH);
  digitalWrite(IN4, LOW);
  analogWrite(ENB, 155);  // Vitesse maximale pour le moteur B

  Serial.println("Les moteurs avancent.");
}

void reculer() {
  // Reculer le moteur A
  digitalWrite(IN1, LOW);
  digitalWrite(IN2, HIGH);
  analogWrite(ENA, 155);  // Vitesse maximale pour le moteur A

  // Reculer le moteur B
  digitalWrite(IN3, LOW);
  digitalWrite(IN4, HIGH);
  analogWrite(ENB, 155);  // Vitesse maximale pour le moteur B

  Serial.println("Les moteurs reculent.");
}
void arreter() {
  // Arrêter le moteur A
  digitalWrite(IN1, LOW);
  digitalWrite(IN2, LOW);
  analogWrite(ENA, 0);  // Arrêter le moteur A

  // Arrêter le moteur B
  digitalWrite(IN3, LOW);
  digitalWrite(IN4, LOW);
  analogWrite(ENB, 0);  // Arrêter le moteur B

  Serial.println("Les moteurs sont arrêtés.");
}
void tournerDroite() {
  myServo.write(angleDroite);
  Serial.println("Tourner à droite");
}

// Fonction pour tourner à gauche
void tournerGauche() {
  myServo.write(angleGauche);
  Serial.println("Tourner à gauche");
}

// Fonction pour arrêter le servo (revenir au centre)
void arreterservo() {
  myServo.write(angleCentre);
  Serial.println("Arrêté (centre)");
}




```
