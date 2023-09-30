---
title: "Installation de Adno"
description: "Instructions pour installer Adno."
lead: "Adno est un logiciel libre que vous pouvez installer sur votre propre ordinateur ou sur un serveur statique pour d'autres utilisateurs sur le web."
date: 2022-12-23T19:08:31
lastmod: 2022-12-27T09:42:23  
draft: false 
images: []
menu:
  docs:
    parent: "help"
weight: 100
toc: true
---

## Prerequis

Avant de personnaliser et d'installer Adno sur votre ordinateur ou sur un serveur, vous devez d'abord installer les éléments suivants :

- [Node.js](https://nodejs.org/fr), la plateforme de développement Javascript utilisée par Adno,
- [Yarn](https://yarnpkg.com/) un gestionnaires de paquets et de dépendances pour Node.js.

Il est important de noter qu'Adno nécessite un accès à Internet pour fonctionner, même en mode local.

## Récupérer Adno

Vous avez deux options pour obtenir Adno : vous pouvez télécharger l'archive de la dernière version et la dézipper, ou bien cloner le dépôt des sources d'Adno en utilisant la commande git.

- téléchargez l'[archive de la dernière version](https://github.com/adnodev/adno/releases) puis dézippez la,
- ou clonez le dépot de Adno : `git clone https://github.com/adnodev/adno.git`.  
 
## Préparer l'installation

Déplacez vous dans le répertoire des sources de Adno.

Renommez le fichier `.env.example` en `.env`  puis éditez le en ajustant les valeurs des variables qu'il contient pour personnaliser votre installation.

- `ADNO_MODE` : Adno est installable, soit en version complète avec l'éditeur et le visualiseur, soit en version reduite avec seulement le visualiseur, respectivement les valeurs `FULL` ou `LIGHT`.
- `ADNO_TITLE` : nom de votre installation.
- `ADNO_FOOTER` : présence `TRUE` ou absence `FALSE` d'un texte en pied de page.
- `ADNO_FOOTER_TEXT` : texte visible dans le pied de page si `ADNO_FOOTER` est à `TRUE`.
- Paramétrage de [Matomo](), un logiciel de suivi des statistiques de fréquentation conforme au RGDP :
  - `MATOMO_SITE_ID` : identifiant dans Matomo de l'installation Adno,
  - `MATOMO_URL` : url de l'installation Matomo.
- `GRANTED_IMG_EXTENSIONS` : extensions autorisées pour les images. 

## Utiliser Adno en local

Vous pouvez alors lancer Adno en local.

- entrez la commande `yarn start`,
- avec votre navigateur rejoignez l'url indiquée, généralement [http://localhost:1234](http://localhost:1234). 

Allez-y !

## Mettre Adno en ligne 

Pour rendre votre installation Adno accessible aux internautes sur le web, vous devez construire une version réduite et optimisée des fichiers Adno nécessaires à son fonctionnement en ligne, puis les déposer sur votre serveur. Suivez ces étapes :

- entrez la commande `yarn build`,
- les fichiers utiles sont générés pour les deux versions dans les répertoires :
  - `adno-full` pour la version avec éditeur et visualiseur,
  - `adno-light` pour visualiseur seul,
- copiez le contenu du répertoire de votre choix sur votre serveur.

Adno ne s'exécute que dans votre navigateur et pas du côté serveur. Vous pouvez alors utiliser un serveur de fichiers statiques. Si vous avez des connaissances en `git` et que vous possédez un compte sur [Github](https://github.com/), vous pouvez utiliser la fonctionnalité [Page](https://pages.github.com/) pour mettre en ligne Adno. Le service [Netlify](https://www.netlify.com/) offre aussi une autre solution gratuite intéressante qui vous permet de faire l'économie d'un serveur.  

### Page Github

à venir 

### Netlify 

à venir 

