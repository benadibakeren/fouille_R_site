---
title: Projet final
---

# Projet final : Détection de texte généré par IA

## Objectifs

- Distinguer un texte humain d'un texte généré par IA.
- Combiner AFD et classification bayésienne.
- Traiter un dataset NLP de grande taille.

## Description

Le projet final s'appuie sur la compétition Kaggle **LLM - Detect AI Generated
Text**. Le point de départ est le dossier `llm-detect-ai-generated-text`.

Pour améliorer la qualité d'apprentissage, un dataset supplémentaire est ajouté
(`train_drcat_01.csv` a `train_drcat_04.csv`), issu de **DAIGT_Proper_Train_Dataset**.

## Problématique

Dans un monde où l'IA est partout, on peut se demander :
- Est-il réellement possible de distinguer des textes rédigés par l'IA des textes rédigés par un humain ?

## Méthodologie

-  **Chargement** des jeux de données (`train_essays.csv`, `train_prompts.csv`).
- **Nettoyage** et normalisation du texte.
- **Vectorisation** (TF-IDF) et sélection de caractéristiques.
- **AFD** pour separer les groupes humain vs IA.
- **Classification bayésienne** sur les axes/distributions issus de l'AFD.

## Résultats

Les analyses mettent en évidence :

- Une structure claire entre certains groupes
- Des variables fortement discriminantes
- Une performance satisfaisante du modèle de classification

La visualisation des axes factoriels permet une interprétation intuitive des résultats.

## Conclusion 

Ce projet final met en évidence qu’il est possible d’identifier des différences statistiques entre des textes rédigés par des humains et ceux générés par une intelligence artificielle, à condition d’utiliser des méthodes adaptées et un prétraitement rigoureux.

Les analyses multivariées et les méthodes de discrimination permettent de :

- Mettre en évidence des structures lexicales spécifiques
- Identifier des régularités stylistiques
- Construire des modèles capables de distinguer certains textes générés par l’IA

En conclusion, les méthodes statistiques offrent un cadre pertinent pour explorer la détection de textes générés par l’IA, tout en soulignant la nécessité d’une interprétation prudente des résultats et d’une amélioration continue des modèles.

## Livrables

- `projet_final.Rmd` 
- `projet_final.html` 



