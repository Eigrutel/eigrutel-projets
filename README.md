# Projets — Eigrutel Lab

Un espace pour retrouver les outils Eigrutel Lab autour d’un même projet de bande dessinée.

**Version : 0.12.0 · 11 septembre 2026**  
Conçu et développé par **Simon Léturgie**, dans le cadre d’Eigrutel BD Academy.

[Ouvrir Projets](https://eigrutel.github.io/eigrutel-projets/) · [Notice FR/EN](NOTICE.md) · [Logithèque](https://www.stripmee.com/logitheque/) · [Soutenir le développement](https://fr.tipeee.com/leturgie/)

L’adresse d’ouverture ci-dessus est celle prévue après activation de GitHub Pages sur ce dépôt. Les liaisons doivent encore être vérifiées sur cette publication.

## Fonctionnement

Créez un projet, choisissez ses outils et passez de l’un à l’autre dans le même espace. Les outils raccordés reçoivent leurs données à l’ouverture et transmettent leurs modifications à Projets.

- Bibliothèque de projets présentés comme des couvertures, avec image et couleur personnalisables.
- Navigation latérale repliable, adaptée aux petits écrans.
- Sauvegarde locale, import et export des projets en JSON.
- Import/export JSON individuel pour les outils compatibles.
- Farde liée à un classeur local distinct, avec sauvegarde ZIP séparée.

L’interface de Projets est actuellement en français. Les applications conservent leurs propres options de langue.

## Applications

| Application | Fonctionnement dans Projets |
| --- | --- |
| [Personnages](https://eigrutel.github.io/eigrutel-personnages/) | Données et portraits inclus dans le JSON du projet |
| [Boussole](https://eigrutel.github.io/eigrutel-boussole/) | Données incluses dans le JSON du projet |
| [Univers](https://eigrutel.github.io/eigrutel-univers/) | Données incluses dans le JSON du projet |
| [Scénoscope](https://eigrutel.github.io/eigrutel-scenoscope/) | Données incluses dans le JSON du projet |
| [Comic Script](https://eigrutel.github.io/eigrutel-comic-script/) | Données incluses dans le JSON du projet |
| [7 Questions](https://eigrutel.github.io/eigrutel-7questions/) | Données incluses dans le JSON du projet |
| [Pop!](https://eigrutel.github.io/eigrutel-pop/) | Données incluses dans le JSON du projet |
| [WIP](https://eigrutel.github.io/eigrutel-wip/) | Données et réglages du calculateur inclus dans le JSON du projet |
| [Farde](https://eigrutel.github.io/eigrutel-farde/) | Liaison locale uniquement ; fiches et images sauvegardées séparément en ZIP |
| [Narratopedia](https://eigrutel.github.io/eigrutel-narratopedia/narratopedia.html) | Consultation directe, sans données enregistrées par Projets |

Flash, References et Chrono ne sont plus proposés comme outils de projet. Les anciens exports contenant ces identifiants restent acceptés.

## Sauvegardes

**ZIP SÉPARÉ — PENSER À ENREGISTRER LE ZIP FARDE !**

Le JSON global ne contient ni les fiches ni les images de Farde. Pour conserver un projet complet utilisant Farde, gardez **son JSON Projets et son ZIP Farde à jour**.

Les données de travail restent dans le navigateur. Il n’y a ni compte, ni synchronisation entre appareils, ni sauvegarde des projets sur GitHub. Un changement de navigateur, d’adresse ou l’effacement des données du site peut rendre ces données indisponibles. Exportez vos copies avant une migration.

Un projet utilisant plusieurs outils est prévu pour circuler entre applications dans le même navigateur. Il ne fournit pas d’édition collaborative simultanée ; l’échange de fichiers nécessite de coordonner les versions entre personnes.

## Installation et publication

Aucune compilation, aucun gestionnaire de paquets, aucun serveur applicatif n’est requis. Voir [DEPLOIEMENT.md](DEPLOIEMENT.md) pour la publication GitHub Pages et les vérifications.

Cette version pointe vers les applications publiées sous `https://eigrutel.github.io`. Projets doit être servi sous cette même origine pour que les liaisons fonctionnent. Un autre chemin de dépôt est possible ; une autre origine nécessite de revoir l’hébergement et les adresses des applications.

## Contenu du dépôt

| Fichier | Rôle |
| --- | --- |
| `index.html` | Application complète : HTML, CSS et JavaScript ; favicons intégrés |
| `projets.html` | Redirection vers l’application pour conserver ce nom de lien |
| `NOTICE.md` | Utilisation, sauvegarde, transfert et dépannage FR/EN |
| `DEPLOIEMENT.md` | Publication GitHub Pages et vérifications FR/EN |
| `CHANGELOG.md` | Historique des versions |
| `RELEASE_NOTES.md` | Texte préparé pour la version 0.12.0 |
| `LICENSE` | Texte intégral GNU AGPL v3 |
| `LICENSE-DOCS.txt` | Texte intégral CC BY-SA 4.0 |
| `TRADEMARKS.md` | Marques, logos et signes distinctifs |
| `CONTRIBUTING.md` | Contributions et signalements |
| `.nojekyll` | Publication statique sans traitement Jekyll |

## Licences et crédits

Copyright © 2026 Simon Léturgie.

- **Code : GNU AGPL v3.0 ou version ultérieure** — [LICENSE](LICENSE).
- **Documentation et modèles : CC BY-SA 4.0**, sauf mention contraire — [LICENSE-DOCS.txt](LICENSE-DOCS.txt).
- **Marques et logos Eigrutel réservés** — [TRADEMARKS.md](TRADEMARKS.md).

Les contenus importés par les utilisateurs ne sont pas placés sous ces licences du seul fait de leur import. Les autres applications restent distribuées dans leurs propres dépôts avec leurs mentions et licences respectives.

---

## English

**Projets** brings Eigrutel Lab tools together within a comic-book project. Create a project, select its tools and switch between them without manually reloading each tool’s JSON file.

Project covers and accent colours are customisable. The navigation panel can be collapsed. The hub currently uses a French interface; individual tools retain their own language options.

Project data is stored locally in the browser, with no account or automatic cross-device synchronisation. Export JSON backups regularly. **Farde remains separate: its images and cards are not included in the project JSON. Keep an up-to-date Farde ZIP alongside that JSON.** Narratopedia is a consultation tool without project data saving.

This repository contains the hub only. Linked applications remain in their own repositories. The current configuration requires the hub and connected tools to share the `https://eigrutel.github.io` origin. Opening the hub as a local file does not provide the complete connected workflow.

Read [NOTICE.md](NOTICE.md) for usage and backups, and [DEPLOIEMENT.md](DEPLOIEMENT.md) for publishing. The GitHub integration still needs a final published-site check before a stable release.

Code: **GNU AGPL v3.0 or later**. Documentation and templates: **CC BY-SA 4.0**, unless otherwise stated. Eigrutel trademarks and logos are reserved. User-imported content retains its own rights.
