# Enchères Radar V2

Application web progressive (PWA) pour suivre et analyser des lots d'enchères dans une démarche d'achat-revente. Fonctionne sans backend, sans compte et sans abonnement. Les données sont stockées dans localStorage sur le téléphone.

## Fonctions
- Ajout, modification, suppression et favoris des lots
- Statuts, source, référence, date de fin, URL et notes
- Calcul du coût complet, du bénéfice, du ROI et de l'enchère maximale cible
- Score heuristique de priorisation (non prédictif)
- Recherche, filtres, classement
- Sauvegarde JSON, restauration JSON V1/V2, export CSV
- Service worker pour fonctionnement hors ligne après première visite
- Liens vers les plateformes (pas de collecte automatisée)

## Publication sur GitHub Pages depuis Android

Téléverser les fichiers **à la racine** du dépôt GitHub (pas le ZIP ni un sous-dossier), en remplaçant `index.html`, `app.js`, `sw.js`, `manifest.webmanifest`, `icon.svg`, `README.md`. Activer Settings > Pages > Deploy from branch > main > /(root). Puis recharger le site après publication. Sauvegarder les lots avant une modification importante.

## Limites
Pas de scraping, d'API externe, de surveillance automatique, de push garanti ou d'enchère automatique. L'évaluation de marché est fournie par l'utilisateur. Les résultats ne tiennent pas compte de la fiscalité, des coûts omis ou de la liquidité. Les données peuvent être perdues si le stockage du navigateur est effacé.
