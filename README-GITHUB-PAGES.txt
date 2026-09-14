POUR PUBLIER CE PROJET SUR GITHUB PAGES

1. N'utilisez PAS le bouton GitHub "Upload files" pour envoyer fichier par fichier.
2. Décompressez ce dossier.
3. Utilisez GitHub Desktop pour ajouter le dossier comme dépôt local.
4. Publiez-le sur votre dépôt GitHub avec la branche main.
5. Dans GitHub : Settings > Pages > Source : GitHub Actions.
6. Faites un push/commit sur main. L'action .github/workflows/deploy-pages.yml construira frontend avec npm run build et publiera frontend/build.

IMPORTANT : le backend Python n'est pas exécuté par GitHub Pages. Les fonctions qui appellent /api nécessitent un backend hébergé ailleurs et une variable REACT_APP_BACKEND_URL configurée pendant le build.
