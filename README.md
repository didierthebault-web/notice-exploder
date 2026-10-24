# Notice Exploder

Application web autonome pour explorer une notice UNIMARC sous forme de visualisation radiale interactive.

## Utilisation

Ouvrir `notice-exploder.html` dans un navigateur. Aucune installation ni compilation nécessaire.

- Import texte UTF-8, MRK et MARCXML / MarcXchange.
- Chargement par ARK BnF via le service SRU (connexion Internet nécessaire).
- Navigation par bloc, champ, occurrence et sous-champ.
- Recherche, arbre, source brute et exports SVG / JSON.
- Import ISO2709 UTF-8 (.mrc, .iso2709, .iso, .marc), y compris plusieurs notices. Validation du guide, du répertoire et des terminateurs. Les encodages historiques ISO 5426 / MARC-8 ne sont pas décodés : réexporter en UTF-8.

## GitHub Pages

Dans Settings > Pages, sélectionner **Deploy from a branch**, branche **main**, dossier **/ (root)**, puis enregistrer.

Adresse prévue : https://didierthebault-web.github.io/notice-exploder/

`index.html` est la copie de l’application servie à la racine du site. `notice-exploder.html` reste le fichier autonome téléchargeable. Mettre les deux fichiers à jour ensemble.

## Données

Les fichiers importés et le texte collé sont traités localement. Le chargement par ARK contacte directement le service public de la BnF. Aucune correction automatique des valeurs sources. Les octets ISO2709 originaux sont conservés en base64 dans le JSON et téléchargeables à l’identique dans la vue Notice brute. Les marqueurs de non-tri restent dans les valeurs sources ; seul le titre de présentation les masque avec un libellé explicite. La vue brute rend visibles les séparateurs binaires. Aucun fichier de données utilisateur n’est inclus dans ce dépôt.