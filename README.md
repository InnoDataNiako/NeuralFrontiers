# 🦠 Projet d'Analyse Exploratoire (EDA) - COVID-19 Sénégal

## 📌 Objectif
Ce mini projet vise à analyser les données épidémiologiques du COVID-19 au Sénégal pour identifier :
- Tendances nationales et régionales
- Taux de mortalité par région
- Évolution temporelle des indicateurs clés

## 🗃️ Structure des données
1_EDA-COVID19/
├── data/
│ ├── raw/ # Données brutes (sen_covid_data.csv)
│ └── processed/ # Données nettoyées (senegal_daily_cases.csv)
├── notebooks/ # Jupyter Notebook d'analyse
├── reports/figures/ # Visualisations (graphiques, cartes)
└── resume_analyse.md # Synthèse des résultats

## 📊 Résultats clés
![Graphique d'évolution](reports/figures/Evolution hebdomadaire des indicateurs.png)  
*Exemple : Évolution hebdomadaire des cas confirmés*

## 🛠️ Installation
1. Cloner le dépôt :
git clone https://github.com/InnoDataNiako/NeuralFrontiers.git
Installer les dépendances :
pip install -r requirements.txt
🧑‍💻 Utilisation
Ouvrir le notebook principal :
jupyter notebook 1_EDA-COVID19/notebooks/COVID19_Analysis.ipynb
📝 Licence
Données publiques du Ministère de la Santé du Sénégal (CC-BY 4.0).

💡 Personnalisation possible
Ajoutez un badge de statut :
![Statut](https://img.shields.io/badge/status-active-success)

Insérez un gif d'une visualisation interactive
![Interactive](reports/figures/interactive_plot.html)
