# Vérification V3.1 — 16 novembre 2026

Six corrections intégrées sur la branche `audit/donnees-bonsai-reims-2026-11-16` de la PR nº 1. Aucune fusion ni publication sur le calendrier principal.

## Données et sources

- Pin blanc : neuf fiches réexaminées avec WP/WZ/WH dédiées à Pinus parviflora ; aucune référence générique EP/BP/HP ni transposition du mekiri. Rempotage mars/avril selon stade ; fin été supprimée du scénario par défaut. Taille lourde août à novembre conditionnelle, aucun optimum forcé. Greffe/marcotte sans calendrier suffisamment étayé.
- Structure lourde : treize familles réexaminées ; Juniperus fin février/début mars privilégié hors gel, selon Galinou p. 2. Le rapport distingue confirmation technique et confirmation de date. Chamaecyparis et tamarin restent sans optimum, pin blanc également après réaudit.
- Treize fiches d’exposition et de froid, références par famille ; rusticité de l’arbre distincte des racines en pot, repères adaptés à Reims et limites explicites.
- Rapport HTML et Markdown, données intégrées et fichier de traçabilité des 1 092 cases mis à jour.

## Contrôles

`node audit/verify.mjs` : réussite. 118 interventions, 1 416 états, 1 344 combinaisons mois/famille/période et 14 vues annuelles dans le DOM simulé. Syntaxe, couverture, références et égalité des données intégrées vérifiées.

Navigateur réel Chromium intégré, dimensions simulées : PC 1440 × 960 ; mobile 390 × 844 et 320 × 740. Aucun iPhone physique ni Safari testé.

- PC : douze mois simultanément visibles ; tableau de 1 249 px dans son conteneur de même largeur, colonne Famille 110 px. Symboles SVG visibles et identiques dans les deux vues.
- Juniperus filtré : février et mars affichent O ; ouverture de sa taille lourde affiche précautions et sources spécifiques.
- Retour depuis cette fiche : vue annuelle et filtre Juniperus restaurés, mois mensuel précédent Novembre restauré, focus sur la case d’origine.
- Mobile 390 px : fiche lisible, bouton Retour visible ; largeur de document 375 px, aucun débordement de page.
- Mobile 320 px : document 305 px ; tableau 940 px dans conteneur 250 px, défilement interne. Case Décembre du pin blanc accessible ; bonne fiche et retour vers le tableau filtré avec position horizontale restaurée.

## Prévisualisation

Adresse séparée prévue : `https://monsieurdeelah.github.io/calendrier-bonsai-preview-v3/v3-1/`. Sous-dossier autonome dans le dépôt de prévisualisation existant ; V3 et calendrier principal conservés. La publication et les derniers contrôles distants sont consignés après déploiement.
