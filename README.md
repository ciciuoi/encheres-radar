# Enchères Radar V1 — prototype PWA local

## Fonctions
- Saisie/modification/suppression de lots
- Coût complet, bénéfice prévisionnel, ROI, enchère maximale cible
- Score indicatif combinant ROI et confiance déclarée (non statistique)
- Filtres, tri, export JSON/CSV, import JSON
- Données enregistrées en localStorage sur le navigateur (pas de serveur)
- Mode hors ligne après mise en cache initiale par service worker

## Lancer sur ordinateur
Dans ce dossier : `python3 -m http.server 8000` puis ouvrir `http://localhost:8000`.

## Installer sur Android
Une PWA installable exige normalement HTTPS (ou localhost). Héberger les fichiers statiques sur un hébergement HTTPS gratuit compatible, puis ouvrir le lien dans Chrome Android et utiliser « Installer l'application » si proposé. Aucun serveur applicatif ni stockage distant des lots n'est nécessaire. Un simple fichier HTML ouvert depuis les fichiers Android permet parfois l'interface, mais pas une installation PWA fiable.

## Limites
Aucun robot de collecte ni estimation automatique de prix du marché dans cette V1. Pas de notifications périodiques. Le stockage localStorage peut être effacé par le navigateur. Sauvegardes JSON régulières recommandées. Frais de TVA/fiscalité et commissions spécifiques non modélisés séparément. Le score est heuristique et ne constitue pas une probabilité de gain.

## Formules
Coût total = enchère × (1 + frais acheteur / 100) + autres coûts + frais de revente.
Bénéfice estimé = prix de revente estimé − coût total.
ROI = bénéfice / coût total × 100 (0 affiché si coût nul).
Enchère max = max(0, (prix revente − autres coûts − frais revente − bénéfice cible)/(1 + frais acheteur / 100)).

## Évolution
Connecteurs aux sources de données autorisées, comparables de prix de revente réellement observés, alertes et scoring de liquidité/risque.
