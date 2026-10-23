# PROJET — Compteur +1

## Description
Web app installable (PWA simplifiée) : un compteur qui s'incrémente à chaque appui. Demande initiale d'Alexis : compter sur les boutons de volume physiques de l'iPhone.

## Décisions
- **2026-10-23** — Limite constatée et vérifiée : iOS n'expose aucun événement volume au navigateur ; interception des boutons physiques impossible en web. Substitut retenu : écran entier tactile = +1 ; touches Volume du clavier (desktop) = +1. Alternative native (Swift, `AVAudioSession`) documentée mais hors périmètre web.
- **2026-10-23** — Fichier unique `index.html`, zéro dépendance, zéro build. Priorité : performance et simplicité maximales.
- **2026-10-23** — Persistance localStorage (`compteur-valeur`), retour haptique `navigator.vibrate` (Android/Chrome), safe-area iOS gérée (`viewport-fit=cover`, `env(safe-area-inset-bottom)`).

## État
- ✅ v1 — compteur, −1, reset, persistance, installation écran d'accueil iOS

## Améliorations possibles (backlog)
- Hébergement GitHub Pages pour un lien d'installation direct
- Service worker + manifest pour PWA complète (offline + install Chrome Android)
- Historique / compteur multi-jours

## Audit / Changelog
- **2026-10-23** — v1 livrée (Ada), review Alexis en attente. Push initial sur `main`.
