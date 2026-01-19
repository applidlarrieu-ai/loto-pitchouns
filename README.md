# Loto associatif - Écran projecteur & console opérateur

Application web statique en deux pages :

- `operator.html` : page opérateur (saisie des numéros + annonces).
- `index.html` : page d'affichage pour le projecteur (lecture seule, avec logos partenaires).

## Lancer l'application

1. Ouvrez `operator.html` sur l'ordinateur de l'animateur.
2. Ouvrez `index.html` sur l'écran de projection (ou un second onglet).
3. Pour une diffusion en plein écran, utilisez le mode plein écran du navigateur (F11).

Aucun serveur ni dépendance n'est nécessaire. Les deux pages communiquent via le `localStorage` du navigateur.

## Modifier les logos partenaires

Les logos sont définis dans un tableau JavaScript en haut du script de la page `index.html` (affichage projecteur) :

```js
const logoFiles = [
  "assets/logos/logo-1.svg",
  "assets/logos/logo-2.svg",
  "assets/logos/logo-3.svg",
  "assets/logos/logo-4.svg"
];
```

Remplacez les fichiers dans `assets/logos/` ou mettez à jour la liste pour pointer vers vos propres logos.

## Raccourcis clavier (page opérateur)

- **Chiffres + Entrée** : valider un numéro
- **Backspace** : annuler le dernier numéro
- **R** : réinitialiser la partie (confirmation)

## Persistance

Les numéros et événements sont sauvegardés automatiquement dans le `localStorage` du navigateur.
