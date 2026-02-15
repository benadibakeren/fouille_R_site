---
title: TD 1
---

# TD 1 : Classifieur bayesien naif

## Objectifs

- Comprendre la logique d'un classifieur bayesien naif.
- Implementer les etapes principales en R.
- Comparer les resultats avec une fonction R existante.

## Description

Ce TD construit un classifieur bayesien naif **pas a pas**. Le but est de
decomposer la regle de Bayes et de comprendre comment sont calculees :

- la **vraisemblance** (probabilites conditionnelles),
- les **probabilites a posteriori**,
- la decision finale par **maximisation**.

Le travail se fait d'abord sur un **jeu de donnees simple** (exemple du cours),
puis sur un jeu plus grand pour verifier la robustesse. Le TD insiste sur :

- le role de l'hypothese d'independance,
- la construction des tables de probabilites,
- la comparaison des performances via une matrice de confusion.
