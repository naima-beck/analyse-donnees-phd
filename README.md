# Analyse de Données : thèse de doctorat en France

Ce projet s'inscrit dans le cadre du cours d'Analyse de Données de Cy Tech et Sciences-Po Saint-Germain-En-Laye. Il comprend la manipulation, le nettoyage et l'analyse de plusieurs jeux de données. Ce vise à analyser l'évolution de l'usage de l'anglais dans les thèses de doctorat en France, mettant ainsi en lumière une tendance croissante liée aux injonctions institutionnelles et à l'internationalisation de la recherche. Parallèlement, nous relèverons une saisonnalité marquée des soutenances, concentrées début décembre en raison des échéances administratives. Enfin, l'exploitation statistique du jeu de données PHD via R permet de quantifier ces phénomènes et d'éclairer les tensions entre francophonie académique et mondialisation scientifique.

## Objectifs

- Maîtriser les techniques de prétraitement et manipulation de données
- Identifier et traiter les données manquantes et outliers
- Produire des visualisations pertinentes
- Analyser un jeu de données complexe 

## Technologies utilisés
- **Langage** : R
- **Outils** : Jupyter Notebook, Overleaf (LaTeX)
- **Bibliothèques principales** : 
  - `dplyr`, `tidyr` : Manipulation de données
  - `ggplot2`, `patchwork` : Visualisation
  
## Installation

### Cloner le repository

```bash
git clone https://github.com/naima-beck/analyse-donnees-phd.git
cd analyse-donnees-phd
```
### Données
Les données brutes sont disponibles sur [Caisses des Dépôts](https://opendata.caissedesdepots.fr/explore/dataset/moncompteformation_formations_engagees/information/?disjunctive.domaine_formation_nsf&disjunctive.region_lieu_formation&disjunctive.departement_lieu_formation&disjunctive.intitule_certification).
le nommer : moncompteformation_formations_engagees.csv

[Institut national d'etudes démographiques](https://www.ined.fr/fr/tout-savoir-population/chiffres/france/structure-population/regions/)
le nommer : .csv 

Placez les fichiers `moncompteformation_formations_engagees.csv`et `.csv`  dans le dossier `data/` avant d'exécuter les notebooks.

### Structure du projet

```bash
analyse-donnees-phd/
├── data/ # Jeux de données
│ ├── age_gender.csv
│ ├── formations_engagees.csv
│ └── theses_doctorat.csv
├── notebooks/ # Notebooks Jupyter
│ ├── .ipynb
│ ├── .ipynb
│ └── .ipynb
├── Rapport
│ 
├── references/ # énoncé
└── README.md
```
## Jeux de Données analysés

### 1. Données Âge-Genre
- Distribution par tranches d'âge
- Comparaison hommes/femmes
- Visualisations avec matplotlib/ggplot2

### 2. Formations Engagées (CDC)
- Taux de complétion par département
- Analyse géographique des formations
- Calcul des montants engagés

### 3. Thèses de Doctorat (1985-2020)
- Données manquantes et patterns
- Distribution temporelle des soutenances
- Analyse des directeurs de thèse
- Évolution des langues de rédaction


## Quelques résultats 

### Visualisations Produites
- Heatmaps des données manquantes (missingno)

- Distribution mensuelle des soutenances

- Évolution des langues de rédaction

- Analyse des outliers parmi les directeurs

### Analyses Réalisées
- Détection de patterns dans les données manquantes

- Identification des périodes préférées pour les soutenances

- Étude des homonymes (cas Cécile Martin)

- Calcul des taux de réalisation par région



## Références

- **[Énoncé du projet](./references/enonce_projet.pdf)**

## Auteur

[@naima-beck](https://www.github.com/naima-beck) - Cy Tech - Sciences-Po Saint-Germain-En-Laye - [2024/2025]


## License

Ce projet est réalisé dans un cadre académique. Les données sont fournies pour usage pédagogique.
Il est sous licence [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
![License](https://img.shields.io/badge/License-CC%20BY--NC--SA-blue.svg)
