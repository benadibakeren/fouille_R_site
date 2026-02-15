---
title: Mini-projet 1
---

# Mini-projet 1 : Classification bayesienne des emotions

## Objectifs

- Predire l'emotion d'une phrase en langage naturel.
- Tester un classifieur bayesien naif sur des textes courts.
- Comparer l'effet du pretraitement sur la performance.

## Dataset

- **Emotion Classify Data** (Kaggle).

## Methode

- Nettoyage du texte (minuscule, ponctuation, chiffres, stopwords).
- Tokenization et stemming/lemmatisation.
- Vectorisation **TF-IDF** avec **bi-grammes**.
- Entrainement d'un **classifieur bayesien naif**.
- Evaluation par distribution des classes et performance globale.

## Livrables

- `project1_code.Rmd`
- `project1_code.html`
