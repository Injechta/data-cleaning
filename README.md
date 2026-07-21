# data-cleaning

À partir de 4 jeux de données aux problématiques différentes, vous devez produire des notebooks de nettoyage propres, documentés et réutilisables, en justifiant chaque choix de traitement.

## Contexte du projet

Un data scientist nettoie des données pour explorer et modéliser. Un data ingénieur nettoie pour construire des pipelines fiables qui tournent en production, souvent sans supervision humaine.

La différence est fondamentale : une erreur de nettoyage non détectée dans un pipeline automatisé peut corrompre silencieusement toutes les données en aval pendant des jours ou des semaines avant d'être repérée.

---

##  Structure des Travaux Pratiques (TPs)

Le dépôt est organisé de manière progressive, allant du nettoyage de base jusqu'à la validation avancée des contraintes inter-colonnes :

| Dossier | Thématique & Description | README associé |
| :--- | :--- | :--- |
| [`TP1_Data_Cleansing`](./TP1_Data_Cleansing/) | **TP1 :** Exploration initiale, gestion des valeurs manquantes et doublons basiques. | [📘 Voir le README](./TP1_Data_Cleansing/README.md) |
| [`TP2_Data_Cleansing`](./TP2_Data_Cleansing/) | **TP2 :** Standardisation des formats, typage et traitement des valeurs aberrantes univariées. | [📘 Voir le README](./TP2_Data_Cleansing/README.md) |
| [`TP3_Data_Cleansing`](./TP3_Data_Cleansing/) | **TP3 :** Gestion avancée des imputations et réconciliation de données textuelles/catégorielles. | [📘 Voir le README](./TP3_Data_Cleansing/README.md) |
| [`TP4_Data_Cleansing`](./TP4_Data_Cleansing/) | **TP4 :** Validation et cohérence des données, contraintes inter-colonnes et règles métiers (santé). | [📘 Voir le README](./TP4_Data_Cleansing/README.md) |

*(Bonus optionnel : TP5 à TP9 disponibles pour approfondissement).*

---

##  Instructions d'Installation et Exécution

1. **Cloner le dépôt :**
   ```bash
   git clone https://github.com/Injechta/data-cleaning.git
   cd data-cleaning
   ```

2. **Créer et activer un environnement virtuel :**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Sur Windows : venv\Scripts\activate
   ```

3. **Installer les dépendances nécessaires :**
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

4. **Lancer Jupyter Notebook :**
   ```bash
   jupyter notebook
   ```
   Naviguez ensuite dans les sous-dossiers pour exécuter les notebooks de chaque TP de bout en bout.

---

## Modalités pédagogiques
Travail individuel en autonomie. Approche progressive : un dataset par problématique, du plus simple au plus complexe.

## Modalités d'évaluation
Soutenance orale de 20 minutes où l'apprenant présente ses notebooks et justifie chaque choix de traitement. Les notebooks doivent s'exécuter sans erreur de bout en bout.

## Critères de performance
* Les 4 notebooks s'exécutent sans erreur de bout en bout.
* Chaque transformation est documentée avec statistiques avant/après dans des cellules Markdown.
* Les choix de traitement sont justifiés.
* Le code est lisible, sans duplication, organisé en sections logiques.
