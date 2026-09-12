# Notice d’utilisation / User guide

Projets 0.14.1 — Eigrutel Lab — Simon Léturgie — 12-09-2026

## Français

### Langue

Le bouton discret FR / EN est disponible dans votre atelier et dans l’espace projet. Le français est utilisé par défaut. Le choix est mémorisé dans ce navigateur ; il ne traduit pas les noms saisis, les contenus ou les applications ouvertes. Le changement conserve les réglages en cours de saisie.

### Créer un projet

1. Ouvrez Projets et cliquez sur « Nouveau projet ».
2. Donnez un nom au projet. Tous les outils disponibles sont déjà cochés ; décochez ceux dont vous n’avez pas besoin.
3. Ajoutez éventuellement une couverture et choisissez une couleur.
4. Validez, puis ouvrez un outil depuis « Les outils du projet ».

Le nom initialise le projet dans l’outil. Certains outils disposent ensuite de leur propre titre éditable. Choisir un outil ne copie pas automatiquement les données d’un autre outil dans celui-ci.

### Personnaliser la couverture et l’ordre des outils

Dans les réglages, après la couleur, « Texte en bas de couverture » remplace la mention Eigrutel Lab. Un champ vide masque cette mention.

Glissez un bandeau gris vers un autre pour déplacer l’outil, à la souris ou au doigt. Un simple clic ouvre l’outil. Au clavier, placez le focus sur le bandeau et utilisez Alt + une flèche. L’ordre est conservé pour ce projet, repris dans la colonne de gauche et dans le JSON exporté. Les catégories ne sont plus affichées dans la colonne de gauche.

### Travailler et naviguer

Utilisez la colonne de gauche pour changer d’outil. Le bouton « Outils » replie ou déplie cette colonne. « Vue du projet » revient aux bandeaux d’applications. « Votre atelier » revient aux couvertures des projets.

Projets attend la confirmation de sauvegarde avant de quitter un outil raccordé. En cas d’erreur, gardez l’outil ouvert et réessayez ; utilisez son export propre si nécessaire. Les projets présents dans un autre navigateur ne sont pas chargés automatiquement.

Dans « Réglages », vous pouvez changer le nom, la couverture, la couleur et les outils sélectionnés. Retirer un outil de l’affichage ne constitue pas une commande d’effacement de ses données conservées dans le projet.

### Exporter et restaurer

« Exporter le projet » produit un JSON contenant les données des outils raccordés, ainsi que la couverture et les réglages du projet. Les boutons JSON individuels, sous les outils compatibles, servent à échanger leurs données séparément.

« Importer un projet » crée un nouvel espace pour les données contenues dans le JSON ; il ne remplace pas un projet existant. Les données Farde ne sont pas dupliquées : leur liaison locale est conservée. Sur le même navigateur, deux projets importés avec la même liaison Farde peuvent donc ouvrir le même classeur local. Pour une Farde réellement indépendante, utilisez un nouveau projet et rechargez-y le ZIP.

Les versions adaptées de Personnages, Boussole, Univers, Scénoscope, Comic Script, Pop!, WIP et 7 Questions peuvent importer un JSON Projets et y extraire leur partie. Une application absente de l’export ne peut pas être restaurée depuis celui-ci.

### Farde : conserver son ZIP

**ZIP SÉPARÉ — PENSER À ENREGISTRER LE ZIP !**

1. Ouvrez Farde depuis le projet.
2. Pour reprendre un classeur existant, importez son ZIP une première fois dans cet espace.
3. Sur le même navigateur et à la même adresse, les fiches et images sont ensuite retrouvées depuis le stockage local.
4. Sauvegardez le ZIP depuis Farde après vos modifications. La vue du projet rappelle le nom du dernier ZIP connu et indique les modifications à exporter lorsqu’elles sont détectées.

Le JSON global conserve uniquement une liaison légère. Il ne contient pas les images ou les fiches Farde. Le nom du ZIP mémorisé n’est pas un accès au fichier sur votre disque : cette version recharge le classeur local du navigateur, pas automatiquement un ZIP téléchargé. Si ce stockage est absent, sélectionnez à nouveau le ZIP. Vérifiez que le téléchargement du ZIP a bien abouti : sa génération ne prouve pas qu’il est conservé durablement sur votre appareil.

### Changer d’appareil, de navigateur ou d’hébergement

Avant de quitter l’ancien environnement, exportez le JSON du projet et le ZIP Farde. Dans le nouvel environnement, importez le JSON puis ouvrez Farde et rechargez son ZIP. Le passage de Stripmee à GitHub Pages nécessite cette opération.

L’effacement des données du site, la navigation privée ou les limites de stockage du navigateur peuvent compromettre la conservation locale. Gardez vos sauvegardes ailleurs que dans le seul navigateur.

### Travailler à plusieurs

Transmettez le JSON et, si nécessaire, le ZIP Farde. Convenez de la personne qui modifie chaque version. Il n’existe pas de fusion automatique ni de synchronisation en temps réel. Identifiez vos sauvegardes par nom et date.

### Dépannage

- **L’outil reste en ouverture :** vérifiez que son adresse ouvre l’application adaptée et que Projets est servi sur la même origine que les outils.
- **Une page de présentation s’affiche :** l’adresse du dépôt ne mène pas au bon HTML. Corrigez l’URL de cet outil dans le catalogue `APPS` de `index.html`.
- **Le classeur Farde est absent :** rechargez son ZIP dans Farde ouverte depuis le projet.
- **Les données de Stripmee ne sont pas visibles :** elles ne migrent pas automatiquement vers GitHub Pages. Retournez sur l’ancienne adresse pour exporter.
- **Un ancien affichage subsiste après publication :** rechargez la page après la fin du déploiement GitHub Pages.

## English

### Language

Use FR / EN in your comic studio or project toolbar. French is the default; the browser remembers your preference. Switching does not translate user content or connected applications, reload the active tool, or discard unsaved project settings.

### Create and navigate

Choose “Nouveau projet”, enter a name, keep all available tools selected or deselect some, and optionally add a cover and colour. Open a tool from the project overview. Use the left navigation to switch tools; “Outils” collapses it and “Votre atelier” returns to the comic studio.

The hub waits for connected tools to acknowledge saving before leaving them. If saving fails, keep the tool open, retry and use its own export when necessary. Selecting tools does not automatically transfer content between them.

### Customise covers and tool order

In project settings, the cover-footer field appears after the colour control and defaults to Eigrutel Lab. Leave it empty to hide the text. Drag a grey tool banner onto another using mouse or touch to reorder it; a simple click opens the tool. Keyboard users can focus a banner and press Alt + an arrow. The order is saved per project, reflected in the left navigation and included in JSON exports. Category headings are removed from the left navigation.

### Back up and restore

“Exporter le projet” downloads the project JSON. “Importer un projet” creates a new project space for the data contained in that JSON. Compatible tools also offer individual JSON import/export and can extract their own data from a global project JSON.

**Farde uses a separate ZIP. Its cards and images are not included in the project JSON.** Open Farde inside the project and import your existing ZIP once. Subsequent openings in the same browser and site use the locally stored binder. Save an updated ZIP after making changes.

The saved ZIP name is only a reference. This version does not automatically reopen a downloaded ZIP from a disk path. If the browser’s binder is missing, select the ZIP again. Confirm that the ZIP download completed successfully.

Importing a project preserves its Farde link. In the same browser, two projects with that link can open the same local binder. For an independent binder, create a new project and import the ZIP there.

### Transfer and collaborate

Keep the project JSON and Farde ZIP together. On another browser, device or origin, import the JSON and reload the ZIP inside Farde. There is no cloud backup, live collaboration or automatic merging. Coordinate file versions when working with others.

Browser storage may be cleared or become unavailable. Export before changing hosting, including migration from Stripmee to GitHub Pages. The website needs network access to load its separately hosted tools; this package is not a complete offline bundle.

### Troubleshooting

If a tool will not connect, verify its adapted version, URL and shared origin. A repository presentation page indicates that the configured URL does not open the application HTML. If Farde is empty, reload its ZIP. If old content remains after an update, reload after deployment finishes.

---
Documentation © 2026 Simon Léturgie — CC BY-SA 4.0, sauf mention contraire / unless otherwise stated.
