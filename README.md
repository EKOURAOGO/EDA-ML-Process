# Guide EDA-ML — Exploration des Données pour le Machine Learning

Guide structuré et complet pour réaliser une **Exploration des Données (EDA)** dans un projet
de Machine Learning, avec des étapes détaillées et des exemples de code Python.

---

## Contenu

Le guide `EDA_guide.md` couvre 10 étapes essentielles :

| Étape | Description |
|-------|-------------|
| 1. Comprendre le problème | Objectif métier, variables clés, contraintes, hypothèses |
| 2. Chargement & exploration | `df.head()`, `df.shape`, `df.info()`, cardinalité |
| 3. Qualité des données | Valeurs manquantes, doublons, types, outliers |
| 4. Analyse univariée | Statistiques descriptives, distributions numériques et catégorielles |
| 5. Analyse bivariée & multivariée | Corrélations, scatter plots, heatmaps, VIF, PCA |
| 6. Feature engineering | Nouvelles variables, encodage, transformations (log, Box-Cox) |
| 7. Détection des anomalies | Boxplots, Z-score, IQR, Isolation Forest, DBSCAN, LOF |
| 8. Gestion des valeurs manquantes | Imputation simple (médiane, mode) et avancée (KNN, EM) |
| 9. Validation & sauvegarde | Récapitulatif des transformations, vérifications finales |
| 10. Synthèse & prochaines étapes | Découvertes, points de vigilance, sélection de modèles |

---

## Utilisation

Ce guide est conçu comme une **checklist de référence** à suivre au début de tout projet ML.

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# Étape 2 — Exploration initiale
df = pd.read_csv('data.csv')
print(df.shape)
print(df.info())
print(df.describe())

# Étape 3 — Valeurs manquantes
print(df.isnull().sum())
sns.heatmap(df.isnull(), cbar=False)

# Étape 5 — Corrélations
sns.heatmap(df.corr(), annot=True, cmap='coolwarm')
```

---

## Structure du repo

```
EDA-ML-Process/
├── EDA_guide.md    # Guide complet EDA en 10 étapes
└── README.md
```

---

## Stack technique

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-visualization-blue?style=flat-square)

---

## Auteur

**Emmanuel KOURAOGO** — M2 IMSD
[GitHub](https://github.com/EKOURAOGO) · [Email](mailto:ekouraogo73@gmail.com)
