# Meuble Cellier — Spécifications

## Objectif

Meuble de rangement pour cellier/garage en OSB 18mm sur roulettes. Trois zones : stockage vin en bas, rangement sec au milieu, espace grillagé anti-rongeurs en haut.

## Matériaux

- **OSB** : panneaux 2500 × 680 mm, épaisseur 18 mm
- **Roulettes** : 80 mm de haut
- **Grillage** : maille fine ≤ 6 mm, **largeur 400 mm** (type grillage à garde-manger)
- **Tasseaux** : chutes de bois ~30 × 30 mm

## Dimensions générales

- **Largeur totale** : 1200 mm
- **Profondeur** : 500 mm (découpé dans la largeur 680 mm de l'OSB)
- **Épaisseur OSB** : 18 mm (prise en compte dans tous les calculs ci-dessous)

### Empilage vertical (du sol vers le haut, côté droit)

| Élément | Épaisseur | Cumul depuis sol |
|---------|-----------|------------------|
| Roulettes | 80 mm | 0 → 80 |
| Plateau de base (OSB) | 18 mm | 80 → 98 |
| Zone vin (intérieur) | 482 mm | 98 → 580 |
| Séparation vin/sec (OSB) | 18 mm | 580 → 598 |
| Zone sec (intérieur) | 764 mm | 598 → 1362 |
| Séparation sec/grillagé (OSB) | 18 mm | 1362 → 1380 |
| Zone grillagée (intérieur droite) | 502 mm | 1380 → 1882 |
| Top panel droit (OSB) | 18 mm | 1882 → 1900 |

**Hauteur totale côté droit : 1900 mm** (= hauteur libre sous plafond)

### Empilage côté gauche

Identique jusqu'à la séparation sec/grillagé (1380 mm), puis :

| Élément | Épaisseur | Cumul depuis sol |
|---------|-----------|------------------|
| Zone grillagée (intérieur gauche) | 302 mm | 1380 → 1682 |
| Top panel gauche (OSB) | 18 mm | 1682 → 1700 |

**Hauteur totale côté gauche : 1700 mm** (= hauteur sous le tuyau)

### Contraintes tuyaux

#### Tuyau de plafond (force le décrochement)

- **Direction** : sort du mur du fond, vient vers l'avant (perpendiculaire au mur)
- **Hauteur** : 1700 mm du sol
- **Position latérale** : à partir de 750 mm depuis le bord droit, vers la gauche
- Le meuble ne peut pas dépasser 1700 mm de ce côté

#### Évacuation WC (colonne verticale)

- **Direction** : verticale, descend du plafond
- **Entre dans le mur du fond à 900 mm du sol**
- **Section** : 200 × 200 mm
- **Position** : 950 mm depuis le bord droit du meuble
- **En dessous de 900 mm : libre** (pas de tuyau)
- **Réservation dans le panneau de fond** : encoche de 200 mm de large, partant du haut du panneau et descendant jusqu'à 900 mm du sol (soit 820 mm depuis le dessus du plateau de base)

## Zones — résumé

| Zone | Intérieur utile | Depuis sol | Description |
|------|----------------|------------|-------------|
| Vin (bas) | 482 mm | 98 → 580 | Casiers pour bouteilles 75cl couchées |
| Sec (milieu) | 764 mm | 598 → 1362 | Étagères ouvertes (conserves, bocaux) |
| Grillagé droit | 502 mm | 1380 → 1882 | Porte grillagée anti-rongeurs |
| Grillagé gauche | 302 mm | 1380 → 1682 | Porte grillagée anti-rongeurs |

## Détail par zone

### Zone vin (bas) — 482 mm utile

- Casiers en grille (diviseurs verticaux + horizontaux) en OSB 18mm
- Bouteilles 75cl : ~300 mm de long, ~75 mm de diamètre
- Largeur intérieure : 1200 - 2×18 = 1164 mm
- Profondeur intérieure : 500 - 18 (fond) = 482 mm (pas de panneau devant)
- Grille : 10 colonnes (~116 mm) × 4 rangées (~120 mm)
- Total : **40 emplacements**, les bouteilles de 300 mm passent largement en profondeur

### Zone sec (milieu) — 764 mm utile

- Étagères horizontales en OSB 18mm
- 2 étagères → 3 niveaux de rangement
- Hauteur par niveau : (764 - 2×18) / 3 ≈ **243 mm** (assez pour des bocaux/conserves)
- Étagères sur tasseaux vissés aux parois latérales
- La colonne d'évac WC traverse cette zone dans le fond (encoche 200 mm dans le panneau de fond)

### Zone grillagée (haut)

- **Droite** (502 mm utile) : porte grillagée + 1 étagère intérieure
- **Gauche** (302 mm utile) : porte grillagée seule (trop basse pour une étagère)
- Portes : cadre OSB avec grillage fin (maille ≤ 6 mm, lé de 400 mm), charnières et loquet simple
- **Porte droite** (~714 mm large) : montant central dans le cadre → 2 lés de grillage
- **Porte gauche** (~432 mm large) : 1 seul lé de grillage suffit
- Un panneau vertical (step panel) à 750 mm du bord droit sépare les deux sections

## Construction

- **Fixation** : tasseaux (chutes de bois) vissés sur les panneaux, puis panneaux vissés sur les tasseaux. Pas de vis dans la tranche de l'OSB, pas de colle.
- Panneaux latéraux pleine hauteur (1820 mm à droite, 1620 mm à gauche, hors roulettes)
- Panneau de fond : OSB 18mm, pleine largeur, avec encoche 200 mm pour l'évac WC
- Base : plateau OSB 18mm posé sur 4 roulettes (80 mm)
- Étagères posées sur tasseaux vissés aux panneaux latéraux
- Step panel : panneau vertical OSB à 750 mm du bord droit, du séparateur sec/grillagé au top

## Fichiers

- `spec-meuble-cellier.md` — ce fichier
- `meuble-cellier-3d.html` — vue 3D interactive
- `plan-cote-meuble-cellier.pdf` — plan coté (à venir)
