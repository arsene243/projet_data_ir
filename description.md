🌦️ Analyse des Tendances Climatiques avec Apache Spark
📌 Présentation du Projet
Ce projet a été réalisé dans le cadre du module Data Engineering (Licence 3). L'objectif est de mettre en place un pipeline de données complet pour traiter et analyser des données météorologiques historiques.

Le projet couvre l'ensemble du cycle de vie de la donnée : de la collecte sur Kaggle à la modélisation dans un Data Warehouse et la visualisation des tendances climatiques.

🚀 Fonctionnalités
Ingestion de données : Lecture de fichiers CSV volumineux (plus de 96 000 enregistrements).

Nettoyage (Data Cleaning) : Traitement des valeurs manquantes et correction des types de données avec PySpark.

Architecture Décisionnelle : Mise en œuvre d'un modèle de données en étoile (Star Schema) basé sur la méthodologie de Kimball.

Analyse Temporelle : Extraction de tendances (températures moyennes par année/saison).

Visualisation : Graphiques d'évolution climatique.

🏗️ Architecture du Projet
Le projet suit une approche ETL (Extract, Transform, Load) :

Extract : Récupération du dataset weatherHistory.csv.

Transform : Nettoyage et normalisation des données via Apache Spark.

Load : Structuration en tables de faits et de dimensions pour le stockage décisionnel.

Modélisation des Données (Schéma en Étoile)
Conformément aux principes des systèmes décisionnels, les données sont organisées comme suit :

Fait_Releves : Contient les mesures (Température, Humidité, Vitesse du Vent) et les clés étrangères.

Dim_Temps : Attributs temporels (Année, Mois, Jour, Heure) pour l'analyse historique.

Dim_Condition : Attributs qualitatifs (Type de précipitations, Résumé météo).

🛠️ Technologies Utilisées
Langage : Python 3.x

Traitement de données : Apache Spark (PySpark)

Environnement : Google Colab

Bibliothèques : Pandas, Matplotlib, Seaborn

📋 Installation et Utilisation
Cloner le projet :

Bash
git clone https://github.com/ton-utilisateur/projet-data-eng-meteo.git
Exécution sur Google Colab :

Importer le fichier .ipynb dans Colab.

Uploader le fichier weatherHistory.csv.

Exécuter les cellules d'installation de Spark et de traitement.

📊 Résultats et Analyses
Le pipeline permet de répondre à des questions métier telles que :

Quelle est l'évolution de la température moyenne annuelle sur les 10 dernières années ?

Existe-t-il une corrélation entre l'humidité et la visibilité ?
