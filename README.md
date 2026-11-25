# Mon Étable — première version

Application web installable (PWA) pour gérer les bâtiments, les cases et les bovins.

## Fonctionnalités
- Ajouter/modifier/supprimer des bâtiments et des cases.
- Définir la capacité de chaque case.
- Enregistrer vaches et veaux avec un identifiant de **4 chiffres** (les zéros initiaux sont conservés).
- Liste distincte des vaches et des veaux.
- Veaux indépendants ou associés à une mère.
- Recherche par numéro, déplacement entre cases d'un même bâtiment.
- Compteurs automatiques et indicateur de case pleine.
- Export/import d'une sauvegarde JSON.
- Enregistrement local sur l'appareil et mise en cache pour le mode hors connexion.

## Démarrage rapide
Ouvre `index.html` dans un navigateur pour tester l'application. Les données restent dans le stockage local de ce navigateur.

## Installation sur téléphone et mode hors connexion
Pour installer la PWA et activer correctement le service worker, les fichiers doivent être servis depuis une adresse HTTPS (ou depuis `localhost`). Dépose le contenu de ce dossier sur un hébergement statique HTTPS gratuit, puis ouvre l'adresse sur le téléphone et utilise le menu du navigateur « Ajouter à l'écran d'accueil » / « Installer ».

Aucun compte ni abonnement n'est requis pour l'application elle-même. L'hébergement HTTPS peut être assuré par un service gratuit, mais il nécessite une mise en ligne initiale.

## Données et confidentialité
Les données sont stockées dans le navigateur de l'appareil, pas dans un compte en ligne. Elles ne se synchronisent pas automatiquement entre appareils. Utilise régulièrement « Exporter mes données » pour conserver une copie. Effacer les données du navigateur peut supprimer l'inventaire local.

## Limites de cette première version
- Déplacement d'un animal entre toutes les cases disponibles de tous les bâtiments.
- Recherche globale d'un bovin depuis l'accueil par ses 4 chiffres d'identification.
- Fiche individuelle de chaque bovin : type, emplacement actuel, lien mère/veau et historique personnel.
- Historique daté des déplacements, consultable depuis la fiche et le tableau de bord.
- Tableau de bord général : effectifs vaches/veaux, bâtiments, cases, capacité et places libres.
- Contrôle de cohérence de l'association mère/veau lors de la modification d'un animal.
- L'association mère/veau est facultative.
- Les numéros à 4 chiffres doivent être uniques dans tout l'inventaire.
