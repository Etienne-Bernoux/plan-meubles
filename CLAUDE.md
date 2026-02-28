# Plan Meuble — Conventions projet

## Structure

```
plan-meuble/
├── index.html                    # Page d'accueil listant tous les meubles
├── CLAUDE.md                     # Ce fichier
├── <nom-du-meuble>/
│   ├── <nom>-3d.html             # Vue 3D interactive (Three.js)
│   └── plan-cote-<nom>.pdf       # Plan coté PDF (optionnel)
```

## Conventions de nommage

- Dossiers : `kebab-case`, pas d'accents, pas d'espaces → `meuble-cantiniere`
- HTML 3D : `<nom>-3d.html` (ex: `rangement-chutes-3d.html`)
- PDF plan : `plan-cote-<nom>.pdf`

## Stack technique — Vues 3D

- **Three.js** importé via CDN (fichier HTML unique, pas de build)
- Style : fond sombre (`#1a1a2e`), overlay info en haut à gauche, boutons de contrôle en bas
- Chaque HTML est autonome (pas de dépendance externe autre que Three.js CDN)
- Rotation / zoom interactif avec OrbitControls

## Workflow

1. Créer un dossier `nom-du-meuble/`
2. Y ajouter le fichier `*-3d.html` avec la vue Three.js
3. Y ajouter le PDF du plan coté si dispo
4. Mettre à jour `index.html` pour référencer le nouveau meuble

## Règles

- Pas de framework, pas de build step — HTML/CSS/JS pur
- Chaque meuble est indépendant (un dossier = un meuble)
- `index.html` est la seule page qui fait le lien entre tous les meubles
