# Español Flash — Application gratuite français ↔ espagnol

Español Flash est une **petite application web installable** (PWA). Aucun compte, aucune publicité, aucun serveur de données et aucun abonnement.

## Contenu

- `index.html` : application complète (HTML + CSS + JavaScript, sans bibliothèque externe).
- `manifest.webmanifest` : permet une ouverture en mode application.
- `sw.js` : met en cache les fichiers afin de pouvoir ouvrir l'application hors connexion **après une première ouverture en ligne**.
- `icon-192.png` et `icon-512.png` : icônes pour l'écran d'accueil.

## Tester sur ordinateur

Double-cliquer sur `index.html` ouvre l'application dans un navigateur. Les cartes, quiz et listes fonctionnent sans serveur. En mode `file://`, l'installation PWA et le service worker ne sont pas actifs.

## Installation sur iPhone avec GitHub Pages (gratuit)

1. Sur https://github.com/, créer un compte gratuit si nécessaire.
2. Créer un nouveau dépôt **Public** (par exemple `espanol-flash`).
3. Dans ce dépôt, cliquer sur **Add file** → **Upload files** et déposer **les 5 fichiers du dossier** (pas seulement le ZIP, ni un dossier parent).
4. Aller dans **Settings** → **Pages** ; sous **Build and deployment**, choisir **Deploy from a branch**, branche **main**, dossier **/(root)** ; enregistrer.
5. Ouvrir l'URL indiquée par GitHub Pages, généralement `https://VOTRE-PSEUDO.github.io/espanol-flash/`, sur l'iPhone dans **Safari**.
6. Dans Safari : **Partager** → **Sur l'écran d'accueil** → activer **Ouvrir comme app web** si proposé → **Ajouter**.
7. Ouvrir l'application depuis sa nouvelle icône au moins une fois **avec Internet** ; les fichiers sont ensuite mis en cache pour une utilisation hors ligne.

À noter : le dépôt GitHub public expose le code de l'application, **pas les listes ajoutées sur ton iPhone**. Les listes et résultats sont conservés dans le stockage local de chaque installation.

## Utilisation

- **Listes** : créer des listes, ajouter des mots, modifier, supprimer, coller plusieurs lignes `français ; espagnol`.
- **Réviser** : révéler la réponse et évaluer la difficulté ; l'application choisit une prochaine date de révision avec un algorithme simplifié (ce n'est pas l'algorithme exact d'Anki).
- **Quiz** : QCM et traduction à écrire, dans les deux sens.
- **Données** : exporter un fichier JSON ou restaurer une sauvegarde.
- **♪** : prononciation espagnole via la voix de l'appareil si disponible.

## Important — sauvegardes

**Les listes ne sont pas synchronisées entre appareils** et peuvent être perdues si l'application est supprimée ou que le stockage du site est effacé. Exporte régulièrement une sauvegarde JSON dans l'onglet « Données » et conserve-la dans Fichiers/iCloud Drive.

Le site doit être chargé via **HTTPS** pour profiter de l'installation en app et du cache hors connexion. Cette version n'utilise aucun service payant.
