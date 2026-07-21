# TP4 : Validation et Cohérence des Données

**Difficulté :** Intermédiaire  
**Dataset :** `healthcare_inconsistent.csv`  
**Objectif :** Maîtriser la validation des contraintes logiques, la détection d'anomalies inter-colonnes et le nettoyage de données de santé incohérentes.

---

##  Contexte du Projet

Dans le cadre de la gestion et de l'analyse de données médicales, la simple détection de valeurs manquantes ne suffit pas. Il est crucial de valider la **cohérence logique** et les **contraintes métiers** entre les différentes variables d'un même enregistrement (par exemple, s'assurer qu'une date de fin de séjour est postérieure à la date de début, ou qu'une fréquence cardiaque se situe dans des plages physiologiques plausibles).

Ce TP vous guide à travers une démarche structurée de validation et de nettoyage sur un dataset intentionnellement corrompu.

---

##  Structure du TP

Le travail est implémenté dans le notebook Jupyter `TP4_Validation_Coherence_Donnees.ipynb` et s'articule autour des étapes suivantes :

1. **Imports et Configuration :** Chargement des bibliothèques (`pandas`, `numpy`, `matplotlib`, `seaborn`) et configuration des options d'affichage.
2. **Exploration Initiale :** Chargement du fichier `healthcare_inconsistent.csv`, analyse des dimensions, typage et empreinte mémoire.
3. **Analyse des Valeurs Manquantes et Doublons :** Inspection structurelle initiale du dataset.
4. **Validation des Contraintes Logiques et Inter-colonnes :**
   - **Âge :** Vérification de la plage valide (`0 <= age <= 120`).
   - **Cohérence Temporelle :** Validation que la date de début de séjour (`start_date`) est antérieure ou égale à la date de fin (`end_date`).
   - **Contraintes Financières :** Vérification que le prix (`price`) est strictement positif (`> 0`).
   - **Bornes Physiologiques :** Contrôle de la fréquence cardiaque (`heart_rate` entre 40 et 180 bpm).
   - **Formats de Contact :** Validation syntaxique des adresses e-mail via des expressions régulières (`regex`).
5. **Visualisation des Anomalies :** Utilisation de boîtes à moustaches (`boxplots`) pour identifier visuellement les valeurs aberrantes.
6. **Nettoyage et Filtrage :** Application des règles métiers pour purifier le dataset.
7. **Export :** Sauvegarde des données nettoyées vers `../data/healthcare_cleaned.csv`.

---

##  Utilisation

Pour lancer et exécuter ce TP :

```bash
# Activer votre environnement virtuel si nécessaire
jupyter notebook TP4_Validation_Coherence_Donnees.ipynb
```

Assurez-vous que le dossier `../data/` contient bien le fichier source `healthcare_inconsistent.csv`.
