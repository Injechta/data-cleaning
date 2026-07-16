# TP1 : Data Cleansing & Pipeline de Nettoyage

Ce dossier contient le premier travail pratique portant sur le nettoyage et la préparation de données (*Data Cleansing*). L'objectif est de transformer un dataset brut en un jeu de données sain et exploitable pour des analyses ultérieures.

##  Objectifs du TP
*   **Analyse exploratoire :** Identifier la structure et les lacunes des données brutes (`df_brut`).
*   **Pipeline de nettoyage :** Mettre en place des stratégies de traitement des valeurs manquantes.
*   **Traçabilité :** Documenter chaque transformation pour garantir la reproductibilité du processus.

##  Compétences démontrées
*   **Manipulation de données :** Utilisation de la bibliothèque `pandas` pour le traitement de datasets.
*   **Stratégies d'imputation :** Application de techniques robustes (médiane pour les données numériques, mode pour les données catégorielles).
*   **DevOps Mindset :** Automatisation du reporting des transformations effectuées et validation de l'intégrité finale des données.

##  Contenu du dossier
*   `TP1_Data_Cleansing_TP1.ipynb` : Notebook Jupyter contenant l'intégralité du code, les analyses et le rapport de synthèse.

##  Résumé des transformations
| Action | Cible | Méthode |
| :--- | :--- | :--- |
| Suppression | Colonnes > 70% vides | Seuil `thresh` |
| Imputation | `price` | Médiane |
| Imputation | `shipping_address` | Mode |
