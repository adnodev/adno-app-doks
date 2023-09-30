---
title: "Visualiser un projet Adno"
description: "Chaque projet Adno peut-être exporté et partagé sous la forme d'un simple fichier texte qui peut permettre diveres représentations, y compris sans Adno."
lead: "Chaque projet Adno peut-être exporté et partagé sous la forme d'un simple fichier texte qui peut permettre diveres représentations, y compris sans Adno."
date: 2023-06-02T09:19:42+01:00
lastmod: 2023-06-02T09:19:42+01:00
draft: false 
weight: 977
---

<link rel="stylesheet" type="text/css" href="https://ncsu-libraries.github.io/annona/dist/annona.css">

Un projet Adno se présente sous la forme d'un simple fichier texte qui peut être enrégistré et partagé. Ce fichier est au format  du standard [Web Annotation model format](https://www.w3.org/TR/annotation-model/). Il peut donc être traité par Adno et par tout autre logiciel compatible. 

Nativement, Adno permet d'incorporer un projet Adno dans une page web. Il est nécessaire que le projet soit accessible en ligne. Ensuite il suffit d'insérer une balise `iframe` en respectant la syntaxe suivante. 

```
<iframe 
    src="https://w.adno.app/#/embed?url=URL DU PROJET" 
    height="600px" width="100%"
    allow="fullscreen"
></iframe>
```  

Soit : 

<iframe 
    src="https://w.adno.app/#/embed?url=https://static.emf.fr/adno/embed/annotations.json" 
    height="600px" width="100%"
    allow="fullscreen"
></iframe>

## Adno views tags

Le projet compagnon [Adno views tags](https://github.com/adnodev/adno-views-tag) vous permet d'intégrer différents types de visualisations dans vos pages web. Attention, il ne fonctionne qu'avec des projets Adno basés sur des images IIIF.  

Pour obtenir chaque rendu, il suffit d'associer des attributs du type `data-*` à une balise enveloppante. Cf. exemple ci après ou MODE est à remplacer par `infos`, `list`, `slider`, `embed` ou `annona`, ainsi que URL par l'url d'un projet Adno. 

```
<div data-adno="MODE" 
    data-src="URL"
    data-width="800px";
></div>
```

Pour en savoir plus et notamment la liste des options associées à chaque mode, consultez la [documentation](https://github.com/adnodev/adno-views-tag).


### Infos

Liste les métadonnées du projet.

<div data-adno="infos"
data-src="https://static.emf.fr/adno/embed/annotations.json"
data-title-level="h4"
></div>

### Slider

Visualisation en mode diapo

<div data-adno="slider"
data-src="https://static.emf.fr/adno/embed/annotations.json"
data-style="normal"
></div>

### Liste

Liste des images et de leurs annotations en légende

<div data-adno="list"
data-src="https://static.emf.fr/adno/embed/annotations.json"
data-image-max-height="400px"
data-image-max-width="500px"
data-caption-position="bottom"
></div>

### Annona

Il est aussi possible de faire appel à la superbe bibliothèque [Annona](https://ncsu-libraries.github.io/annona/) qui offre une flopée de possibilités.  

<div data-adno="annona"
data-src="https://static.emf.fr/adno/embed/annotations.json"
data-infos="true"
data-option-autorun_onload="true"
data-option-autorun_interval="4"
></div>

<script src="https://code.jquery.com/jquery-3.6.2.min.js"></script>
<script src="https://static.emf.fr/adno/views/adno-display-tags.js"></script>
<script src="https://static.emf.fr/adno/views/jquery.shortslider.min.js" defer></script>
<script src="https://ncsu-libraries.github.io/annona/dist/annona.js" defer></script>


