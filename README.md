# Automatidata-Taxi-Fare-Prediction
Modèle de régression linéaire pour prédire les tarifs des taxis de NYC (Projet Automatidata).

# Automatidata : Prédiction des Tarifs de Taxi (NYC TLC)

## 📌 Présentation du Projet
Ce projet a été réalisé pour la **New York City Taxi and Limousine Commission (TLC)**. L'objectif principal était de transformer les données massives de trajets (plus de 1 million de trajets quotidiens) en un outil prédictif capable d'estimer les tarifs des courses avant le départ.

Cette solution permet d'améliorer la transparence pour les clients et d'offrir une aide à la décision stratégique pour la régulation des tarifs.

## 🛠️ Stack Technique
* **Langage :** Python 3
* **Analyse de données :** Pandas, Numpy
* **Visualisation :** Matplotlib, Seaborn
* **Machine Learning :** Scikit-learn (Multiple Linear Regression)

## 📊 Méthodologie & Analyse
Le projet a suivi les étapes clés du cycle de vie de la donnée :
1. **EDA (Exploratory Data Analysis) :** Analyse des distributions et traitement des valeurs aberrantes (outliers) sur les tarifs et les distances.
2. **Ingénierie des caractéristiques :** Création de variables pertinentes pour capturer la relation entre durée, distance et coût.
3. **Modélisation :** Mise en œuvre d'une Régression Linéaire Multiple.
4. **Évaluation :** Vérification des hypothèses de régression (homoscédasticité, normalité des résidus).

## 🚀 Résultats du Modèle
Le modèle final présente des performances solides, indiquant une grande fiabilité pour les prédictions en conditions réelles :

| Métrique | Valeur |
| :--- | :--- |
| **R² (Coefficient de détermination)** | **0,87** |
| **MAE (Erreur Absolue Moyenne)** | **2,10 $** |
| **RMSE (Racine de l'Erreur Quadratique Moyenne)** | **3,80 $** |

> **Insight Clé :** La **durée du trajet** est le facteur le plus influent sur le prix de la course. Le modèle explique environ **87%** de la variance des tarifs observés.

## 📁 Structure du Dépôt
* `Automatidata_projec.ipynb` : Le notebook complet contenant le code, les visualisations et l'entraînement du modèle.
* `reports/` : Contient le résumé exécutif destiné aux parties prenantes (Executive Summary).

## 📈 Recommandations Business
Sur la base de cette analyse, il est recommandé à la NYC TLC de :
* Intégrer ce modèle dans une application client pour afficher une estimation tarifaire avant la course.
* Collecter des données supplémentaires sur les itinéraires sous-représentés pour affiner la précision locale.
