# Portfolio de photographe

Site vitrine de démonstration construit avec Astro, HTML et CSS classique. Le contenu personnel et les photographies client restent à fournir : les placeholders et les images de démonstration sont signalés dans le site.

## Installation et commandes

Depuis PowerShell, placez-vous dans le dossier du projet et installez les
dépendances à partir du lockfile :

```powershell
npm ci
```

Lancez le serveur de développement :

```powershell
npm run dev
```

Ouvrez ensuite `http://localhost:4321/`. Pour construire le site puis prévisualiser
localement la version de production :

```powershell
npm run build
npm run preview
```

Si PowerShell bloque la commande `npm` à cause de sa politique d’exécution,
utilisez `npm.cmd` à la place pour chaque commande : `npm.cmd ci`,
`npm.cmd run dev`, `npm.cmd run build` et `npm.cmd run preview`.

## Structure

```text
src/
├── components/
│   ├── GalleryGrid.astro
│   ├── SiteFooter.astro
│   └── SiteHeader.astro
├── layouts/
│   └── SiteLayout.astro
├── pages/
│   ├── a-propos.astro
│   ├── contact.astro
│   ├── index.astro
│   └── portfolio/
│       ├── index.astro
│       ├── lifestyle.astro
│       ├── mode.astro
│       └── portraits.astro
└── styles/
    └── global.css
public/
└── images/
```

- `src/pages/` contient les pages et détermine les adresses du site.
- `src/layouts/SiteLayout.astro` fournit la structure HTML et les métadonnées communes.
- `src/components/` regroupe les éléments réutilisés ; `GalleryGrid.astro` affiche les séries et leur agrandissement natif.
- `src/styles/global.css` contient les styles, les règles responsive et les états de focus.
- `public/images/` contient les fichiers d’images servis tels quels.

## Contenu de démonstration et pistes d’adaptation

- Remplacer « Nom du photographe » et compléter la biographie, la ville et les coordonnées après validation.
- Remplacer les images de démonstration Unsplash par les photographies autorisées du client. Les listes d’images se trouvent dans les pages de série sous `src/pages/portfolio/`.
- La page Contact ne contient pas encore de formulaire actif. Il faudra choisir les coordonnées et, si un formulaire est souhaité, son service de traitement.
- Le dépôt Git est local ; aucun dépôt GitHub ni projet Vercel n’est configuré dans ce dépôt à ce stade.
