##  Comment exécuter le projet
Ce notebook a été conçu pour être facilement reproductible. Voici les étapes pour le relancer :

1. **Prérequis :**
   - Avoir installé [Jupyter Notebook](https://jupyter.org/) ou [JupyterLab](https://jupyterlab.readthedocs.io/).
   - Installer les dépendances nécessaires via le terminal :
     ```bash
     pip install pandas numpy
     ```

2. **Lancement :**
   - Place ton fichier de données (format `.csv`) dans le même répertoire que le notebook.
   - Ouvre un terminal dans le dossier `TP1`.
   - Lance l'interface Jupyter :
     ```bash
     jupyter notebook
     ```
   - Ouvre le fichier `TP1_Data_Cleansing_TP1.ipynb`.
   - Utilise l'option **"Restart & Run All"** dans le menu "Kernel" pour exécuter l'intégralité du pipeline de nettoyage.

3. **Validation :**
   - Vérifie la cellule finale du notebook pour confirmer que le total des valeurs manquantes est bien à `0`.
