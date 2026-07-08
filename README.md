# Sell4All — Data Exploration Project

## 1. Présentation rapide du besoin

Sell4All est une entreprise de vente au détail de vêtements d'occasion en ligne.
Ce projet consiste à réaliser une première exploration et un nettoyage des données
clients (`dataset-sell4all.csv`), afin de préparer leur utilisation future dans un
projet d'intelligence artificielle (recommandation automatique de produits).

## 2. Étapes suivies pendant les 3 jours


- **Jour 1** :
  - Installation de l'environnement (Python via Miniconda, Jupyter, pandas, matplotlib)
  - Lecture du fichier CSV et affichage des 5 premières lignes
  - Affichage et explication du résumé technique des données
- **Jour 2** :
  - Calcul de la médiane et moyenne (Age, Customer spendings)
  - Question bonus : médiane d'âge par pays
  - Visualisation des dépenses par pays (graphique à barres)
    - Choix : Affichage de deux graphiques à barres distincts : un pour la moyenne, un pour la somme des dépenses par pays.
  - Nettoyage des lignes < 10€ de dépenses
  - Suppression des doublons
  - Export du CSV nettoyé avec les colonnes Country, Âge, Gender, Customer spendings
  - Rédaction du README 

## 3. Fonctionnalités développées / éléments finalisés

- [ ] Lecture du CSV avec pandas
- [ ] Affichage des 5 premières lignes (`head()`)
- [ ] Résumé technique des données (`info()`) + explication en cellule markdown
- [ ] Médiane / moyenne de "Age" et "Customer spendings"
- [ ] Bonus : médiane d'âge par pays (`groupby`)
- [ ] Graphique à barres : dépenses par pays
- [ ] Suppression des lignes < 10€ de dépenses
- [ ] Suppression des doublons
- [ ] Export du CSV nettoyé (colonnes : Country, Âge, Gender, Customer spendings)

## 4. Difficultés rencontrées et solutions mises en place

- Difficulté : première utilisation de Python, Jupyter Notebook et de l'environnement Miniconda — habitué à coder dans un éditeur de code classique avec exécution linéaire d'un fichier avec terminal linux, pas avec des cellules indépendantes.
  Solution : recherche de tutoriels sur le fonctionnement des cellules Jupyter (ordre d'exécution, kernel, état partagé entre cellules) ; plusieurs erreurs "variable non définie" corrigées en comprenant que les cellules doivent être exécutées dans le bon ordre (utilisation de "Restart & Run All" pour vérifier la cohérence du notebook).
- Difficulté : découverte des fonctions pandas spécifiques (head, info, groupby, agg, drop_duplicates, etc.).
  Solution : consultation de la documentation pandas et des ressources fournies dans le brief pour comprendre le rôle de chaque méthode avant de l'utiliser.

## 5. Mode d'exécution du projet

### Prérequis
- Python via Miniconda installé
- Git

### Installation

1. Cloner le dépôt :
   `git clone git@github.com:Saad05-dev/sell4all-data-management.git`
2. Se placer dans le dossier du projet
  `cd sell4all-data-management`
3. Créer et activer l'environnement virtuel :
   `conda create -n sell4all-data-management python=3.11 -y`
   `conda activate sell4all-data-management`
4. Installer les dépendances :
   `conda install pandas matplotlib jupyter notebook`


### Lancer le projet

1. Démarrer Jupyter Notebook :
   `jupyter notebook`
2. Ouvrir le fichier `exploration.ipynb`
3. Exécuter les cellules dans l'ordre

## 6. Structure du dépôt

```
├── exploration.ipynb
├── dataset-sell4all.csv
├── dataset-sell4all-clean.csv
├── README.md
└── .gitignore
```