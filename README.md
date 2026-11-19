# Enchères Radar V5 — recherche configurable + swipe

Fonctionnel : swipe V4, données V1–V4 conservées, budget total 500 €, bénéfice prévisionnel minimal 100 €, stockage local, export et restauration JSON, import CSV/JSON, URLs HTTPS de flux CSV ou JSON accessibles en CORS, dédoublonnage, actualisation manuelle et automatique toutes les 15 minutes quand la page est ouverte.

**IMPORTANT** : aucun flux actif de plateforme n'est préconfiguré, faute d'API publique de lots actuels autorisée et vérifiée. Le logiciel ne scrape pas Interencheres, Drouot ou Domaine. Les boutons ouvrent des recherches sur ces sites. Le moteur automatique n'importe de vraies annonces que si l'utilisateur ajoute un flux autorisé et compatible navigateur. Les valeurs de revente manquantes sont mises « À estimer » et ne sont pas classées comme bonnes affaires. Même renseignée, la valeur de revente n'est pas vérifiée automatiquement.

Schéma JSON exemple : `[ {"name":"Perceuse X","bid":80,"category":"Outillage","source":"Flux autorisé","reference":"123","url":"https://exemple.fr/lot/123","fee":25,"fixed":10,"resale":10,"value":0} ]`. Pour une estimation documentée, renseigner `value` et les sources en `notes`. Les fichiers doivent être conformes aux règles d'usage du diffuseur et servir des entêtes CORS autorisant l'origine GitHub Pages.

Installation : sauvegarder ses données avec Réglages → Sauvegarder JSON ; remplacer les six fichiers de la racine du dépôt GitHub Pages. Vérifier Version 5.0 et recharger. Sans serveur, l'application ne recherche pas lorsque Chrome est fermé.

Tests : contrôle syntaxique de app.js, contrôle d'intégration navigateur Chromium et tests du connecteur par flux JSON simulé (voir rapport de test lors de la livraison).
