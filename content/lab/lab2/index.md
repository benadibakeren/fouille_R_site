---
title: TD 2
---

# TD 2 : MANOVA

[Ouvrir le TD 2 (HTML)](./II_MANOVA.html)

## Objectifs

- Comprendre la logique de la MANOVA et ses liens avec l'ANOVA.
- Implémenter le calcul des inerties **totale**, **intra** et **inter**.
- Valider les résultats avec la fonction `manova` de R.

## Description

Ce TD développe une fonction MANOVA générique. L'idée est d'écrire toutes les
étapes mathématiques pour comparer des groupes sur plusieurs variables :

- calcul de la **SST** (somme des carrés totale),
- calcul de la **SS intra**,
- dérivation de la **SS inter**,
- calcul de **Lambda de Wilks** et de la statistique de test.

Le jeu de données utilise (**MANOVA_DATASET.csv**) porte sur la composition
chimique de poteries antiques, avec plusieurs variables numeriques et une
variable de groupe.

Le TD se termine par une comparaison avec `manova`, afin de vérifier que la
fonction implémentée reproduit les résultats attendus.


## Principe théorique de MANOVA

La MANOVA teste l’égalité des vecteurs de moyennes entre groupes en utilisant des statistiques comme :

- Wilks’ Lambda
- Pillai’s Trace
- Hotelling-Lawley

Elle repose sur l’analyse des matrices de variance-covariance.


## Méthodologie

- Vérification des hypothèses (normalité  multivariée, homogénéité des matrices de covariance)
- Construction du modèle MANOVA
- Analyse des statistiques de test
- Interprétation des p-values

## Résultats 

La MANOVA permet :

- De détecter un effet global du facteur explicatif
- D’éviter la multiplication des tests séparés
- De mieux comprendre les interactions multivariées

## Conclusion 

La MANOVA est pertinente lorsque plusieurs variables dépendantes sont liées entre elles.
Elle fournit une vision globale plus cohérente que des ANOVA indépendantes.