# Filtre annuel par intervention — 16 novembre 2026

Ajout de « Type d’intervention » dans la vue annuelle, combinable avec Famille. « Toutes les interventions » rétablit les lignes de la famille choisie. Les sélecteurs gardent toutes leurs options ; un croisement vide affiche un message explicite. Les 12 mois et tous leurs états sont conservés, y compris non applicable, déconseillé et non documenté.

Les types stables regroupent les variantes de taille d’entretien et de pincement/sélection des pousses sans comparaison exacte des libellés. Le désaiguillage, la défoliation, l’éclaircissage et la suppression des fleurs ont des types distincts ; le mekiri reste distinct du pincement. Aucun changement des 118 lignes de données, précautions ou photos. Les libellés spécifiques restent visibles dans les lignes et fiches.

Validation : node audit/verify.mjs réussit (1 344 combinaisons mensuelles, 196 combinaisons annuelles famille × type, contrôle du nombre de lignes et des 12 états par ligne, cas vide, couverture de 13 familles pour rempotage et pincement, mekiri limité à sa ligne existante).

Navigateur intégré, largeurs 1440, 390 et 320 px : rempotage = 13 lignes / 156 cellules ; 12 mois ; aucun débordement de page ; tableau intégral visible sur PC et défilement interne sur mobile. Croisement Tamarin + Rempotage, ouverture de fiche puis Retour : famille, intervention et photo préservées. Tamarin + Mekiri : message vide. Retour à Toutes les interventions : 9 lignes Tamarin. Variantes de pincement et désaiguillage vérifiées, mekiri séparé. Aucune erreur JavaScript observée. Captures PC et mobile jointes. Mobile émulé, aucun appareil physique testé.

La PR reste en brouillon. Seule la prévisualisation /v3-1/ du dépôt calendrier-bonsai-preview-v3 doit être actualisée ; aucun changement de main ni publication du calendrier principal.
