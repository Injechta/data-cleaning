# TP1 - Découverte et Valeurs Manquantes Simples

##  Contexte et Objectifs
Bienvenue sur le  TP1 de ce module ! Ce notebook a pour objectif d'introduire les bases du traitement et du nettoyage de données avec Python, en se focalisant particulièrement sur **la détection et la gestion basique des valeurs manquantes**.

- **Niveau :** Débutant [cite: 2]
- **Dataset associé :** `ecommerce_simple.csv` (situé dans le dossier `../data/`) [cite: 2]
- **Volume du dataset :** 500 lignes, 8 colonnes [cite: 2]

---

##  Dépendances et Environnement
Ce notebook nécessite l'installation des bibliothèques Python suivantes :
- `pandas` (manipulation et analyse de données) [cite: 2]
- `numpy` (calculs numériques) [cite: 2]
- `matplotlib` & `seaborn` (visualisation de données) [cite: 2]
- `missingno` (visualisation spécifique des valeurs manquantes) [cite: 2]

Vous pouvez installer l'ensemble des dépendances nécessaires via la commande suivante :
```bash
pip install pandas numpy matplotlib seaborn missingno
```

---

##  Guide de Démarrage / Comment relancer ce Notebook

Pour exécuter ce notebook dans de bonnes conditions, suivez les étapes ci-dessous :

1. **Prérequis :** Assurez-vous d'avoir un environnement Python (3.8 ou supérieur) et Jupyter Notebook / JupyterLab installés.
2. **Structure des dossiers :** Vérifiez que votre arborescence respecte la structure suivante pour que les chemins relatifs fonctionnent correctement :
   ```text
   mon_projet/
   ├── data/
   │   └── ecommerce_simple.csv
   └── notebooks/
       └── tp1_decouverte.ipynb
   ```
3. **Lancement de Jupyter :**
   Ouvrez votre terminal dans le dossier du projet et lancez :
   ```bash
   jupyter notebook
   ```
4. **Exécution :** Ouvrez le notebook `TP1` et exécutez les cellules de manière séquentielle (de haut en bas) pour charger les bibliothèques, importer le dataset, et afficher les analyses statistiques et graphiques.

---

##  Structure du Notebook

1. **Imports des Bibliothèques :** Chargement des outils nécessaires et configuration globale de l'affichage (pandas, seaborn, matplotlib, etc.).
2. **Import du Dataset :** Chargement du fichier `ecommerce_simple.csv`, vérification de la structure (`df.shape`, types de données, mémoire utilisée) et aperçu des premières lignes.
3. **Visualisation des Valeurs Manquantes :** Analyse graphique et tabulaire des données absentes pour identifier les colonnes à nettoyer (notamment `price` et `shipping_address`).

---

##  Notes & Bonnes Pratiques
* Pensez à bien vérifier l'emplacement de votre fichier de données par rapport au chemin relatif (`../data/ecommerce_simple.csv`) si vous déplacez le notebook.
* Ce TP pose les bases indispensables pour aborder les techniques d'imputation et de nettoyage avancées des TPs suivants.
