# MaeS'Stro

# Auteur : Sarah MARECAR

## Description

MaeS'Stro est une application mobile Android qui permet d'extraire des informations importantes sur un sujet en question. L'utilisateur peut entrer un mot-clé dans une barre de recherche, et l'application affiche des graphes interactifs avec les mots-clés les plus importants liés au sujet. En cliquant sur un graphe, l'utilisateur peut obtenir les informations essentielles sur le sujet, notamment les faits, les sujets d'actualité et les sentiments évoqués. Le besoin essentiel dans ce projet est de permettre aux utilisateurs d'atteindre facilement les sujets d'actualités et si le sujet n'est pas dans la connaissance de l'utilisateur, il doit pouvoir rapidement monter en compétences dessus et connaître les tendances sentimentales sémantiques. Ce projet est un premier jet à l'analyse sémantique en masse, est tend à une évolution sous une autre version.

## Spécifications Fonctionnelles

### Fonctionnalités Principales

1. **Sujets Tendance Actuels**
   - Affichage des sujets tendances provenant de Twitter et LinkedIn.
   - Options de filtres pour choisir les sources et les catégories.
   - Rafraîchissement des sujets tendances.

2. **Recherche de Sujet**
   - Barre de recherche pour entrer un mot-clé.
   - Résultats de recherche sous forme de graphes de bulles représentant les mots-clés associés.
   - Options de tri et zoom sur les bulles.

3. **Détails du Sujet**
   - Description détaillée du mot-clé.
   - Présentation des sujets d'actualité liés.
   - Analyse des sentiments (positif, négatif, neutre).
   - Liens vers les sources et options de partage.

### Interface Utilisateur (UI)

1. **Écran d'Accueil**
   - Affichage des sujets tendances avec icônes des réseaux sociaux.
   - Barre de recherche et filtres.
   - Bouton de rafraîchissement.

2. **Écran de Recherche**
   - Résultats de recherche sous forme de graphes de bulles.
   - Fonctionnalité de zoom et options de tri.

3. **Écran de Détails**
   - Description, actualités, et analyse des sentiments.
   - Liens vers les sources et bouton de partage.

## Spécifications Techniques

### Technologies Utilisées

- **Langage de Programmation**: Java/Kotlin
- **IDE**: Android Studio
- **Backend**: Firebase ou Node.js (selon les besoins)
- **Base de Données**: Firestore (Firebase) ou MongoDB
- **API de Recherche**: OpenAI API
- **Bibliothèques de Visualisation**: MPAndroidChart pour les graphes
- **NLP et Analyse des Sentiments**: OpenAI API, Google Cloud Natural Language API, IBM Watson

### Architecture de l'Application

1. **Frontend (Application Mobile)**
   - Android avec Java/Kotlin
   - Interface utilisateur pour la recherche, l'affichage des résultats et les détails

2. **Backend**
   - Serveur Node.js pour traiter les requêtes API
   - Firebase pour l'authentification et la base de données

3. **Intégration de l'API OpenAI**
   - Requêtes à l'API OpenAI pour obtenir des informations sur les mots-clés
   - Traitement et affichage des résultats dans l'application

### Fonctionnement de l'Application

1. **Sujets Tendance**
   - Affichage des sujets tendances actuels sur l'écran d'accueil.
   - Options de filtre et de rafraîchissement.

2. **Recherche**
   - L'utilisateur entre un mot-clé et soumet la recherche.
   - Le frontend envoie une requête au backend avec le mot-clé.

3. **Traitement**
   - Le backend envoie une requête à l'API OpenAI pour obtenir des informations.
   - Les données reçues sont traitées et formatées pour l'affichage.

4. **Affichage**
   - Les résultats sont renvoyés au frontend et affichés sous forme de graphes.
   - L'utilisateur peut cliquer sur un graphe pour voir les détails (faits, actualités, sentiments).

### Déploiement

1. **Configuration de Firebase/Node.js**
   - Configuration et déploiement du backend.
   - Configuration de la base de données.

2. **Développement Mobile**
   - Ouvrez le projet dans Android Studio.
   - Configurez les dépendances et lancez l'application sur un émulateur ou un appareil réel.

## Guide d'Installation

1. **Clone du Dépôt**
   ```bash
   git clone https://github.com/MaeS-Stro/MaeSStro.git
   cd MaeSStro
