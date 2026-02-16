---
title: TD 4
---

# TD 4 : AFD et classification supervisee

[Ouvrir le TD 4 (HTML)](./IV_AFD.html)

## Objectifs

Cette partie applique l’AFD dans un cadre plus opérationnel :

- Interprétation des axes
- Analyse des contributions des variables
- Évaluation des performances de classification

## Description

Ce TD reprend les résultats de l'AFD (TD3) et passe à la **classification**.
L'idée est de projeter les individus sur les axes factoriels, puis :

- Calculer le **centre** de chaque groupe,
- Mesurer les **distances** aux centres,
- Affecter chaque individu à la classe la plus proche,
- Evaluer la performance via une matrice de confusion.

Le jeu de données reste **VIN_QUALITE.txt**. 

## Résultats

Les axes discriminants mettent en évidence :

- Les variables les plus structurantes
- Les groupes les plus proches
- Les éventuels recouvrements entre classes

