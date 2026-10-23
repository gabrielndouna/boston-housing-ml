# 🏠 Boston Housing Price Prediction - Machine Learning (Supervised Learning)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-LinearRegression-orange.svg)
![Matplotlib](https://img.shields.io/badge/Visualization-Matplotlib-green.svg)

## 📌 Présentation du Projet
Ce projet met en œuvre une démarche d'**apprentissage supervisé** (*Supervised Learning*) pour prédire la valeur médiane des logements dans la région de Boston (`MEDV`). 

L'objectif principal est de suivre une méthodologie d'analyse granulaire ("une action par cellule") couvrant l'ensemble du workflow Machine Learning : exploration, nettoyage, visualisation avec Matplotlib, modélisation et prédiction.

---

## 📊 Jeu de Données
- **Nom :** Boston Housing Dataset (`BostonHousing.csv`)
- **Taille :** 506 observations, 14 variables
- **Variable cible ($y$) :** `MEDV` (Valeur médiane des maisons occupées par leur propriétaire, en milliers de $)
- **Variables explicatives ($X$) :** 13 caractéristiques urbaines, sociales et structurelles (ex: `RM` nombre de pièces, `CRIM` taux de criminalité, `LSTAT` statut socio-économique).

---

## 🛠️ Stack Technique & Outils
- **Langage :** Python 3
- **Manipulation de Données :** Pandas, NumPy
- **Visualisation de Données :** Matplotlib (`plt`)
- **Machine Learning :** Scikit-Learn (`LinearRegression`, `train_test_split`)

---

## 📈 Démarche & Résultats Clés

### 1. Exploration & Contrôle Qualité (EDA)
- Inspection de la structure (`shape`, `head`, `info`).
- Validation de la qualité des données : **0 valeur manquante** et **0 doublon**.

### 2. Analyse Exploratoire Visuelle (Matplotlib)
- **Distribution de la cible :** L'histogramme montre une distribution centrée autour de $20\,000$ \$ - $25\,000$ \$.
- **Corrélations :** La matrice de corrélation et le nuage de points (*Scatter Plot*) confirment une forte relation linéaire positive entre le nombre moyen de pièces (`RM`) et la valeur médiane (`MEDV`).

### 3. Modélisation & Évaluation
- **Modèle :** Régression Linéaire Multiple
- **Découpage :** 80% entraînement / 20% test
- **Performances ($R^2$) :**
  - **Score Entraînement ($R^2$) :** `0.719` ($71.9\%$)
  - **Score Test ($R^2$) :** `0.691` ($69.1\%$)

> **Conclusion :** L'écart très faible entre le score d'entraînement et le score de test démontre que le modèle généralise très bien sur de nouvelles données sans subir de surapprentissage (*overfitting*).

---

## 🚀 Comment exécuter ce projet en local ?

1. Cloner ce dépôt :
   ```bash
   git clone [https://github.com/votre-compte/boston-housing-ml.git](https://github.com/votre-compte/boston-housing-ml.git)
