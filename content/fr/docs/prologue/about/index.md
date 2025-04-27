---
title: "À-propos de Adno"
description: "Adno est une application web de visualisation, d’édition et de partage de récits et de parcours sur des images statiques et des images IIIF. Elle s'adresse principalement aux médiateurs culturels et scientifiques ainsi qu'aux enseignants. Elle concerne notamment les fonds patrimoniaux, les archives, les bibliothèques, la recherche scientifique, les humanités numériques, et plus généralement la valorisation de données culturelles et scientifiques."
lead: "Adno est une application web de visualisation, d’édition et de partage de récits et de parcours sur des images statiques et des images IIIF. Elle s'adresse principalement aux médiateurs culturels et scientifiques ainsi qu'aux enseignants. Elle concerne notamment les fonds patrimoniaux, les archives, les bibliothèques, la recherche scientifique, les humanités numériques, et plus généralement la valorisation de données culturelles et scientifiques."
date: 2022-12-23T19:08:31
lastmod: 2022-12-30T21:15:46  
draft: false
images: []
menu:
  docs:
    parent: "prologue"
weight: 100
toc: true
---

Porté par l'[Espace Mendès France](https://emf.fr) - Poitiers, en partenariat avec l'[Abbaye de Saint-Savin-sur-Gartempe et la vallée des fresques](https://www.abbaye-saint-savin.fr/), la [Bibliothèque Sainte-Geneviève](https://www.bsg.univ-paris3.fr/iguana/www.main.cls), Paris, la [Cité internationale de la bande dessinée et de l'image](http://www.citebd.org/), Angoulême, les [Musées de Poitiers](https://www.poitiers.fr/c__231_977__accueil_musee_sainte_croix.html), le [Muséum d’histoire naturelle de La Rochelle](https://museum.larochelle.fr/), Adno  a été retenu parmi les seize lauréats de l’édition 2022 de l’appel à projets [Services numériques innovants](https://www.culture.gouv.fr/Presse/Communiques-de-presse/Resultats-de-l-appel-a-projets-Services-numeriques-innovants-2022) porté par le ministère de la Culture. Adno a été initialement développé et soutenu par la [Serli](https://www.serli.com/).

[Dossier de présentation du projet](/fr/blog/pr%C3%A9sentation-du-projet/EspaceMendesFrance_PresentationProjet.pdf) 

![Logos](bloc-logos.png)

## Origine de Adno

Un acteur culturel qui souhaite mettre en ligne ses collections d'images est confronté à des choix complexes. Les solutions sont trop souvent onéreuses, peu évolutives et surtout incompatibles les unes avec les autres alors qu'elles tentent pourtant de répondre à des besoins communs.

L’initiative [IIIF (International Image Interoperability Framework)](https://iiif.io) est née de la constatation que la diffusion des images sur le web était « trop lente, trop coûteuse, trop disjointe et trop complexe ». Elle a été lancée en 2015 par la British Library, la Bibliothèque Nationale de France, Die Bayerische Staatsbibliothek, Nasjonalbiblioteket, Artstor, Wellcome Trust et les universités Cornell, Oxford, Princeton, Stanford et Yale. Le Consortium réunit aujourd’hui une soixantaine de bibliothèques de recherche, de bibliothèques nationales, d'archives, de sociétés et d'agrégateurs du monde entier. De nombreux professionnels et amateurs contribuent aussi au dynamisme de la communauté.

IIIF est devenu le cadre technique commun et standardisé de diffusion des images de haute qualité et de leurs métadonnées. Les images deviennent véritablement accessibles, consultables, comparables, manipulables, citables, annotables et mixables par n'importe quelle application compatible capable de se « brancher » sur les entrepôts des uns et des autres. Des centaines de millions de ressources — reproductions de documents et d'œuvres, photos, dessins, bandes dessinées, cartes, plans, graphiques,  etc. — sont ainsi exposées.  Le protocole s’est étendu récemment à l’audio, à la vidéo et à la 3D.

Si les serveurs et les visualiseurs IIIF sont répandus et matures, les outils « grand public » restent expérimentaux et souvent fermés. Quelques logiciels et services de « storytelling » dédiés à l'éditorialisation et à la médiation de ressources IIIF sont particulièrement intéressants :  

- [Storiiies](https://storiiies.cogapp.com/) - un service bien conçu et en accès libre mais propriétaire.
- [Panel Truck](https://cartinal.leventhalmap.org/documentation/panel-truck.html) - un logiciel libre qui requiert l'édition de code.
- [Exhibit](https://www.exhibit.so/) - un service initié pendant la crise Covid-19 pour assurer la continuité pédagogique d’une université.
- [Tesselle](https://medialab.sciencespo.fr/outils/tesselle/) - un outil libre développé au Media Lab de SciencesPo,  avec une très bonne ergonomie mais ne supporte par IIIF.

En associant étroitement visualisation et édition, Adno tente de dépasser les limites de l’existant et apporte une solution accessible et conviviale aux chercheurs, aux artistes, aux enseignants, aux médiateurs culturels et scientifiques. Elle vise à développer de nouveaux usages créatifs et pédagogiques.

## Description

Adno permet d’explorer une œuvre ou un document dans son ensemble ou par ses détails, de présenter des connaissances, de raconter des histoires, de dessiner ou de taguer, etc. et en pratique, de lire et d’écrire des annotations et de les partager simplement.  

Adno est une application web, simple et ergonomique, qui permet la visualisation, l’édition et la diffusion d’images IIIF annotées. Elle prend en entrée une image IIIF (seule ou provenant d’un manifeste) ou une liste d’annotations (au sens W3C ou IIIF). Elle produit une liste ordonnée d’annotations. Une annotation associe des informations textuelles ou multimédias à une zone.  Concrètement, Adno présente les caractéristiques suivantes :

- __côté serveur :__ l'installation est simplifiée (fichiers statiques), le service ne distribue et n'enregistre aucun contenu et ne collecte pas de données personnelles,

- __côté client :__ traitement, stockage et diffusion sont opérés par le navigateur, l'application est utilisable sur une tablette, un ordinateur ou une table tactile.

L'InterPlanetary File System (IPFS) est le protocole utilisé par Adno pour partager les annotations. C’est un système pair à pair de distribution de contenus adressables par hypermédia. Il permet de stocker des fichiers ou des arborescences de manière décentralisée et pérenne, et d’y accéder via un identifiant IPFS ou une URL http classique.

Adno repose sur des standards ouverts et des composants libres. Il est développé de manière agile en respectant les bonnes pratiques (code, tests, documentation, accessibilité, etc.).  C’est un service en ligne (adno.app), un logiciel autonome et un composant naturellement intégrable aux technologies du Web3 : web sémantique, intelligence artificielle, blockchain, etc.

Par conception, le recours aux protocoles IPFS et IIIF contribue à limiter la consommation énergétique. Les  listes d'annotations sont textuelles et donc très légères, les images y sont seulement référencées. Enfin, seules les parties d'images nécessaires sont téléchargées.

Adno facilite la diffusion et la visibilité des contenus culturels et contribue à l’amélioration des moyens techniques permettant l’interopérabilité et la réutilisation, en adéquation avec la feuille de route « données et contenus culturels » du ministère de la culture.

## Caractère innovant

IIIF offre un accès simplifié et uniforme à des fonctions avancées d’interactions avec les documents : exploration fluide et enrichie des images (zoom profond, rotation, etc.), visualisation multi-couches et multispectrales, comparaison et annotation de zones, etc.

Adno est un outil commun au service des humanités numériques, de l’éducation, de la recherche et de la création. Il rend abordable et populaire deux technologies innovantes et prometteuses : IIIF et IPFS. Ces approches fondamentalement décentralisées et collaboratives concrétisent le potentiel du web sémantique et préfigurent le web distribué.   

Adno ouvre des nombreuses perspectives : prise en charge des audios, des vidéos et des objets 3D, édition collaborative, production participative (crowdsourcing), développement de modules pours logiciels spécialisés de bibliothèques numériques ou de publication, connexion avec des dispositifs de reconnaissances de formes (IA), etc.

## Caractère diffusable et réplicable

Adno est librement utilisable sur adno.app. Les sources comme la documentation sont publiées sous licences libres. Elles sont téléchargeables depuis les forges logicielles ouvertes. Adno peut donc être installée et adaptée sans aucune restriction.

## Versions

- beta 2 : 19 septembre 2023
- beta 1 : 29 mars 2023
- beta 0 : Noël 2022
- alpha : octobre 2022

## Contact

N'hésitez pas à nous contacter via le [formulaire en ligne](https://adno.app/contact/).
