# Loto associatif - Écran projecteur

Application web statique (une seule page) pour afficher les numéros tirés pendant un loto associatif.

## Lancer l'application

1. Ouvrez directement `index.html` dans un navigateur.
2. Pour une diffusion en plein écran, utilisez le mode plein écran du navigateur (F11).

Aucun serveur ni dépendance n'est nécessaire.

## Modifier les logos partenaires

Les logos sont définis dans un tableau JavaScript en haut du script dans `index.html` :

```js
const logoFiles = [
  "assets/logos/logo-1.svg",
  "assets/logos/logo-2.svg",
  "assets/logos/logo-3.svg",
  "assets/logos/logo-4.svg"
];
```

Remplacez les fichiers dans `assets/logos/` ou mettez à jour la liste pour pointer vers vos propres logos.

## Raccourcis clavier

- **Chiffres + Entrée** : valider un numéro
- **Backspace** : annuler le dernier numéro
- **R** : réinitialiser la partie (confirmation)

## Persistance

Les numéros et événements sont sauvegardés automatiquement dans le `localStorage` du navigateur.
