# TP2 - Doublons et Standardisation

## Contexte et Objectifs

Bienvenue sur le TP2 de ce module ! Ce notebook a pour objectif d'aborder les techniques fondamentales de nettoyage de données avec Python, en se focalisant particulièrement sur la détection et la suppression des doublons, ainsi que sur la standardisation des formats de données.
* **Niveau :** Débutant
* **Dataset associé :** `customers_duplicates.csv` (situé dans le dossier `../data/`)
* **Objectif du dataset :** Nettoyage et uniformisation de données client comportant des doublons stricts/partiels et des incohérences de format.

## Dépendances et Environnement

Ce notebook nécessite l'installation des bibliothèques Python suivantes :
* `pandas` (manipulation et analyse de données)
* `numpy` (calculs numériques)
* `matplotlib` & `seaborn` (visualisation de données)
* `missingno` (visualisation spécifique des valeurs manquantes)

Vous pouvez installer l'ensemble des dépendances nécessaires via la commande suivante :
```bash
pip install pandas numpy matplotlib seaborn missingno
```

## Guide de Démarrage / Comment relancer ce Notebook

Pour exécuter ce notebook dans de bonnes conditions, suivez les étapes ci-dessous :
1. **Prérequis :** Assurez-vous d'avoir un environnement Python (3.8 ou supérieur) et Jupyter Notebook / JupyterLab installés.
2. **Structure des dossiers :** Vérifiez que votre arborescence respecte la structure suivante pour que les chemins relatifs fonctionnent correctement :
   ```text
   mon_projet/
   ├── data/
   │   └── customers_duplicates.csv
   └── notebooks/
       └── tp2_doublons_standardisation.ipynb
   ```
3. **Lancement de Jupyter :** Ouvrez votre terminal dans le dossier du projet et lancez :
   ```bash
   jupyter notebook
   ```
4. **Exécution :** Ouvrez le notebook TP2 et exécutez les cellules de manière séquentielle (de haut en bas) pour charger les bibliothèques, importer le dataset, et afficher les analyses et visualisations.

## Structure du Notebook

1. **Imports des Bibliothèques :** Chargement des outils nécessaires et configuration globale de l'affichage (`pandas`, `seaborn`, `matplotlib`, `missingno`, etc.).
2. **Import du Dataset :** Chargement du fichier `customers_duplicates.csv`, vérification de la structure et aperçu des premières lignes.
3. **Visualisation des Valeurs Manquantes :** Analyse graphique via `missingno` et tabulaire des données absentes pour préparer le nettoyage.
4. **Questions Préalables :** Série de questions d'analyse exploratoire pour identifier les spécificités du dataset (doublons, formats de texte, variations de catégories).

## Notes & Bonnes Pratiques

* Pensez à bien vérifier l'emplacement de votre fichier de données par rapport au chemin relatif (`../data/customers_duplicates.csv`) si vous déplacez le notebook.
* Ce TP complète les bases de la découverte de données en s'attaquant à la qualité des données textuelles et à l'unicité des enregistrements.
