---
title: "Stockage avec Google Drive"
description: "Comment stocker et récupérer des images et des projets Adno sur Google Drive."
lead: "Comment stocker et récupérer des images et des projets Adno sur Google Drive."
date: 2024-10-23T19:08:31
lastmod: 2024-10-27T09:42:23  
draft: false
images: []
menu:
  docs:
    parent: "help"
weight: 400
toc: true
---

Google Drive offre une solution utilisée par de nombreuses personnes pour déposer et partager des fichiers. 


Pour obtenir un lien de téléchargement direct d'une image, d'un manifeste IIIF ou d'un projet Adno :

- connectez-vous à votre compte Google Drive,
- chargez le fichier puis faites un clic droit dessus,
- récupérez le lien de partage :
  - cliquez sur "Partager",
  - dans la fenêtre qui s'ouvre, sous "Obtenir le lien", rendre le fichier accessible en sélectionnant "Toute personne disposant du lien",
  - cliquez sur "Copier le lien".

Le lien copié ressemble à ceci : 

```
https://drive.google.com/file/d/FILE_ID/view?usp=sharing
```

Pour transformer ce lien en lien de téléchargement direct, modifiez-le comme suit : 

```
https://drive.google.com/uc?export=download&id=FILE_ID
```

Remplacez `FILE_ID` par l'identifiant unique de votre fichier, qui se trouve dans l'URL d'origine.

Vous pouvez maintenant partager ce lien avec d'autres utilisateurs qui pourront l'utiliser dans l'interface Adno. Vous pouvez aussi utiliser de lien dans un code d'intégration (iframe) pour insérer votre projet dans une page web.
