🌍 Étude Météorologique Interactive : Pipeline Big Data & BI
📌 Présentation du Projet
Ce projet, réalisé dans le cadre de ma Licence 3 en Big Data, vise à analyser plus de 95 000 relevés météorologiques sur une période de 10 ans. L'objectif était de construire un pipeline ETL complet, de la donnée brute (CSV) jusqu'à une visualisation interactive permettant de comprendre les corrélations climatiques.

🛠️ Architecture Technique
Le projet suit une architecture de type Data Warehouse avec un modèle en étoile :

Ingestion & Nettoyage (Python/PySpark) : * Traitement massif des données avec Spark pour assurer la scalabilité.

Nettoyage des valeurs manquantes et formatage des types (Dates, Décimales).

Modélisation (Star Schema) :

Table de Faits : fait_releves (Température, Humidité, Vent).

Tables de Dimensions : dim_temps (Années, Mois, Jours) et dim_condition (Summary, Precip).

Analyse Statistique :

Calcul des coefficients de corrélation de Pearson.

Utilisation de modèles de régression pour valider les tendances.

📊 Visualisation (Tableau Public)
Le dashboard final permet une exploration multidimensionnelle :

Bandeau de KPIs : Affichage en temps réel de la température moyenne globale, du taux d'humidité et du volume total de données.

Analyse Temporelle : Graphique d'évolution permettant le "drill-down" de l'année vers le mois.

Matrice de Corrélation : Visualisation Heatmap montrant la relation inverse entre la température et l'humidité.

Interactivité : Filtrage dynamique de tout le dashboard en cliquant sur les conditions météo (ex: Nuageux, Pluvieux).

🚀 Comment exécuter le projet ?
Cloner le dépôt :

Bash
git clone https://github.com/ton-pseudo/projet-meteo-bigdata.git
Exécuter le script de nettoyage :
Ouvrez le dossier scripts/ et lancez le notebook PySpark pour générer les fichiers CSV propres.

Visualisation : https://public.tableau.com/app/profile/philemon.kubuya/viz/Classeur1_17740257068620/Tableaudebord1?publish=yes
