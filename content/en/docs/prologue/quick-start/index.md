---
title: "Quick Start"
description: "The essentials in one page to get started with Adno.."
lead: "The essentials in one page to get started with Adno.."
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

## An online service 

The easiest way to get started is to use the [online service](https://w.adno.app). It is free and does not require registration. You can also start with [an example](/example).

<a href="https://w.adno.app" target="_blank"><button type="button" class="btn btn-primary">Get started!</button></a>
<a href="/example" target="_blank"><button type="button" class="btn btn-success">Examples</button></a>

As Adno is free software, you can also install it for yourself and others. The sources and installation instructions are available on [Github](https://github.com/adnodev/adno).

{{< alert icon="👉" context="info" >}}
Adno is under development, its features and interface are subject to change.
{{< /alert >}}

## Start a project 

The Adno home screen is divided into three areas.

The first is a simple form, the second, next to it, allows you to load an existing project, and the third, below it, lists the projects stored by the browser.

![home page](home.png)

It allows you to:

- **create a project** by entering the URL of a static image or an IIIF image,
- **import a project** by loading an Adno project file.
- **retrieve a project** a previously created project stored in your browser.

![project example](project.png)

For each existing project in the browser, a series of buttons allows access to the following features:

- **<i class="fa-solid fa-eye"></i> Preview**
- **<i class="fa-solid fa-pen-to-square"></i> Edit**
- **<i class="fa-solid fa-copy"></i> Duplicate**
- **<i class="fa-solid fa-download"></i> Download**
- **<i class="fa-solid fa-trash"></i> Delete**

### Start with a static image

The image in `png` or `jpg` format must be on the Internet permanently and you must know its address (the URL). Enter this URL in the dedicated field and click on `Create my project`. 

<button class="btn btn-copy"></button>
``` 
https://upload.wikimedia.org/wikipedia/commons/f/f3/Chenille_de_Grand_porte_queue_%28macaon%29.jpg
```

### Start with an IIIF resource 

If you're not familiar with IIIF or if you want to learn more, you can check out the [IIIF Online workshop](https://training.iiif.io/iiif-online-workshop/) provided by the [IIIF consortium](https://iiif.o) and led by Glen Robson.

You can start with an IIIF manifest or an IIIF image.

#### IIIF Manifest

This is a URL provided by the document publisher. The manifest describes the document with its metadata and images.

<button class="btn btn-copy"></button>
```
https://api.artic.edu/api/v1/artworks/251131/manifest.json
```

If there are several images, select one.

![Sélection d'une image dans un manifeste](select.png)

#### IIIF Image

You then use the direct url of an IIIF image, ending with `info.json`. 

<button class="btn btn-copy"></button>
```
https://gallica.bnf.fr/iiif/ark:/12148/btv1b8626777x/f13/info.json
```

### Start with an example

The [examples page](/en/example/) suggests resources from various domains. 

### Import a project

Use the Import a project button (`Importer un projet`) to upload a previously downloaded Adno file.

## View and edit your project 

The same interface allows you to view and edit a project.

Icon options in the header :

- <i class="fa-solid fa-house"></i> return to the home page and to the list of projects, 
- <i class="fas fa-download"></i> export the current project, 
- <i class="fas fa-file"></i> <i class="fas fa-file-edit"></i> respectively reading and editing of the project metadata, 
- <i class="fas fa-toggle-off"></i> switch from view mode to edit mode, and vice versa.


### Editing interface

![Editor screen](editor.png)

To create a new annotation choose an annotation form:

![Annotation buttons](annoButtons.png)

Then select an area on the image by clicking and dragging. The editing interface appears to write the annotation.

To modify the content of an existing annotation, click on it. To resize it, move on the circles at the corners.

Actions to manage each annotation from the annotation list:

- **<i class="fa-solid fa-pen-to-square"></i> Edit** this annotation,
- **<i class="fa-solid fa-bullseye"></i> Focus** on the annotation area,
- **<i class="fa-solid fa-up-long"></i> <i class="fa-solid fa-down-long"></i> Move** the annotation into the list of annotations,
- **<i class="fa-solid fa-trash"></i> Delete** the annotation.

### Viewing interface

![Visualisation screen](viewer.png)

- **<i class="fa-solid fa-play"></i> Autoplay** of annotations (see settings), 
- **<i class="fa-solid fa-magnifying-glass-minus"></i> Back** to the beginning of the annotation 
- **<i class="fa-solid fa-arrow-left"></i> Previous annotation**,
- **<i class="fa-solid fa-arrow-right"></i> Next annotation**,
- **<i class="fa-solid fa-expand"></i> fullscreen**,

Keyboard shortcuts:

- Key `p` or `P` to start the autoplay,
- Key `e` or `E` to toggle FullScreen,
- Key `s` or `S` to toggle annotation bounds,
- Key `t` or `T` to toggle the toolsbar,
- Key <code><i class="fa-solid fa-arrow-left"></i></code> and <code><i class="fa-solid fa-arrow-right"></i></code> to move from the current annotation to the previous or the next one.

L'icone **<i class="fa-solid fa-gear"></i>** allows you to adjust some playback settings :

- delay between two annotations (5 seconds by default),
- viewport navigator,
- display the toolbar in full screen mode, 
- display the navigation bar for annotations, 
- always start autoplay at the first annotation, 
- enable image rotation,,
- display the toolbar.

Actions to access each annotation from the annotation list: 

- **<small>READ MORE</small> <i class="fa-solid fa-circle-plus"></i> View** the annotation content in a modal window, 
- **<i class="fa-solid fa-bullseye"></i> Focus** on the annotation area,

## Retrieve your projects 

Projects are stored in the local storage of your browser. You will be able to find them by reopening a session on the site from which they were created.

{{< alert icon="👉" context="danger">}}
In private browsing projects are "forgotten" when you close your session. The same can happen with a restrictive setting of your browser.
{{< /alert >}}

## Share your projects

Start by downloading your Adno project. It takes the form of a simple text file in [json format](https://json.org).

This file is generally light. So you can easily send it by e-mail. Your correspondent will then be able to visualize it, as well as make variations or corrections.

You can also place your file online and distribute its URL. To do this, you can use a website or file server. The IPFS protocol provides an interesting decentralized alternative.

Once your Adno project is online, you can make it visible on a web page by inserting an `iframe` tag and adjusting the parameters below.

```
<iframe
    src="https://w.adno.app/#/embed?url=URL HERE"
    height="600px"
    width="100%"
    allow="fullscreen"
></iframe>

```

Note that by inserting the URL of an IIIF or non-IIIF image, or an IIIF manifest, you can obtain an IIIF viewer.

[Adno views tags](https://github.com/adnodev/adno-views-tag) allows you to embed different types of visualization in your web pages.

## Help 

Check the frequently asked questions and the documentation to learn more (beware! these parts are still incomplete). If you have any problems or suggestions, please [contact us](/contact).

