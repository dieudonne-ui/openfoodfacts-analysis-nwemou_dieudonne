# openfoodfacts-analysis-nwemou_dieudonne
Scraping, nettoyage et analyse de produits alimentaires OpenFoodFacts



 **Analyse des Produits Alimentaires — OpenFoodFacts

Scraping • Nettoyage • Analyse Exploratoire • Visualisations**

Ce projet a pour objectif de collecter, nettoyer et analyser un ensemble de données provenant de la base ouverte OpenFoodFacts, en utilisant des techniques de web scraping, de nettoyage avancé, d’analyse exploratoire (EDA) et de visualisation.

Il a été réalisé dans le cadre d'un exercice complet d’analyse de données, intégrant Python, Pandas, Matplotlib/Seaborn et Power BI.

🔍 🎯 Objectif du projet

L’objectif principal est de :

Scraper des données réelles depuis l’API OpenFoodFacts

Construire un dataset propre et exploitable

Analyser les produits alimentaires selon leurs valeurs nutritionnelles

Créer des visualisations pour extraire des tendances

Produire un tableau de bord Power BI pour une analyse interactive



🌐 1. Collecte des données (Scraping)

Les données proviennent de la plateforme OpenFoodFacts, via l’API publique :

Extraction d’un large échantillon de produits

Sélection des variables pertinentes :

Nom du produit

Marque

Pays

Catégorie

Énergie (kcal/100g)

Graisses (g/100g)

Sucres (g/100g)

Protéines (g/100g)

Score nutritionnel (Nutri-Score)

Le scraping a été réalisé dans un notebook Google Colab 

 2. Nettoyage des données

Plusieurs étapes de nettoyage ont été nécessaires :

Suppression des doublons

Traitement des valeurs manquantes

Normalisation des noms de pays

Conversion des colonnes numériques (text → float)

Filtrage des produits exploitables

Sélection des colonnes finales

👉 Le dataset final contient 2873 produits exploitables.

📊 3. Analyse et Visualisations

L’analyse exploratoire a porté sur :

🔢 Analyses statistiques

stats descrribre des valeurs nutritionnelle

Répartition par catégories

Top produits les plus gras

Top produits avec meilleur score nutritionnel

Bottom produits nutritionnellement faibles

🗺️ Visualisations Python

Histogrammes

Camemberts

Heatmap de matrice de corrélation

Graphiques de distribution

Bar charts pour les top/bottom produits

📈 Power BI

Un tableau de bord inclut :

Filtre par pays
top pays et top score
Camemberts







Structure du Dépôt
openfoodfacts-analysis/
│
├── data/
│     └── openfoodfacts_cleaned.csv        # Dataset final nettoyé
│
├── notebooks/
│     └── openfoodfacts_analysis.ipynb     # Notebook complet avec scraping & analyses
│
├── powerbi/
│     └── dashboard.pbix                   # Tableau de bord Power BI (optionnel)
│
└── README.md                              # Documentation du projet



Technologies utilisées
Outil	            Usage
Python	          Scraping, nettoyage, analyse (Pandas, Requests)
Google Colab	    Hébergement du notebook
Pandas	          Manipulation du dataset
Matplotlib / Seaborn	Visualisations
Power BI	       Tableau de bord interactif
Git / GitHub	    Versioning & partage



🔁 Reproduire le projet
1️⃣ Cloner le dépôt
git clone lien du ripo
cd openfoodfacts-analysis

2️⃣ Installer les dépendances
pip install pandas requests matplotlib seaborn

3️⃣ Lancer le notebook

Ouvre :

notebooks/openfoodfacts_analysis.ipynb


et exécute les cellules dans l’ordre.



Auteur

N'WEMOU DIEUDONNE
Développeur Web FullStack(javascipt) • Africa citizen Data Scientist
dieudonnenwemou4@gmail.com
+229 01 66 03 85 12
📍 Bénin





Répartition des produits par pays

Analyse du score nutritionnel
