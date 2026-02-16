---
title: TD 1
---

# TD 1 : Classifieur bayesien naif

[Ouvrir le TD 1 (HTML)](./I_BAYESIEN.html)

## Objectifs

- Comprendre la logique d'un classifieur bayesien naif.
- Implémenter les étapes principales en R.
- Comparer les résultats avec une fonction R existante.

## Description

Ce TD a pour but d'appliquer un classifieur bayésien naif **pas a pas**. Le but est de décomposer la règle de Bayes et de comprendre comment sont calculées :

- la **vraisemblance** (probabilites conditionnelles),
- les **probabilités à postériori**,
- la décision finale par **maximisation**.

Le travail se fait d'abord sur un **jeu de données simple** (exemple du cours), puis sur un jeu plus grand pour verifier sa robustesse. Le TD insiste sur :

- le rôle de l'hypothèse d'indépendance,
- la construction des tables de probabilités,
- la comparaison des performances via une matrice de confusion.


## Méthodologie

- Nettoyage et préparation des données
- Séparation train / test
- Estimation des probabilités a priori
- Estimation des vraisemblances
- Prédiction sur l’échantillon test
- Analyse des performances (accuracy, matrice de confusion)

## Résultats

Le modèle bayésien permet :
- Une classification rapide
- Une interprétation claire
- Une base solide pour comparaison avec d'autres méthodes

Cependant, l’hypothèse d’indépendance peut limiter les performances lorsque les variables sont fortement corrélées.


## Conclusion

Le classificateur bayésien constitue une méthode simple et efficace, particulièrement adaptée aux jeux de données de taille modérée et aux problématiques textuelles ou catégorielles.