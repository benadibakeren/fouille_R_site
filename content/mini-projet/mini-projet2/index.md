---
title: Mini-projet 2
---

# Mini-projet 2 : AFD sur tweets (sentiment)

[Ouvrir le mini-projet 2 (HTML)](./projet2.html)

## Objectifs

- Transformer des tweets en variables numériques exploitables.
- Appliquer l'Analyse Factorielle Discriminante (AFD).
- Evaluer la séparation des classes de sentiment.

## Dataset

- **Twitter Entity Sentiment Analysis** (Kaggle).

## Problématique

L’AFD permet-elle de bien séparer des tweets selon leur polarité émotionnelle ?

Nous explorons plusieurs pistes :

- Gestion intelligente des stopwords
- Conservation des négations
- Utilisation de bigrammes
- Pondération TF-IDF

## Methodologie

- Nettoyage et normalisation du texte.
- Vectorisation **TF-IDF**.
- Ajout d'un score de sentiment.
- AFD via **LDA** (package `MASS`).
- Visualisation des classes et mesure de la precision.

## Résultats 

Les résultats montrent que :

- L’AFD parvient à séparer partiellement les sentiments
- Les tweets fortement polarisés (très positifs ou très négatifs) sont mieux discriminés
- Les tweets neutres peuvent parfois se situer entre les deux groupes

La visualisation permet une meilleure compréhension que le modèle bayésien seul.


## Conclusion

Ce projet montre que les méthodes statistiques traditionnelles restent pertinentes en Data Science, à condition d’adapter correctement les données.

## Livrables

- `projet2.Rmd`
- `projet2.html`
