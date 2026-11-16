# V3.1 — typologies et photographies de référence

Vérification du 16 novembre 2026. Cette évolution poursuit la PR nº 1 et ne modifie aucun calendrier horticole.

## Classement des treize familles

- **Feuillus** : Azalée satsuki, Charme, Chêne, Érables du Japon, Hêtre. La satsuki est explicitement présentée comme un feuillu persistant.
- **Conifères** : Chamaecyparis, Juniperus chinensis, Mélèzes, Pin blanc du Japon, Pin noir du Japon, Pin sylvestre. Le mélèze reste un conifère malgré son feuillage caduc.
- **Tropicaux** : Ficus, Tamarin.

Ordre français insensible aux accents à l’intérieur de chaque groupe. Bandeaux de groupes visibles dans le tableau annuel, y compris après filtrage ; titres maintenus dans la zone visible lors du défilement horizontal. Les listes de sélection suivent le même ordre. Les 118 lignes et les 1 416 états mensuels restent identiques.

## Photographies

Une photographie de référence apparaît au-dessus des résultats quand une famille précise est sélectionnée, dans les deux vues. Elle reste présente même si les autres filtres ne donnent aucune intervention. Aucune galerie pour « Toutes les familles ».

Treize photographies réelles, identifiées par espèce, vérifiées dans les fiches Wikimedia Commons et examinées visuellement. Le manifeste `photos-familles.json` conserve nom du fichier, espèce, auteur, licence, lien de licence, source et adresses externes sans jeton d’expiration. Les références des genres regroupant plusieurs espèces sont précisées dans la légende (ex. Carpinus betulus, Ficus microcarpa, Larix decidua). Pin blanc : Pinus parviflora, distinct de Pinus thunbergii. Tamarin : Tamarindus indica, collection du Morikami Museum. Aucun âge n’est inventé ; il s’agit de spécimens formés, pas de photographies des arbres personnels de l’utilisateur.

Les licences retenues sont CC BY-SA ou CC0. Chaque légende affiche le crédit et des liens vers la source et la licence. Images entières, sans recadrage, adaptées au conteneur, chargement différé et décodage asynchrone. En cas d’échec réseau, l’image disparaît et un message accessible conserve les liens vers sa source. Le calendrier reste utilisable hors connexion ; les photographies nécessitent une connexion et la disponibilité du tiers.

## Tests exécutés

- `node audit/verify.mjs` : syntaxe, intégrité des données, 1 344 combinaisons de filtres mensuels et 14 vues annuelles.
- `node audit/test-family-views.cjs` avec Playwright : Microsoft Edge / Chromium réel en mode headless, 1440 × 960, 390 × 844 et 320 × 740.
- Pour chaque largeur : trois groupes dans le bon ordre, treize familles triées, sélection des treize familles dans chacune des deux vues, maintien du filtre au retour d’une fiche, résultats vides, absence de débordement global, douze mois visibles sur PC.
- Chargement réel des treize photographies externes ; panne réseau forcée dans les deux vues ; absence de galerie sans sélection ; aucune erreur JavaScript.
- Captures PC et mobile inspectées visuellement. Aucun iPhone ou Safari physique testé.

Le script navigateur attend le serveur local sur `http://127.0.0.1:8765` (variable `BONSAI_BASE_URL` pour une autre adresse). Installer Playwright et son Chromium, ou définir `BROWSER_EXECUTABLE_PATH` pour un navigateur compatible déjà installé.

## Publication

PR conservée en brouillon sur sa branche de développement. Seule la copie de prévisualisation séparée, sous `/v3-1/` dans `calendrier-bonsai-preview-v3`, est mise à jour. Aucune fusion dans main, aucun déploiement ni changement de configuration du site principal.
