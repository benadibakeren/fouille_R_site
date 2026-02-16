---
title: Mini-projet 3
---

# Mini-projet 3 : Classification de theses francaises

[Ouvrir le mini-projet 3 (HTML)](./projet3.html)

## Objectifs

- Classer des résumés de thèses par domaine.
- Combiner réduction de dimension et classification.
- Evaluer les performances par validation croisée.

## Dataset

- **French thesis metadata** (Kaggle).

## Problématique 

Peut-on classer automatiquement des résumés scientifiques selon leur domaine (informatique, mathématiques, physique, biologie, sciences humaines…) uniquement à partir du texte ?

Les enjeux sont :

- La richesse et la complexité du vocabulaire académique
- La proximité lexicale entre certains domaines
- Le déséquilibre possible des classes


## Methodologie

- Nettoyage du texte et suppression des stopwords.
- Vectorisation **TF-IDF**.
- Réduction de dimension via **AFD**.
- Classification bayésienne naif.
- Evaluation (validation croisée, mesures de performance).


## Résultats

Les résultats montrent que :

- Les domaines très distincts sont bien classifiés
- Les disciplines proches peuvent être confondues
- La performance dépend fortement de la richesse lexicale

L’utilisation du TF-IDF améliore significativement la capacité de discrimination.

## Difficultés rencontrées

- Déséquilibre potentiel entre classes
- Similarité du vocabulaire scientifique
- Importance du choix des paramètres (seuils, taille vocabulaire)

## Conclusion 

Ce troisième projet démontre que la classification automatique de documents scientifiques est possible et pertinente.

Il confirme :

- L’importance du feature engineering
- L’impact du choix des représentations textuelles
- La complémentarité entre statistiques et NLP

## Livrables

- `projet3.rmd`
- `projet3.html`
