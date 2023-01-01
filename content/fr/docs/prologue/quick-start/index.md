---
title: "Mode d'emploi rapide"
description: "L'essentiel en une page pour débuter avec Adno."
lead: "L'essentiel en une page pour débuter avec Adno."
date: 2022-11-24T10:45:41   
lastmod: 2022-12-30T21:17:03  
draft: false
images: []
menu:
  docs:
    parent: "prologue"
weight: 110
toc: true
---

## Un service en ligne

Le plus simple pour commencer est d'utiliser [le service en ligne](https://w.adno.app) du projet. Il est gratuit et ne nécessite pas d'inscription. Vous pouvez aussi partir [d'un exemple](/example).

<a href="https://w.adno.app" target="_blank"><button type="button" class="btn btn-primary">Essayer maintenant !</button></a>
<a href="/example" target="_blank"><button type="button" class="btn btn-success">Exemples</button></a>


Comme Adno est un logiciel libre, vous pouvez aussi l'installer pour vous-même et les autres. Les sources et les instructions d'installation sont accessibles sur [Github](https://github.com/adnodev/adno).

{{< alert icon="👉" context="info" >}}
Adno est en cours de développement, ses fonctionnalités et son interface sont susceptibles de changer.
{{< /alert >}}

## Débuter un projet 

L'écran d'accueil de Adno, se présente sour la forme d'un simple formulaire. 

![champ de saisie](url-field.png)

Il permet :

- **de créer un projet** en entrant l'URL d'une image statique ou d'une image IIIF,
- **d'importer un projet** en chargeant le fichier d'un projet Adno. 

Cet écran affiche la liste des projets créés dans cette session de votre navigateur. 

![Écran d'accueil](home.png)

### Partir d'une image statique

L'image au format `png` ou `jpg` doit être présente en permanence sur Internet et vous devez connaitre son adresse (l'URL). Entrez cette URL dans le champ dédié puis cliquez sur `Créer mon projet`.
 
<button class="btn btn-copy"></button>
``` 
https://upload.wikimedia.org/wikipedia/commons/f/f3/Chenille_de_Grand_porte_queue_%28macaon%29.jpg
```

### Partir d'une image IIIF

Si vous ne connaissez pas IIIF, consultez cette [page de présentation](https://doc.biblissima.fr/iiif/introduction-iiif/) pour en savoir plus.

Vous pouvez utiliser :

- l'url directe d'une image IIIF, elle se termine par `info.json`
- l'url d'un document, un manifeste IIIF, cependant actuellement seule la première image est prise en compte. 

<button class="btn btn-copy"></button>
```
https://free.iiifhosting.com/iiif/1c8d49343676a04fffcd92979c02e9394e48bac96f590fffbadffc9133cd06b9/info.json
```

<button class="btn btn-copy"></button>
```
https://gallica.bnf.fr/iiif/ark:/12148/btv1b8626777x/f13/info.json
```

### Partir d'un exemple

La [page des exemples](/fr/example/) propose, pour commencer, des ressources issues des domaines les plus divers. 

### Importer un projet 

Utilisez le bouton `Importer un projet` pour teléverser un fichier Adno préalablement téléchargé.

## Visualiser et éditer son projet 

La même interface vous permet de visualiser et d'éditer un projet. 

Fonctions des icônes de l'entête :

- <i class="fa-solid fa-house"></i> retour à la page d'accueil et à la liste des projets, 
- <i class="fas fa-download"></i> exportation du projet courant, 
- <i class="fas fa-file"></i> <i class="fas fa-file-edit"></i> respectivement lecture et édition des métadonnées du projet 
- <i class="fas fa-toggle-off"></i> passage du mode visualisation au mode édition, et inversement.


### Interface d'édition
![Interface d'édition](editor.png)

### Interface de visualisation
![Interface de visualisation](viewer.png)

## Retrouver ses projets 

Les projets sont conservés dans votre navigateur. Vous pourrez les retrouver en rouvrant une session sur le site à partir duquel ils ont été créés. 

{{< alert icon="👉" context="danger">}}
En navigation privée les projets sont "oubliés" à la fermeture de la session. Il peut en être de même avec un paramétrage restrictif de votre navigateur. 
{{< /alert >}}

### Aide 

Consultez la foire aux question et la documentation pour en savoir plus (attention ! ces parties sont encore incomplètes). 
En cas de problème ou de suggestion n'hésitez à [nous contacter](/contact).

