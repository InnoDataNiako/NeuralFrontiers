# Analyse COVID-19 Sénégal - Février à Mai 2020
## 🔍 Contexte
-Source : Données officielles du Ministère de la Santé Sénégalais
-Période: 28/02/2020 au 23/05/2020
-Objectif: Analyse de la propagation et impact régional

## 📊 Méthodologie

### Traitement des données
python
# Script de nettoyage principal
df = pd.read_csv("sen_covid_data.csv", parse_dates=['DATE'])
df = df[df['REGION'] != 'Non spécifié']
df['TAUX_MORTALITE'] = (df['DECES'] / df['CONTAMINES'].replace(0, 1)) * 100
Outils utilisés
Python : 3.10

Librairies : Pandas, Seaborn, Matplotlib

Environnement : Jupyter Notebook

📌 Insights Principaux
1. Dynamique Nationale
Courbe épidémique

Période clé : Accélération à partir du 15/03/2020

R0 estimé : 2.3 (calculé par régression linéaire)

2. Analyse Régionale
python
Copy
Régions les plus touchées :
1. Dakar (72% des cas)
2. Thiès (12%)
3. Diourbel (8%)
3. Indicateurs Clés
Métrique	Valeur
Cas confirmés	3,542
Décès	42
Taux de létalité	1.19%
📂 Structure des Données
Copy
data/
├── raw/                # Données brutes
│   └── sen_covid_data.csv
└── processed/          # Données nettoyées
    ├── daily_cases.csv
    └── regional_stats.csv
🛠 Limitations
Données manquantes dans 3 régions avant avril

Biais de reporting en début d'épidémie

🔮 Recommandations
Prioriser la vaccination à Dakar

Renforcer les tests dans les régions frontalières

Mettre en place un dashboard de suivi