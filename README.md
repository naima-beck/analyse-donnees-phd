# Analyse de Données : thèse de doctorat en France

Ce projet s’inscrit dans le cadre du cours d’Analyse de Données proposé conjointement par CY Tech et Sciences Po Saint-Germain-en-Laye. Il porte sur l’étude des thèses de doctorat soutenues en France, et plus particulièrement sur l’évolution de l’usage de l’anglais dans leur rédaction. L’objectif est de comprendre comment les dynamiques d’internationalisation et les injonctions institutionnelles influencent les pratiques d’écriture scientifique.

L’analyse met également en évidence une forte saisonnalité des soutenances, concentrées en décembre, ce qui reflète les contraintes administratives et les échéances liées aux concours et commissions d’évaluation.
Grâce à l’exploitation statistique du jeu de données PHD via R, le projet permet de quantifier ces phénomènes et de mettre en lumière les tensions entre francophonie académique et mondialisation scientifique.

## Objectifs

Le projet vise à maîtriser les principales techniques de prétraitement, de nettoyage et de manipulation de données.
Il comprend l’identification et le traitement des valeurs manquantes et des outliers, la production de visualisations pertinentes et l’analyse approfondie de jeux de données complexes.
L’ensemble de ces étapes s’inscrit dans une démarche rigoureuse de compréhension des données relatives aux thèses de doctorat.

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

Placez les fichiers `moncompteformation_formations_engagees.csv`et `.csv`  dans le dossier `data/raw/` avant d'exécuter les notebooks.

### Structure du projet

```bash
analyse-donnees-phd/
├── data/ # Jeux de données
│ ├── raw
│    ├── age_gender.csv
│    ├── moncompteformation_formations_engagees.csv
│    ├── nom.csv
│    ├── PhD.dataset.csv 
│ ├── processed
│    ├── PhD.dataset.clean.csv 
│ ├── external
│    └── fr_population.region.departement.csv
├── notebooks/ # Notebooks Jupyter séparés en fonction des exercices
│ ├── 4.ipynb
│ ├── 5.1.1.ipynb
│ ├── 5.2.1.ipynb
│ ├── 6.1.ipynb
│ ├── 6.2.ipynb
│ ├── 6.3.ipynb
│ └── 6.4.ipynb
├── Rapport_phd
├── references/ # énoncé
└── README.md
```

## Jeux de Données analysés

L’étude s’appuie sur trois ensembles de données principaux :

Âge et genre : analyse de la distribution par tranches d’âge et par sexe, appuyée sur des visualisations statistiques.

Formations engagées (Caisse des Dépôts) : exploration géographique et financière des formations, incluant les taux de complétion et les montants engagés.

Thèses de doctorat (1985–2020) : étude des données manquantes, de la distribution temporelle des soutenances, des directeurs de thèse et de l’évolution des langues de rédaction.


## Quelques résultats 

Les visualisations produites comprennent des heatmaps des données manquantes, la distribution mensuelle des soutenances, l’évolution des langues de rédaction ainsi qu’une analyse des valeurs extrêmes liées aux directeurs de thèse.
Les analyses ont permis d’identifier des patterns temporels, de détecter des homonymes (notamment le cas « Cécile Martin ») et de comparer les taux de réalisation par région. Il y a d'avantage d'informations dans le rapport.


## Ressources

- **[Rapport](./Rapport_phd.pdf)**
- **[Énoncé du projet](./references/enonce_projet.pdf)**


## Auteur

[@naima-beck](https://www.github.com/naima-beck) - Cy Tech - Sciences-Po Saint-Germain-En-Laye - [2024/2025]


## License

Ce projet est réalisé dans un cadre académique. Les données sont fournies pour usage pédagogique.
Il est sous licence [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
![License](https://img.shields.io/badge/License-CC%20BY--NC--SA-blue.svg)
