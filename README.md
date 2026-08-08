# 🌍 Global Sustainable Energy Analysis (2000–2020)

> **High Dimensional Statistics** — Master 2 TIDE, Université Paris 1 Panthéon-Sorbonne
> Academic year 2025–2026 | Professor: Alain Celisse

---

## 📌 Project Overview

This project analyses the **Global Sustainable Energy dataset** (2000–2020), covering 176 countries and 21 energy, economic and environmental indicators. The goal is to uncover country energy profiles, track their evolution over two decades, and predict key energy indicators using machine learning methods.

The project is structured around three research questions:

| # | Research Question | Method | Author |
|---|---|---|---|
| Q1 | Predicting primary energy consumption per capita | LASSO, Ridge, OLS | A.-E. Makosso |
| Q2 | Predicting access to clean fuels for cooking | XGBoost | A. Sellami |
| **Q3** | **Identifying country energy profiles & temporal evolution** | **PCA + K-Means** | **A. Mattei** |

---

## 🔬 My Contribution — Q3: Country Energy Profiling via PCA & K-Means

### Objective
Identify latent energy profiles across 148 countries and track their structural evolution from 2000 to 2020 using high-dimensional statistical methods.

### Methodology
- **12 variables** selected: electricity access, clean fuels, renewable share, fossil/nuclear/renewable electricity, low-carbon %, energy per capita, energy intensity, CO₂ emissions, GDP per capita, financial flows
- **PCA** (standardised): PC1 captures energy development level (43.5%), PC2 captures energy mix (14.2%) → 80% variance explained by 3 components
- **K-Means clustering** (K=4) applied on the first 5 principal components
- **Temporal analysis**: country trajectories mapped from 2000 → 2020 in PCA space

### Results — 4 Country Clusters

| Cluster | Profile | Examples |
|---------|---------|---------|
| 0 | Low development / high renewable share | Ethiopia, Nigeria, Sub-Saharan Africa |
| 1 | Fossil-intensive giants | Qatar, USA, Australia |
| 2 | Rich & developed | France, Germany, Japan |
| 3 | Emerging economies | China, India, Brazil, Indonesia |

Key finding: **significant cluster migrations** observed between 2000 and 2020, particularly for emerging economies transitioning toward more developed profiles.

### Visualisations
- Scree plot & cumulative explained variance
- PCA biplot — country projections 2000 vs 2020 (by continent)
- Correlation circle
- Energy transition trajectories (2000 → 2020 arrows)
- K-Means cluster profiles (standardised bar charts)

---

## 🗂️ Repository Structure

```
global-sustainable-energy/
│
├── notebook/
│   └── projet_GD_Alexis.ipynb     # Q3 analysis (PCA + K-Means)
│
├── data/
│   └── final_dataset.csv          # Preprocessed dataset (group work)
│
├── report/
│   └── Gr1_GrandeDimension_2026.pdf  # Full academic report (Group 1)
│
└── README.md
```

> **Note:** The original raw dataset is publicly available on [Kaggle — Global Data on Sustainable Energy](https://www.kaggle.com/datasets/anshtanwar/global-data-on-sustainable-energy).

---

## 🛠️ Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat)

**Methods:** PCA · K-Means · Standardisation · Temporal trajectory analysis

---

## 👤 Author

**Alexis Mattei** — Data Scientist @ Groupe BPCE | MSc Data Science, Paris 1 Panthéon-Sorbonne

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/alexis-mt)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/alexissmtt)
