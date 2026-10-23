# Compteur +1

Web app minimaliste : un compteur qui s'incrémente d'un coup à chaque appui.

## Utilisation
- **Tap n'importe où sur l'écran** : +1 (tout l'écran est le bouton)
- **Touches Volume + / −** au clavier (desktop) : +1
- **−1** et **Remettre à zéro** : boutons en bas
- Compteur **persistant** (localStorage)

## Installation sur iPhone
1. Ouvrir `index.html` hébergé (ou via GitHub Pages)
2. Safari → Partager → **« Sur l'écran d'accueil »**
3. S'ouvre en plein écran, sans barre de navigateur

> ⚠️ **Limite connue** : iOS n'expose pas les boutons de volume physiques au navigateur — aucune web app ne peut les intercepter. Le tap plein écran est le substitut ; les touches Volume d'un clavier fonctionnent elles.

## Structure
- `index.html` — l'application complète, fichier unique, zéro dépendance (~5 Ko)

## Fichier-projet
Voir `PROJET.md` — source de vérité du chantier (règle de l'atelier).
