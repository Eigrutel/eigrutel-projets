# Publication GitHub Pages / Publishing

## Français

### Mettre les fichiers en place

1. Créez le dépôt `eigrutel-projets` sous le compte `Eigrutel`.
2. Décompressez l’archive fournie. Déposez **le contenu du dossier** à la racine du dépôt : `index.html` doit être à la racine, pas dans un sous-dossier `eigrutel-projets`.
3. Conservez les fichiers de licence et les documents. L’archive ZIP du dépôt n’est pas à déposer comme substitut à ces fichiers.
4. Publiez cette racine avec GitHub Pages, en sélectionnant la branche contenant les fichiers et son dossier racine dans les réglages Pages.
5. Après déploiement, ouvrez `https://eigrutel.github.io/eigrutel-projets/`.

`index.html` est le fichier source principal. Modifiez-le pour les évolutions futures. `projets.html` est une redirection, à conserver pour les liens utilisant ce nom. Les favicons des outils sont intégrés au HTML. Déposez aussi le dossier `favicon/`, qui contient `favprojets.png` pour Projets et son icône tactile. Ce PNG reprend le monogramme P existant et peut être remplacé en conservant le même nom. Chaque application distante conserve ses propres ressources dans son dépôt.

### Adresses et sécurité des échanges

Les neuf applications raccordées disposent d’une propriété `url` dans le tableau `APPS` du HTML. Le programme y ajoute `?projets=1` pour activer leur mode intégré. Narratopedia utilise `directUrl` pour sa consultation sans échange de données.

Toutes les applications raccordées et Projets doivent partager exactement la même origine, ici `https://eigrutel.github.io`. Les chemins de dépôts peuvent être différents. Les messages vérifient l’origine, la fenêtre, l’identifiant de l’outil et la session. Ne supprimez pas ces vérifications pour contourner une erreur de chargement.

Les adresses ont été fournies pour les racines des sites. Chaque racine doit ouvrir le bon HTML adapté, et non un README ou une version ancienne. Si nécessaire, ajoutez le nom exact du fichier à la propriété `url` correspondante.

### Vérifications avant release

- Créer un projet de test et ouvrir chacun des neuf outils raccordés.
- Saisir une modification, changer d’outil puis revenir : la modification doit être retrouvée.
- Recharger Projets et vérifier la reprise des données.
- Exporter le JSON, le réimporter et vérifier les données des outils compatibles.
- Dans Farde, importer un ZIP, changer d’outil et revenir ; contrôler les images. Exporter un nouveau ZIP et vérifier sa réimportation dans un autre projet de test.
- Vérifier que le JSON Projets ne contient que la liaison Farde, sans ses images.
- Contrôler la navigation repliable sur ordinateur et petit écran.

Les vérifications de code ont été effectuées lors de la préparation. La validation du chargement depuis les adresses GitHub Pages doit être faite après publication. Les releases ne sont pas nécessaires au service GitHub Pages.

La version reste **0.14.1** pour cette étape. Une version stable 1.0.0 pourra être préparée après validation, avec mise à jour cohérente du HTML, du README, de la notice et de l’historique. Le fichier `RELEASE_NOTES.md` contient un texte prêt pour une éventuelle préversion 0.14.1.

## English

Create `eigrutel-projets` under the `Eigrutel` account. Extract the archive and upload the contents of its folder to the repository root, with `index.html` directly at that root. Keep the licences and documentation. Enable GitHub Pages for the branch and root containing those files, then open `https://eigrutel.github.io/eigrutel-projets/`.

No build step is required. `index.html` contains the complete hub; `projets.html` redirects to it. Tool icons are embedded. Also upload `favicon/favprojets.png`, used for the hub and touch icon. Other tools remain separately hosted.

The configured URLs must open the adapted applications. The hub adds `?projets=1`. The hub and all connected tools must share the same origin. Preserve the origin, source-window and session checks.

Before a release, test every connected tool, switching and reloading, JSON export/import, and Farde ZIP import/export with images. Farde’s global JSON entry must remain a lightweight link. Check desktop and small-screen navigation. The hosted integration still needs validation; version 0.14.1 is retained for this stage.
