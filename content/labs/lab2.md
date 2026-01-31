---
title: Lab 2
---

# Lab 2: 

## Objectifs

- Comprendre le principe d’Infrastructure as Code (IaC) et ses avantages par rapport à une         gestion manuelle de l’infrastructure.
- Authentifier de manière sécurisée des outils DevOps pour interagir avec les services AWS.
- Automatiser le déploiement d’une instance EC2 à l’aide d’un script Bash.
- Déployer et configurer une instance distante en utilisant Ansible et des playbooks.
- Créer une image serveur (AMI) contenant une application préconfigurée à l’aide de Packer.
- Décrire, déployer, mettre à jour et supprimer une infrastructure cloud de manière déclarative    avec OpenTofu.
- Utiliser des modules OpenTofu afin de factoriser le code et faciliter la réutilisation de        l’infrastructure.

## Description

Ce second lab permet de découvrir le principe d'**Infrastructure as Code** (IaC). 
Cette infrastructure consiste à déployer et gérer une infrastructure informatique grâce à des scripts plutôt que par des actions manuelles. Elle repose sur AWS EC2 et une application web en **Node.js**. 

Dans un premier temps, on met en place des clés d'accès IAM pour permettre d'intéragir avec AWS de manière sécurisée. On déploie ensuite l'infrastructure à l'aide d'un script Bash, ce qui va permettre d'automatiser la création d'instance EC2, la configuration du réseau et le lancement de l'application. 

Par la suite, ce lab introduit **Ansible** qui va permettre d'automatiser la configuration des serveurs. Les ressources sont créées **et** configurées via des playbooks. 
On introduit ensuite **Packer**, qui va créée **AMI**. Il s'agit d'un serveur qui va en une seule fois lancer une **instance EC2** temporaire, y installer Node.js et l'application, garder en mémoire le serveur et le transformer en **AMI**. Cela permet de rendre le serveur opérationnel dès sont démarrage.

Enfin, on utilise **OpenTofu** pour définir l'infrastructure cloud à l'aide de fichiers **.tf**. Ces fichiers vont décrire les instances EC2, les rècles réseau ou encore les paramètres de démarrage attendus. **OpenTofu** se charge ensuite de créer, mettre à jour ou supprimer les ressources nécessaires afin que l’infrastructure corresponde à ce que l'on souhaite. Pour cela, on utilise les commandes suivantes : 
- tofu init (prépare le projet)
- tofu apply (crée les ressources si elles n’existent pas oules modifie si elles ont changé)
- tofu destroy (supprime toute l'infrastructure)
