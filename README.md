# Notice Exploder

Application web autonome pour explorer une notice UNIMARC sous forme de visualisation radiale interactive.

## Utilisation

Ouvrir `notice-exploder.html` dans un navigateur. Aucune installation ni compilation nécessaire.

- Import texte UTF-8, MRK et MARCXML / MarcXchange.
- Chargement par ARK BnF via le service SRU (connexion Internet nécessaire).
- Navigation par bloc, champ, occurrence et sous-champ.
- Recherche, arbre, source brute et exports SVG / JSON.
- ISO2709 binaire non pris en charge.

## GitHub Pages

Dans Settings > Pages, sélectionner **Deploy from a branch**, branche **main**, dossier **/ (root)**, puis enregistrer.

Adresse prévue : https://didierthebault-web.github.io/notice-exploder/

`index.html` est la copie de l’application servie à la racine du site. `notice-exploder.html` reste le fichier autonome téléchargeable. Mettre les deux fichiers à jour ensemble.

## Données

Les fichiers importés et le texte collé sont traités localement. Le chargement par ARK contacte directement le service public de la BnF. Aucune correction automatique des valeurs sources.