---
title: Projet final
---

# Projet final : Detection de texte genere par IA

## Objectifs

- Distinguer un texte humain d'un texte genere par IA.
- Combiner AFD et classification bayesienne.
- Traiter un dataset NLP de grande taille.

## Description

Le projet final s'appuie sur la competition Kaggle **LLM - Detect AI Generated
Text**. Le point de depart est le dossier `llm-detect-ai-generated-text`.

Pour ameliorer la qualite d'apprentissage, un dataset supplementaire est ajoute
(`train_drcat_01.csv` a `train_drcat_04.csv`), issu de **DAIGT_Proper_Train_Dataset**.

Le pipeline suit ces etapes :

1. **Chargement** des jeux de donnees (`train_essays.csv`, `train_prompts.csv`).
2. **Nettoyage** et normalisation du texte.
3. **Vectorisation** (TF-IDF) et selection de caracteristiques.
4. **AFD** pour separer les groupes humain vs IA.
5. **Classification bayesienne** sur les axes/distributions issus de l'AFD.

Le livrable principal est `projet_final.Rmd` (et la version HTML). Il documente
les choix de pretraitement, la selection de variables et l'evaluation des
performances.



