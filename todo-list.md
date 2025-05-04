# Todo List

## Le fichier index.html

- [x] Créer le fichier `index.html`

## Titre et meta-description

- [x] **Titre de la page** : Run – Bouge, respire, explore.
      _Entre 50 et 60 caractères_
- [x] **Meta-description** : Run est une invitation au mouvement, à l’exploration et à la reconnexion avec soi-même à travers chaque foulée.
      _Entre 150 et 160 caractères_

## Les favicons

- [x] **Préparer les favicons :**
  - [x] Une favicon en .SVG de 512x512 `favicon.svg`
  - [x] Un fichier .ICO avec 2 layers 16x16 et 32x32 `favicon.ico`
  - [x] Deux favicons en .PNG de 16x16 et 32x32 `favicon-16x16.png` et `favicon-32x32.png`
  - [x] Une apple-touch-icon en .PNG en 180x180 `apple-touch-icon.png`

## Les Open Graph réseaux sociaux

- [x] Titre de la page : Run - Le rythme de la liberté
      _Moins de 60 caractères_
- [x] Description de la page : Run est une ode au mouvement, à la nature et à l’élan intérieur. Prêt·e à avancer ?
      _Entre 120 et 140 caractères_
- [x] Image Open Graph en .PNG de 1200x630 `opengraph.png`

> On pourra utiliser le site [Opengraph](https://www.opengraph.xyz) pour générer les bonnes balises OpenGraph

## Traitement des images

- [x] Redimensionner, formatter et compresser les images utilisées sur le site
      _On pourra penser à faire différentes versions des images selon leur utilité_

**_Pour intégrer plusieurs versions d'une même image :_**

```html
<img
  srcset="./chemin/vers/image.webp, ./chemin/vers/image@2x.webp 2x"
  src="./chemin/vers/image.webp"
  alt="descriptif de l'image"
/>
```

> On pourra utiliser le site [Squoosh](https://squoosh.app/) pour générer des images en webp

- [x] Identifier les images à "preload"
- [x] Prévoir les icones en SVG si utilisation d'icones

> Si on intègre les icones avec <svg> et non avec <img>, on ajoutera un `aria-label:"description de l'icone"`

## La(les) polices

- [x] Télécharger la(les) polices
- [x] Lier celle(s)-ci au projet dans `settings.scss` par :

```scss
@font-face {
    font-family: "Nom-police";
    src: url(../chemin/vers/la/font.ttf)
    font-display: swap; //Pour éviter les décalages de mise en page
}
```

## La feuille de style .CSS

- [x] Créer le fichier `index.scss` et `_settings.scss`
- [x] Lier la page `_settings.scss` à l'`index.scss` par :

```scss
@import "./settings";
```

- [x] Lancer Watch Sass
- [x] Lier la feuille de style CSS au fichier HTML

## Structure de la page web

- [x] Réfléchir à la structure sémantique de la page web.
- [x] Définir les images les plus importantes (qui s'afficheront en premier) et les images qui sont cachées au chargement de la page. On "preload" les plus importantes, on fait un `loading="lazy"`

## Vérification de la sémantique

- [ ] Vérifier qu'il n'y a pas d'erreurs sémantiques dans le code.

> On pourra utiliser le site [Markup Validation service](https://validator.w3.org/)

## Vérification des performances

- [ ] Lancer un Audit Lighthouse

## Mise à jour du Readme.md

- [ ] Remplir les premières parties du Readme

## Commit & Push sur la manche "Main"

- [ ] Commit et Push les fichiers sur la branche principale "main"
