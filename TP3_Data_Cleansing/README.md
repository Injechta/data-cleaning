# TP3 - Détection et Traitement des Outliers

**Difficulté:** Intermédiaire  
**Dataset:** sales_outliers.csv  
**Description:** Identification des valeurs aberrantes avec méthodes statistiques

---

## Contexte et Objectifs

Bienvenue sur le TP3 de ce module ! Ce notebook a pour objectif d'aborder les techniques fondamentales de nettoyage et de traitement des données avec Python, en se focalisant particulièrement sur la détection et le traitement des valeurs aberrantes (outliers) à l'aide de méthodes statistiques (IQR et Z-score).

* **Niveau :** Intermédiaire
* **Dataset associé :** `sales_outliers.csv` (situé dans le dossier `../data/`)
* **Objectif du dataset :** Identification, analyse et traitement des valeurs aberrantes sur des données de transactions commerciales.

## Dépendances et Environnement

Ce notebook nécessite l'installation des bibliothèques Python suivantes :
* `pandas` (manipulation et analyse de données)
* `numpy` (calculs numériques)
* `matplotlib` & `seaborn` (visualisation de données)
* `missingno` (visualisation spécifique des valeurs manquantes)
* `scipy` (fonctions statistiques pour le Z-score)

Vous pouvez installer l'ensemble des dépendances nécessaires via la commande suivante :
```bash
pip install pandas numpy matplotlib seaborn missingno scipy
```

## Guide de Démarrage / Comment relancer ce Notebook

Pour exécuter ce notebook dans de bonnes conditions, suivez les étapes ci-dessous :

1. **Prérequis :** Assurez-vous d'avoir un environnement Python (3.8 ou supérieur) et Jupyter Notebook / JupyterLab installés.
2. **Structure des dossiers :** Vérifiez que votre arborescence respecte la structure suivante pour que les chemins relatifs fonctionnent correctement :
   ```text
   mon_projet/
   ├── data/
   │   └── sales_outliers.csv
   └── notebooks/
       └── tp3_detection_outliers.ipynb
   ```
3. **Lancement de Jupyter :** Ouvrez votre terminal dans le dossier du projet et lancez :
   ```bash
   jupyter notebook
   ```
4. **Exécution :** Ouvrez le notebook TP3 et exécutez les cellules de manière séquentielle (de haut en bas) pour charger les bibliothèques, importer le dataset, et afficher les analyses et visualisations.

## Structure du Notebook

1. **Imports des Bibliothèques :** Chargement des outils nécessaires et configuration globale de l'affichage (`pandas`, `seaborn`, `matplotlib`, `missingno`, `scipy`, etc.).
2. **Import du Dataset :** Chargement du fichier `sales_outliers.csv`, vérification de la structure, aperçu des premières lignes et dimensions (1020 lignes × 4 colonnes).
3. **Visualisation des Valeurs Manquantes :** Analyse graphique via `missingno` et tabulaire des données absentes pour préparer le nettoyage.
4. **Questions Préalables :** Série de questions d'analyse exploratoire pour identifier les spécificités du dataset (distribution de `amount`, recherche de valeurs négatives, maximums aberrants, détection d'outliers par IQR et Z-score, impact sur la moyenne, etc.).

## Notes & Bonnes Pratiques

* Pensez à bien vérifier l'emplacement de votre fichier de données par rapport au chemin relatif (`../data/sales_outliers.csv`) si vous déplacez le notebook.
* Ce TP complète les bases de la qualité des données en s'attaquant à la détection rigoureuse des anomalies statistiques.
