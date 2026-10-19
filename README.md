# classinus-updates-pc

Dépôt public qui héberge les installeurs Windows de l'appli PC de Classinus. L'appli installée y lit les releases pour se mettre à jour toute seule.

Il ne contient aucun code source de l'appli, seulement les releases : un fichier `Classinus-Setup-X.Y.Z.exe` par version, avec les fichiers de description qu'electron-updater lit (`latest.yml` et l'empreinte de vérification).

Rien ne se modifie à la main ici. Tout est publié automatiquement par le workflow `.github/workflows/publier-pc.yml` du dépôt `classinus-frontend`, quand une étiquette `pc-vX.Y.Z` est poussée sur un commit de `main`.

Ce dépôt est indépendant de `classinus-updates`, qui sert les mises à jour de l'appli Android.
