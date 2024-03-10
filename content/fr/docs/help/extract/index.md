---
title: "Extraire les images d'un manifeste"
description: "Il est parfois nécessaire ou intéressant de récupérer les URL des images référencées dans un manifeste."
lead: "Il est parfois nécessaire ou intéressant de récupérer les URL des images référencées dans un manifeste."
date: 2024-03-10T09:19:42+01:00
lastmod: 2024-03-10T09:19:42+01:00
draft: false 
weight: 940
---

Entrez l'URL du manifeste pour extraire les références des images.

<div id="manifest_enter">
    <form>
        <label for="manifest_uri" style="display: block;"><b>URL du manifeste :</b></label>
        <input type="text" id="manifest_uri" style="width:100%; margin: 10px 0;">
        <div style="display: block;">
		<button onclick="loadManifest(event)">Charger</button>
        	<button onclick="clearManifest(event)" class="button">Réinitialiser</button>
	</div>
    </form>
</div>
<div id="manifest_content" style="margin: 0 0 30px 0"></div>

La base du code de cette fonctionnalité provient du site [IIIF Training](https://training.iiif.io/advanced_iiif/day-two/image-servers/images_in_manifest.html).

<script src="/js/canvas_finder.js"></script>


