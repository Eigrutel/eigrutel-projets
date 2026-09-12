# Repères de maintenance / Maintenance guide

Le fichier source principal est `index.html`. Il contient le HTML, le CSS, le catalogue, les favicons des outils, les traductions et la logique JavaScript. Il ne nécessite pas de compilation. `projets.html` redirige vers ce fichier. Le favicon propre à Projets est `favicon/favprojets.png`.

## Langues

Les textes français sont les clés du dictionnaire `EN`. `tr()` choisit la traduction, `locale()` définit le format des dates. Les attributs `data-i18n` du HTML statique sont appliqués par `applyStaticLanguage()`. Les fonctions de rendu utilisent `tr()` explicitement : les noms, couvertures et contenus utilisateur ne passent pas dans la traduction. `switchLanguage()` conserve l’iframe ouverte et les valeurs du formulaire. La langue des outils raccordés reste indépendante.

## Projets et sauvegardes

`APPS` décrit les outils, leurs URL et leur état. Les outils retirés restent dans le catalogue pour accepter les anciens exports ; ils ne sont ni proposés ni présélectionnés. `seed()` initialise les formats natifs. L’ordre de `project.apps` pilote les bandeaux et la colonne. `project.imprint` personnalise le bas de couverture ; son absence signifie Eigrutel Lab.

`persist()` sérialise les écritures IndexedDB. `flush()` attend la sauvegarde de l’outil avant de quitter l’iframe. Les messages vérifient l’origine, la fenêtre émettrice, l’identifiant de l’outil et la session. Les validations d’import précèdent toute modification. Les formats des exports restent en version 1 : la version de l’interface ne remplace pas celle du format de données.

Farde conserve uniquement une liaison locale dans le JSON. N’y ajoutez pas ses images : son ZIP doit rester une sauvegarde séparée. Importer un JSON ne duplique pas le classeur local pointé par sa liaison.

## English

Edit `index.html`; no build step is required. French strings are keys in the `EN` dictionary. Static markup uses `data-i18n`; dynamic renderers call `tr()` explicitly. User content and tool identities are never translated. The hub language is independent from connected application languages.

`APPS` defines tools and URLs; `seed()` preserves native data contracts. Project tool order is stored in `project.apps`, and cover text in `project.imprint`. IndexedDB writes are queued; iframe navigation waits for tool saving. Preserve source-window, origin and session checks. Export schema versions remain independent from application versions. Keep Farde’s separate ZIP model intact.
