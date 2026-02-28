# Plan Meuble — Conventions projet

## Structure

```
plan-meuble/
├── index.html                    # Page d'accueil listant tous les meubles
├── CLAUDE.md                     # Ce fichier
├── <nom-du-meuble>/
│   ├── spec-<nom>.md             # Spécifications du meuble
│   ├── <nom>-3d.html             # Vue 3D interactive (Three.js)
│   └── plan-cote-<nom>.pdf       # Plan coté PDF (optionnel)
```

## Conventions de nommage

- Dossiers : `kebab-case`, pas d'accents, pas d'espaces → `meuble-cantiniere`
- Spec : `spec-<nom>.md`
- HTML 3D : `<nom>-3d.html` (ex: `rangement-chutes-3d.html`)
- PDF plan : `plan-cote-<nom>.pdf`

## Stack technique — Vues 3D

- **Three.js** importé via CDN (fichier HTML unique, pas de build)
- **OrbitControls** via CDN (`three@0.128.0/examples/js/controls/OrbitControls.js`)
- Style : fond sombre (`#1a1a2e`), overlay info en haut à gauche, boutons de contrôle en bas
- Chaque HTML est autonome (pas de dépendance externe autre que Three.js CDN)
- Rotation / zoom interactif avec OrbitControls
- **Bouton « Stopper rotation »** obligatoire sur chaque vue 3D (toggle auto-rotate)

## Workflow par meuble

1. Rédiger la spec `spec-<nom>.md` (dimensions, contraintes, zones)
2. **Valider la spec** avant de passer au HTML 3D
3. Créer le dossier `nom-du-meuble/`
4. Y ajouter le fichier `*-3d.html` avec la vue Three.js
5. Y ajouter le PDF du plan coté si dispo
6. Mettre à jour `index.html` pour référencer le nouveau meuble

### Rigueur dans les specs

- **Toujours compter l'épaisseur de l'OSB** (18 mm) dans les empilages verticaux et horizontaux
- **Toujours compter les roulettes** dans la hauteur totale depuis le sol
- Présenter un **tableau d'empilage** (du sol vers le haut) avec épaisseur et cumul pour chaque élément
- Les hauteurs utiles (intérieur) = hauteur de zone − épaisseurs des séparations OSB
- Ne pas lancer la modélisation 3D tant que la spec n'est pas validée et complète
- La spec est la **source de vérité** : le HTML 3D doit la respecter à la lettre

## Méthode de construction

- **Matériau principal** : OSB 18mm (panneaux 2500 × 680 mm)
- **Fixation** : tasseaux (chutes de bois) vissés sur les panneaux, puis panneaux vissés sur les tasseaux. Pas de vis dans la tranche de l'OSB, pas de colle.
- Les étagères reposent sur des tasseaux vissés aux panneaux latéraux

## Outillage disponible

- Scie sauteuse
- Scie à onglet
- Scie plongeante (+ rail de guidage)
- Défonceuse

## Règles

- Pas de framework, pas de build step — HTML/CSS/JS pur
- Chaque meuble est indépendant (un dossier = un meuble)
- `index.html` est la seule page qui fait le lien entre tous les meubles
