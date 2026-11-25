# Rotuleo — Design system

## Brand overview
Rotuleo vend une orthèse rotulienne (sangle sous la rotule) pour les douleurs du genou. Public : seniors actifs, randonneurs, sportifs, personnes qui veulent remarcher sans appréhension. Trafic majoritairement mobile (pubs Meta). Le site doit inspirer crédibilité, confiance, efficacité, simplicité : une vraie marque d'orthopédie moderne, pas une boutique générique.

## Design thesis
La précision, pas la pression : une interface aussi ciblée que le produit — une couleur de marque, une couleur d'action, beaucoup d'air, rien qui ne serve pas la décision d'achat.

## Colors
| Nom | Valeur | Token | Rôle |
|---|---|---|---|
| Marine | #0D2E57 | --rt-navy / secondary_button_background | Marque : titres, offre sélectionnée, bandeaux, colonne Rotuleo du comparatif, pied de page |
| Turquoise | #1BB0C9 | --rt-teal / primary_button_background | Action uniquement : boutons d'achat (texte marine), icônes sur fond marine |
| Turquoise encre | #0A7A8E | --rt-teal-ink | Icônes « check », économies, texte turquoise sur fond clair (contraste ≥ 4,5:1) |
| Turquoise doux | #E7F6F9 | --rt-teal-soft | Cadeaux inclus dans l'offre sélectionnée |
| Encre | #111111 | text_color | Texte courant (noir foncé) |
| Encre secondaire | #1F2329 | --rt-ink-2 | Sous-titres, mentions (jamais de gris clair) |
| Fond | #FFFFFF | background | Fond de page |
| Turquoise clair | #E8F5F8 | --rt-tint | Bandes alternées (bénéfices, avis, mode d'emploi, FAQ) |
| Surface | #FFFFFF | --rt-surface | Bandes blanches (logos, bénéfices, avis, mode d'emploi), cartes FAQ |
| Ligne | #DCE3EC | --rt-line | Séparateurs, bordures |
| Rouge | #C8372D | --rt-danger | Négatif uniquement (✗ du comparatif) |
| Étoiles | #F2B01E | --rt-star | Notes uniquement |

## Typography
- Archivo 700 (titres), Archivo 400 (texte), réglages du thème (`heading_font`, `text_font`).
- Texte : 16 px mobile, 17 px ordinateur, interlignage 1,5–1,65 dans les blocs longs.
- Titres : interlignage 1,05–1,1, lettrage −1, casse phrase. Majuscules réservées aux petites étiquettes (barre d'annonce, « Vu sur ») avec lettrage élargi.

## Spacing and composition
- Rayon : boutons 12 px, cartes 14–16 px, champs 10 px. Aucune ombre portée (block_shadow_opacity 0).
- Rythme des sections : fond gris / bandes blanches / un seul bandeau marine (garantie).
- Mobile d'abord : bloc d'achat visible sans détour, cibles tactiles ≥ 48 px, bouton d'achat 58 px.

## Components
- Bouton principal : fond turquoise, texte marine 700, rayon 12 px.
- Bouton secondaire : fond marine, texte blanc.
- Bloc d'achat : note + preuve sociale → titre → points clés (2 colonnes) → offre limitée (vraie date de fin, se masque seule) → offres Kaching → bouton → réassurance 3 icônes + moyens de paiement → accordéons.
- Offres Kaching : cartes blanches, bordure #C9D3DF, sélection marine, cadeaux en turquoise doux.
- Sections Rotuleo : rt-benefits, rt-media-text, rt-comparison, rt-steps.

## Dos and Don'ts
- Do : une seule couleur d'action (turquoise) ; le marine porte la marque.
- Do : preuves sociales et urgence réelles et vérifiables uniquement.
- Don't : promesses médicales non démontrées, faux stocks, faux compteurs.
- Don't : dégradés décoratifs, ombres lourdes, badges sans fonction.

## Motion philosophy
Quasi aucune : pas d'animation d'apparition des titres, pas de transition de page. Seules animations : défilement de la barre d'annonce et compte à rebours de l'offre.

## Structure de la page produit (playbook ECC)
1 Hero promesse (image lifestyle, titre bénéfice, sous-titre promesse, sans bouton) · 2 Vu sur (logos en couleur) · 3 Bénéfices · 4 Comparatif (contraste, remplace l'avant/après) · 5 Avis clients · 6 Bloc d'achat = SEUL bouton d'achat de la page · 7 Mode d'emploi puis arguments (force, genouillère, anti-glisse, 10 h) · garantie · 9 FAQ · 10 Contact · 11 Pied de page (liens légaux + SAV).
Règle : aucun bouton d'achat hors du bloc d'achat (barre fixe désactivée).
