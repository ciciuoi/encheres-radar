# Enchères Radar V4 — mode swipe

Application PWA locale pour Android/Chrome. Préserve la clé `encheres-radar-v1-lots` de V1–V3.

## Mode Découvrir
- Glisser vers la droite ou appuyer sur ♥ pour garder (favoris + À surveiller).
- Glisser vers la gauche ou appuyer sur ✕ pour écarter.
- ↶ annule la dernière décision de la session.
- Fiche : coût total, prix d’enchère, valeur de revente supposée, bénéfice, ROI, prix maximal pour 100 € de gain.
- Filtre initial : coût total ≤ 500 € et bénéfice estimé ≥ 100 €. Bouton « Tout examiner » pour afficher le reste.
- Si aucune fiche, ajouter un lot, importer un fichier ou charger des exemples fictifs.

Les résultats reposent sur **les estimations saisies/importées**, pas sur une estimation automatique fiable des prix du marché. Pas de recherche automatisée sur des plateformes ni d'enchères placées automatiquement.

## Déploiement
Envoyer les six fichiers **à la racine** du dépôt GitHub Pages existant. Sauvegarder JSON avant remplacement. Le lien du site ne change pas. L'ancienne PWA peut afficher une version en cache : actualiser et vérifier le libellé 4.0.
