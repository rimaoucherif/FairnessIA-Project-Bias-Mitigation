# FairnessIA — Analyse et Mitigation des Biais sur un Dataset Médical

## Présentation du projet

Ce projet a pour objectif d’analyser les biais potentiels présents dans un jeu de données de radiographies thoraciques avant toute utilisation prédictive.

L’objectif principal est d’identifier les déséquilibres structurels du dataset et d’explorer des méthodes de mitigation au niveau du pré-traitement.

L’analyse porte sur trois dimensions principales :

- Le déséquilibre lié au **genre** (attribut sensible)
- La distribution des **tranches d’âge**
- L’hétérogénéité des **pathologies médicales** (Finding Labels)

---

## Méthodologie

### Analyse descriptive des biais

- Étude de la distribution du genre
- Analyse de la répartition des tranches d’âge
- Analyse de la fréquence des différentes pathologies

### Méthodes de mitigation (pré-processing)

Deux approches ont été explorées :

- **Ré-pondération (Reweighting)**  
  Pondération inversement proportionnelle à la fréquence des groupes afin d’équilibrer leur influence statistique sans modifier le dataset.

- **Rééchantillonnage **  
  Under-sampling du groupe majoritaire pour obtenir un jeu de données équilibré en effectif.

---

## Technologies utilisées

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

---

## Conclusion du projet

Ce travail met en évidence l’importance d’examiner attentivement la structure d’un jeu de données avant toute modélisation, en particulier dans un contexte médical où les biais peuvent influencer l’interprétation et l’équité des analyses.
