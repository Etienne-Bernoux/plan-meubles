# Meuble Cellier — Spécifications

## Objectif

Meuble de rangement pour cellier/garage en OSB 18mm sur roulettes. Trois zones : stockage vin en bas, rangement sec au milieu, espace grillagé anti-rongeurs en haut.

## Matériaux

- **OSB** : panneaux 2500 × 680 mm, épaisseur 18 mm
- **Roulettes** : 80 mm de haut
- **Grillage** : maille fine ≤ 6 mm, **largeur 400 mm** (type grillage à garde-manger)
- **Tasseaux** : chutes de bois ~30 × 30 mm

## Dimensions générales

- **Largeur totale** : 1350 mm
- **Profondeur** : 500 mm (découpé dans la largeur 680 mm de l'OSB)
- **Épaisseur OSB** : 18 mm (prise en compte dans tous les calculs ci-dessous)

### Empilage vertical (du sol vers le haut, côté droit)

| Élément | Épaisseur | Cumul depuis sol |
|---------|-----------|------------------|
| Roulettes | 80 mm | 0 → 80 |
| Plateau de base (OSB) | 18 mm | 80 → 98 |
| Zone vin (intérieur) | 482 mm | 98 → 580 |
| Séparation vin/sec (OSB) | 18 mm | 580 → 598 |
| Zone sec (intérieur) | 504 mm | 598 → 1102 |
| Séparation sec/grillagé (OSB) | 18 mm | 1102 → 1120 |
| Zone grillagée (intérieur droite) | 762 mm | 1120 → 1882 |
| Top panel droit (OSB) | 18 mm | 1882 → 1900 |

**Hauteur totale côté droit : 1900 mm** (= hauteur libre sous plafond)

### Empilage côté gauche

Identique jusqu'à la séparation sec/grillagé (1120 mm), puis :

| Élément | Épaisseur | Cumul depuis sol |
|---------|-----------|------------------|
| Zone grillagée (intérieur gauche) | 492 mm | 1120 → 1612 |
| Top panel gauche (OSB) | 18 mm | 1612 → 1630 |

**Hauteur totale côté gauche : 1630 mm** (= 20 mm sous le tuyau Ø120 mm, bas à 1650 mm)

### Contraintes tuyaux

#### Tuyau de plafond (force le décrochement)

- **Direction** : sort du mur du fond, vient vers l'avant (perpendiculaire au mur)
- **Hauteur bas du tuyau** : 1650 mm du sol, Ø 120 mm → centre à 1710 mm
- **Position latérale** : à partir de 750 mm depuis le bord droit, vers la gauche
- Le meuble ne peut pas dépasser 1630 mm de ce côté (20 mm de marge)

#### Évacuation WC (colonne verticale)

- **Direction** : verticale, descend du plafond
- **Entre dans le mur du fond à 900 mm du sol**
- **Section** : 200 × 200 mm
- **Position** : 950 mm depuis le bord droit du meuble
- **En dessous de 900 mm : libre** (pas de tuyau)
- **Réservation dans le panneau de fond** : fond en 2 pièces avec encoche
  - **Fond gauche** : 675 × 1550 mm, avec encoche rectangulaire de 200 mm (x=300→500) de 900 mm jusqu'en haut (scie plongeante)
  - **Fond droit** : 675 × 1550 mm, rectangle simple
  - Le tuyau remplit l'encoche, jeu résiduel comblé avec mousse ou grillage fin (anti-rongeurs)

## Zones — résumé

| Zone | Intérieur utile | Depuis sol | Description |
|------|----------------|------------|-------------|
| Vin (bas) | 482 mm | 98 → 580 | Tasseaux horizontaux, bouteilles 75cl couchées (~80 places) |
| Sec (milieu) | 504 mm | 598 → 1102 | Étagère ouverte (conserves, bocaux) |
| Grillagé droit | 762 mm | 1120 → 1882 | Porte grillagée anti-rongeurs + étagère |
| Grillagé gauche | 492 mm | 1120 → 1612 | Porte grillagée anti-rongeurs + étagère |

## Détail par zone

### Zone vin (bas) — 482 mm utile

- **Système tasseaux horizontaux** : paires de tasseaux 30×30mm espacés de 60mm (gap libre)
- Bouteilles 75cl : ~300 mm de long, ~75 mm de diamètre
- Les bouteilles se calent entre 2 tasseaux (Ø75 > gap 60 → la bouteille repose sur les bords)
- 2 rangées de tasseaux en profondeur (avant à ~380mm, arrière à ~60mm du fond) pour supporter chaque bouteille
- Largeur intérieure : 1350 - 2×18 = 1314 mm
- Pas de répétition vertical : 30 (tasseau) + 60 (gap) = 90 mm → 5 rangées dans 482 mm
- Bouteilles par rangée : 1314 / (75 + 10) ≈ **15 bouteilles**
- Total : **5 × 15 = 75 emplacements**
- Montants latéraux OSB pour visser les tasseaux

### Zone sec (milieu) — 504 mm utile

- Étagère horizontale en OSB 18mm
- 1 étagère (à 841 mm du sol) → 2 niveaux de rangement
- Hauteur par niveau : (504 - 18) / 2 ≈ **243 mm** (assez pour des bocaux/conserves)
- Étagère sur tasseaux vissés aux parois latérales
- La colonne d'évac WC traverse cette zone dans le fond (encoche 200 mm dans le panneau de fond)

### Zone grillagée (haut)

- **Droite** (762 mm utile) : 2 portes grillagées côte à côte + 2 étagères intérieures → 3 niveaux ~242 mm
- **Gauche** (492 mm utile) : 2 portes grillagées côte à côte + 1 étagère intérieure → 2 niveaux ~237 mm
- Portes : cadre bois avec grillage fin (maille ≤ 6 mm, lé de 400 mm), charnières et loquet simple
- **2 portes droites** : chaque ~342 mm × 762 mm (ouverture 714 mm ÷ 2, montant central tasseau 30 mm) → grillage 400 mm en 1 lé ✓
- **2 portes gauches** : chaque ~267 mm × 492 mm (ouverture 564 mm ÷ 2, montant central tasseau 30 mm) → grillage 400 mm en 1 lé ✓
- Total : **6 portes**, chacune couverte par un seul lé de grillage 400 mm
- Un panneau vertical (step panel) à 750 mm du bord droit sépare les deux sections

## Construction

- **Fixation** : tasseaux (chutes de bois) vissés sur les panneaux, puis panneaux vissés sur les tasseaux. Pas de vis dans la tranche de l'OSB, pas de colle.
- Panneaux latéraux pleine hauteur (1820 mm à droite, 1550 mm à gauche, hors roulettes)
- Panneau de fond : 2 pièces OSB 18mm de 675×1550mm. La pièce gauche a une encoche 200mm pour l'évac WC (scie plongeante). Le tuyau remplit l'encoche, jeu comblé en mousse/grillage fin
- Base : plateau OSB 18mm posé sur 4 roulettes (80 mm)
- Étagères posées sur tasseaux vissés aux panneaux latéraux
- Step panel : panneau vertical OSB à 750 mm du bord droit, du séparateur sec/grillagé au top

### Renforts structurels (tasseaux 30×30 mm)

- **Tasseau vertical au joint des 2 fonds** : à 675 mm du bord gauche, pleine hauteur, vissé sur les 2 panneaux de fond pour solidariser la jonction
- **Tasseau(x) horizontal(aux) au fond** : sous le séparateur sec/grillagé (portée 1314 mm) pour limiter la flèche — fixé au fond, le séparateur repose dessus

## Fichiers

- `spec-meuble-cellier.md` — ce fichier
- `meuble-cellier-3d.html` — vue 3D interactive
- `plan-cote-meuble-cellier.pdf` — plan coté (à venir)
