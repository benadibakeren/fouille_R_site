---
title: Mini-projet 1
---

# Mini-projet 1 : Classification bayesienne des emotions

[Ouvrir le mini-projet 1 (HTML)](./project1_code.html)

## Objectifs

- Predire l'émotion d'une phrase en langage naturel.
- Tester un classifieur bayésien naif sur des textes courts.
- Comparer l'effet du prétraitement sur la performance.

## Dataset

- **Emotion Classify Data** (Kaggle).

## Problématique

Peut-on déterminer automatiquement si un texte exprime :

- Joie
- Colère
- Tristesse
- Peur
- Amour
- Surprise

en utilisant uniquement du texte ?


## Méthodologie

- Nettoyage du texte (minuscule, ponctuation, chiffres, stopwords).
- Tokenization et stemming/lemmatisation.
- Vectorisation **TF-IDF** avec **bi-grammes**.
- Entrainement d'un **classifieur bayesien naif**.
- Evaluation par distribution des classes et performance globale.

## Résultats

Le modèle permet :
- Une classification rapide
- Une interprétation claire
- Une base solide pour comparer avec d'autres méthodes

Cependant, certaines émotions proches sont parfois confondues (ex : tristesse / peur).

## Conclusion 

Ce premier projet montre l’efficacité du modèle bayésien en traitement automatique du langage.

Il constitue une base solide pour améliorer les performances dans les projets suivants.

## Livrables

- `project1_code.Rmd`
- `project1_code.html`
