---
title: TD 3
---

# TD 3 : AFD (Analyse factorielle discriminante)

[Ouvrir le TD 3 (HTML)](./III_AFD.html)

## Objectifs

- Réduire la dimensionnalite avec l'AFD.
- Evaluer la discrimination entre classes.
- Visualiser les individus sur les axes factoriels.

## Description

Ce TD construit l'AFD à partir des éléments calculés en MANOVA. L'idée est de :

- maximiser la variance inter-classes
- minimiser la variance intra-classe

Elle repose sur la décomposition des matrices : 

- Matrice de variance intra-groupes
- Matrice de variance inter-groupes

Le jeu de données utilisé est **VIN_QUALITE.txt**. 

## Méthodologie

- Calcul des centres de gravité des classes
- Construction des matrices de dispersion
- Résolution du problème aux valeurs propres
- Projection des individus sur les axes discriminants


## Résultats

L'AFD permet :
- Une visualisation claire des groupes
- Une meilleure compréhension des variables discriminantes
- Une base pour la classification supervisée

## Conclusion 

L’AFD est particulièrement adaptée aux problèmes de classification lorsque l’objectif est à la fois explicatif et prédictif.