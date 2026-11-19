# Enchères Radar V3

Application PWA locale, déployable sur GitHub Pages.

## Critères
- Budget total maximal : 500 € (enchère + frais acheteur + frais fixes + frais de revente).
- Bénéfice estimé minimal : 100 €.
- La valeur de revente est une hypothèse à documenter, pas une estimation automatique.

## Détection de lots
Importer un CSV ou JSON de lots obtenu légalement, avec les colonnes du modèle téléchargeable dans l’onglet Sources. L’application déduplique les lots et classe les opportunités. Elle ne scrappe pas les sites d’enchères et ne fonctionne pas comme un robot de surveillance autonome.

## Déploiement Android
Remplacer les fichiers du dépôt GitHub Pages par ceux du ZIP. Rafraîchir Chrome. Exporter une sauvegarde JSON avant la mise à jour.

## Limites
Stockage localStorage propre au navigateur, risque de perte si données du site effacées. Aucun ordre d'enchère. Calculs indicatifs hors fiscalité et frais non renseignés.
