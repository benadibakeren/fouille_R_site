---
title: Lab 1
---

# Lab 1: 

## Description 

Ce lab est une première immersion dans le monde du DevOps. Il introduit le passage d'un programme exécuté localement puis via une application accessible sur internet grâce à un serveur. 
L'application utilisée est une application web développée en **Node.js**, qui a pour rôle d'afficher le message suivant : "Hello World".

Dans un premier temps, notre programme affiche le messaga attendu lorsque nous accédons à l'application via un navigateur. Pour cela, plusieurs actions sont réalisées.
Premièrement, nous allons créer l'arborescence du projet. Dans notre dossier **sample-app**, on crée notre fichier **app.js**. Cette application repose sur le module **http** de Node.js, qui permet de créer un serveur web capable de traiter des requêtes HTTP. 
À chaque requête reçue, le serveur renvoie une réponse avec un code HTTP 200 et le message 
« Hello World ».
Le serveur écoute sur le port par défaut "8080", ou un port défini grâce à la variable PORT.
Cela permet à l’application de s'adapter à différents environnements de déploiement.
Une fois déployé avec la commande **node app.js**, on peut ouvrir **http://localhost:8080** dans notre navigateur et voir le message **"Hello, World!"**.

Dans un second temps, on va déployer l'application sur un server. Pour cela, on va utiliser deux méthodes, la première sera d'utiliser la plateforme PaaS et la seconde d'utiliser l'infrastructure IaaS.
Pour **PaaS**, nous fournissons à la plateforme le code source de l’application, puis on laisse le service se charger automatiquement du reste du processus.
Plus précisément, l’application est placée dans un dépôt Git public, qui est ensuite relié à la plateforme PaaS. Lors de cette connexion, la plateforme détecte automatiquement qu’il s’agit d’une application **Node.js** et installe les dépendances nécessaires. Elle lance le serveur de l’application qui une fois terminé, attribue une URL publique à l'application. Cette URL est accessible depuis un navugateur.
Cependant **IaaS**, n'automatise pas le déploiement de l'application. 
Pour utiliser l'infrastructure IaaS, une instance EC2 est créée sur AWS, cela correspond à un serveur virtuel distant. 
Nous configurons manuellement son environnement notamment l'installation de **Node.js**, les ports réseau et le lancement de l'application.
Afin d'automatiser au mieux le lancement de l'application, on créée dans notre terminal un script : "user data". Grâce à ça, l'appliation est accessible via l'IP publique du serveur.


## Objectifs

- Lancer localement une application
- Déployer une application automatiquement grâce à la plateforme PaaS
- Déployer  une application automatiquement grâce à l'infrastructure IaaS
