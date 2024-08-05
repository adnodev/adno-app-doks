---
title: "Utilisation de IPFS"
description: "Le système de fichiers decentralisés IPFS offre une solution innovante et relativement simple pour diffuser les projets Adno."
lead: "Le système de fichiers decentralisés IPFS offre une solution innovante et relativement simple pour diffuser les projets Adno."
date: 2022-12-23T19:08:31
lastmod: 2022-12-27T09:42:23  
draft: false
images: []
menu:
  docs:
    parent: "help"
weight: 300
toc: true
---

## Qu'est-ce qu'IPFS ?

IPFS, le système de fichier interplanétaire, est un protocole _pair à pair_ de distributions de contenus numériques. Son fonctionnement est décentralisé. La diffusion d'un fichier ne repose plus sur un serveur comme pour le web mais sur un réseau de nœuds interconnectés. Votre ordinateur ou votre navigateur peut constituer un de ces nœuds. 

IPFS utilise un système d'adressage décentralisé basé sur le contenu au lieu d'un lien vers un emplacement. Chaque fichier devient accessible via un identifiant unique, son CID.

## Pourquoi utiliser IPFS avec Adno

Pour partager un fichier avec une personne, le plus simple est de lui transmettre en pièce jointe par mail ou via un service comme WeTransfert. D'autant que le fichier d'un projet Adno ne comporte que du texte et reste généralement de petite taille. 

Cependant, si l'on souhaite le diffuser plus largement, il faut disposer d'un serveur de fichiers ou d'un site web sur lequel le déposer, puis populariser l'URL du fichier.

IPFS simplifie grandement ce processus, il suffit de déposer le fichier du projet Adno sur IPFS et de diffuser son CID. 

## Comment faire ?

Utiliser un service ou installer IPFS sur son propre ordinateur. 

### Utiliser un service

Des opérateurs proposent des solutions de stockage distribué utilisant IPFS. 

Pour un usage basique, ils proposent une offre gratuite et disposent d'interfaces web simples et intuitives. 

| Opérateur | Limites de l'offre gratuite | Note | 
| -------- | -------- | -------- |
| [Filebase](https://filebase.com/) | 5G et 1000 fichiers | Possibilité de charger des images et des projets, temps de réponse assez long parfois | 
| [Pinata](https://www.pinata.cloud/) | 1G et 500 fichiers | Possibilité de charger des images et des projets |
| [NFT.storage](https://nft.storage/) | 32G | Ne prends en charge que des CID |

### Disposer de IPFS sur son ordinateur

Pour commencer, le plus simple et le plus rapide consiste à installer le logiciel  [IPFS Desktop](https://docs.ipfs.tech/install/ipfs-desktop/) compatible Windows, Mac et Linux.

Les navigateurs Brave et Opera sont compatibles avec IPFS. [IPFS Companion](https://docs.ipfs.tech/install/ipfs-companion/) est un module dédié aux navigateurs avec Chrome, Edge, Firefox, Brave et Opera.

## Que faire avec Adno ?

Un CID ressemble à une assez longue suite de chiffres et de lettres : 

- `QmS6BrC3G3EdWozCuRfEp2avZHwwzyDCKpjvJDcCauk1jL`. 

Ce CID pourra être saisi dans Adno en lieu et place d'une URL.

Il est possible de «&nbsp;localiser&nbsp;»  un fichier IPFS sur le web en utilisant une passerelles. Il suffit d'ajouter le CID à l'URL du point d'entrée de la passerelle de la forme : 

- `https://gateway.tld/ipfs/`. 

Exemples : 

- https://ipfs.io/ipfs/QmS6BrC3G3EdWozCuRfEp2avZHwwzyDCKpjvJDcCauk1jL
- https://dweb.link/ipfs/QmS6BrC3G3EdWozCuRfEp2avZHwwzyDCKpjvJDcCauk1jL
