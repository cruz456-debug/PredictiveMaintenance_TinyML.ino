# PredictiveMaintenance_TinyML.ino

# TinyML-Based Predictive Maintenance System
**Intelligence Artificielle Embarquée et IoT Industriel**

## Présentation
Ce projet implémente un système de détection d'anomalies en temps réel pour moteurs industriels, utilisant le **Machine Learning sur microcontrôleur (TinyML)**. Contrairement aux systèmes classiques qui envoient les données sur le Cloud, ce système effectue l'inférence localement, garantissant une latence nulle et une confidentialité totale des données.

## Architecture Technique
* **Acquisition :** Accéléromètre 3 axes (MPU6050) capturant les vibrations à haute fréquence (50Hz).
* **Prétraitement :** Transformation de Fourier Rapide (FFT) et calcul des caractéristiques spectrales (Spectral Features).
* **Modèle IA :** Réseau de neurones à couches denses (DNN) entraîné avec **Edge Impulse** et optimisé pour le runtime C++ de l'ESP32.
* **Inférence :** Détection de 3 états : *Normal*, *Anomalie de roulement*, *Surcharge moteur*.

## Points Techniques Clés
* **Edge Computing :** Réduction drastique de la bande passante en ne transmettant que les alertes, pas les données brutes.
* **Optimisation Mémoire :** Modèle quantifié (INT8) pour minimiser l'empreinte RAM/Flash sur l'ESP32.
* **Signal Processing :** Analyse fréquentielle pour identifier les signatures vibratoires des pannes.

## Compétences Validées
* Workflow complet de Machine Learning (Collecte -> Entraînement -> Déploiement).
* Programmation de systèmes temps réel contraints en mémoire.
* Expertise en Industrie 4.0 et maintenance prédictive.

---
**Développeur :** Dylan Bassinga  
*L3 Applied Informatics (ETSE) - Spécialisation Systèmes Embarqués*
