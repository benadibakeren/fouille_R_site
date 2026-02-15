---
title: TD 4
---

# TD 4 : AFD et classification supervisee

[Ouvrir le TD 4 (HTML)](./IV_AFD.html)

## Objectifs

- Utiliser les scores AFD pour classifier.
- Mesurer la qualite d'une classification (matrice de confusion).
- Mettre en pratique la logique distance-centre de groupe.

## Description

Ce TD reprend les resultats de l'AFD (TD3) et passe a la **classification**.
L'idee est de projeter les individus sur les axes factoriels, puis :

- calculer le **centre** de chaque groupe,
- mesurer les **distances** aux centres,
- affecter chaque individu a la classe la plus proche,
- evaluer la performance via une matrice de confusion.

Le jeu de donnees reste **VIN_QUALITE.txt**. Le TD permet de relier analyse
factorielle, visualisation et classification supervisee.
