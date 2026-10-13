# TP1 — Développement Mobile avec Android Studio

## Informations générales

- **Étudiante :** Mariem Hammouda
- **Formation :** Licence 3 — Sciences Informatiques
- **Spécialité :** Génie Logiciel et Système d'Information (LSI3)
- **Matière :** Développement Mobile
- **Outil de développement :** Android Studio
- **Langage de programmation :** Java
- **Plateforme :** Android

## Objectifs du TP

Ce travail pratique a pour objectifs de :

- Découvrir l'environnement de développement Android Studio.
- Apprendre à créer et configurer un projet Android.
- Comprendre la structure d'un projet Android.
- Découvrir le SDK Android (Software Development Kit).
- Créer et configurer un appareil virtuel Android (AVD).
- Compiler et exécuter une application Android.
- Utiliser Logcat pour consulter les messages de diagnostic.
- Internationaliser une application Android en français et en anglais.

## Présentation du projet

Ce projet consiste à créer une application Android simple avec Android Studio, en utilisant le modèle **Empty Views Activity** et le langage Java.

L'application affiche deux informations :
- La matière : Développement Mobile.
- La filière : LSI3.

L'interface est définie dans un fichier XML et les textes sont stockés dans les ressources de l'application afin de faciliter leur traduction.

## Structure du projet

Les principaux fichiers et répertoires utilisés sont :

```text
Hammouda_Mariem_LSI3_DevMobil_TP1/
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── .../
│           │       └── MainActivity.java
│           ├── res/
│           │   ├── layout/
│           │   │   └── activity_main.xml
│           │   ├── values/
│           │   │   └── strings.xml
│           │   ├── values-en/
│           │   │   └── strings.xml
│           │   └── ...
│           └── AndroidManifest.xml
├── build.gradle.kts
├── settings.gradle.kts
├── gradle.properties
├── gradlew
├── gradlew.bat
└── README.md
```

**Rôle des principaux éléments :**

- `MainActivity.java` : classe principale de l'application.
- `activity_main.xml` : décrit l'interface graphique.
- `strings.xml` : contient les chaînes de caractères de la langue par défaut.
- `values-en/strings.xml` : contient les traductions anglaises.
- `AndroidManifest.xml` : décrit les composants et les caractéristiques principales de l'application.
- `build.gradle.kts` : contient la configuration de compilation du module.
- `res/` : contient les ressources de l'application, notamment les interfaces, les images et les textes.

*Remarque : la structure exacte peut varier légèrement selon la version d'Android Studio.*

## Exercice 1 — Création d'un AVD

L'objectif de cet exercice est de créer un appareil Android virtuel pour tester l'application.

Configuration demandée :

- **Type :** Phone.
- **Taille d'écran :** 5,1 pouces.
- **Résolution :** 480 × 800 pixels.
- **Densité :** mdpi.
- **Version Android :** Android 8.1.
- **Niveau d'API :** 27.
- **RAM :** 512 Mo.

L'AVD permet de simuler un smartphone Android sans utiliser obligatoirement un appareil physique.

## Exercice 2 — Internationalisation de l'application

Cet exercice consiste à modifier l'interface de l'application et à proposer deux versions linguistiques.

### Version française

```text
Matière : Développement Mobile
Filière : LSI3
```

### Version anglaise

```text
Subject: Mobile Development
Major: LSI3
```

Les textes sont définis dans les ressources `strings.xml` plutôt que directement dans le fichier XML de l'interface.

Android utilise les ressources linguistiques correspondant à la langue sélectionnée sur l'appareil. Le fichier `values/strings.xml` contient les textes par défaut, tandis que `values-en/strings.xml` contient les traductions anglaises.

Cette organisation facilite l'ajout d'autres langues sans devoir modifier la structure de l'interface.

## Compilation et exécution

L'application peut être compilée et exécutée depuis Android Studio.

Les tests peuvent être effectués :
- Sur un émulateur Android.
- Sur un smartphone physique compatible, connecté à l'ordinateur.

L'outil **Logcat** permet de consulter les messages de diagnostic et de faciliter la recherche d'éventuelles erreurs.

## Livrables

Les livrables prévus pour ce TP sont :

1. Un document Word nommé `Hammouda_Mariem_TP1.docx`, contenant les captures d'écran des différentes étapes.
2. Le projet Android publié sur GitHub.

## Auteur

**Mariem Hammouda**  
Licence 3 — Sciences Informatiques  
Spécialité Génie Logiciel et Système d'Information

---

*Projet réalisé dans le cadre du TP1 de Développement Mobile.*
