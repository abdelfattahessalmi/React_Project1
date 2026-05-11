# React_Project1
# ChatUI-Pro - NeoCare Medical Hub

## Description du projet et contexte NeoCare

Ce projet est une interface conversationnelle React realisee dans le cadre du module **Developper un chatbot avec React**.  
Le scenario se passe dans l'univers **NeoCare Medical Hub** (clinique connectee en 2031), avec **ARIA**, une assistante conversationnelle medicale.

L'application permet aux agents de:

- consulter un tableau de bord
- discuter avec ARIA dans un salon de chat
- personnaliser leur profil et leurs preferences

Toutes les reponses du chatbot sont **simulees localement** via un fichier mock (`src/data/responses.json`), sans appel API externe.

## Instructions d'installation et de lancement

### 1) Installer les dependances

```bash
npm install
```

### 2) Lancer le projet en developpement

```bash
npm run dev
```

Puis ouvrir l'URL locale affichee dans le terminal (exemple: `http://localhost:5173/` ou `http://localhost:5174/`).

### 3) Build de production (optionnel)

```bash
npm run build
```

## Description des choix techniques

- **React + Vite**: interface rapide, composants fonctionnels, experience de developpement fluide.
- **Redux Toolkit**: gestion centralisee de l'etat avec trois slices:
  - `messagesSlice`: historique des echanges et reinitialisation de conversation
  - `userSlice`: profil agent (nom + avatar)
  - `settingsSlice`: preferences utilisateur (mode sombre/clair)
- **React Router**: navigation entre les vues principales:
  - `/` -> Tableau de bord
  - `/chat` -> Salon de chat
  - `/settings` -> Parametres
  - `*` -> Page 404
- **Mock local JSON**: `src/data/responses.json` pour simuler les reponses d'ARIA avec delai de saisie.
- **UI/UX**:
  - design responsive mobile/desktop
  - focus visible pour l'accessibilite de base
  - interface 100% en francais
  - avatars SVG personnalises dans `src/assets/avatars/`

## Capture d'ecran / GIF de demonstration (optionnel)
!

```
