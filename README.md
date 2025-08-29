# Séchilienne — Histoire vivante (GitHub Pages)

Ce paquet contient un `index.html` prêt à publier sur GitHub Pages (React via CDN, Tailwind, sans build) et un fichier `.nojekyll`.

## Publication via interface web (le plus simple)

1. Créez (ou ouvrez) votre dépôt sur GitHub.
2. Ajoutez **`index.html`** et **`.nojekyll`** à la **racine** du dépôt.
3. Allez dans **Settings → Pages** :
   - **Build and deployment** : *Deploy from a branch*.
   - **Branch** : `main` (ou `master`) **/** `root` (pas `/docs`).
   - Enregistrez. L’URL s’affiche une fois le déploiement terminé.
4. Ouvrez l’URL indiquée (ex. `https://votre-identifiant.github.io/nom-du-repo/`).

> Astuce : si vous préférez publier depuis `/docs`, placez ces fichiers dans un dossier `docs/`, puis sélectionnez `main / /docs` dans Settings → Pages.

## Publication par ligne de commande

```bash
git add index.html .nojekyll
git commit -m "Publish Séchilienne — Histoire vivante"
git push
# Puis Settings → Pages : main / root
```

## Personnalisation

Dans `index.html`, remplacez les tableaux `EVENTS`, `PLACES`, `FAMILIES`, `INDUSTRIES`, `MEMOIRE44` par vos contenus validés. 
Pour une vraie carte, remplacez le placeholder par Leaflet/MapLibre.
