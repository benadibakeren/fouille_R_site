---
title: TD 2
---

# TD 2 : MANOVA

## Objectifs

- Comprendre la logique de la MANOVA et ses liens avec l'ANOVA.
- Implementer le calcul des inerties **totale**, **intra** et **inter**.
- Valider les resultats avec la fonction `manova` de R.

## Description

Ce TD developpe une fonction MANOVA generique. L'idee est d'ecrire toutes les
etapes mathematiques pour comparer des groupes sur plusieurs variables :

- calcul de la **SST** (somme des carres totale),
- calcul de la **SS intra**,
- derivation de la **SS inter**,
- calcul de **Lambda de Wilks** et de la statistique de test.

Le jeu de donnees utilise (**MANOVA_DATASET.csv**) porte sur la composition
chimique de poteries antiques, avec plusieurs variables numeriques et une
variable de groupe.

Le TD se termine par une comparaison avec `manova`, afin de verifier que la
fonction implementee reproduit les resultats attendus.
