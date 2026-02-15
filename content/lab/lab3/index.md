---
title: TD 3
---

# TD 3 : AFD (Analyse factorielle discriminante)

[Ouvrir le TD 3 (HTML)](./III_AFD.html)

## Objectifs

- Reducer la dimensionnalite avec l'AFD.
- Evaluer la discrimination entre classes.
- Visualiser les individus sur les axes factoriels.

## Description

Ce TD construit l'AFD a partir des elements calcules en MANOVA. L'idee est de :

- calculer les axes factoriels qui maximisent la separation inter-groupes,
- projeter les individus dans le plan factoriel,
- tester la qualite de la discrimination (tests de Wilks).

Le jeu de donnees utilise est **VIN_QUALITE.txt**. Le TD produit :

- les scores (coordonnees sur les axes),
- un graphique de projection des groupes,
- des indicateurs statistiques pour valider la separation.