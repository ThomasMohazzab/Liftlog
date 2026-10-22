LIFTLOG — INSTALLATION

Ce dossier contient une PWA (application web installable) pour suivre les performances de musculation.

CE QUI EST DÉJÀ PRÉVU
- Saisie exercice, poids, répétitions et date
- Graphique par exercice (poids ou répétitions)
- Historique avec suppression d'une entrée
- Sauvegarde locale automatique dans le navigateur
- Export/import d'une sauvegarde JSON
- Mise en cache pour utilisation hors ligne après la première visite

IMPORTANT SUR LES SAUVEGARDES
Les données restent sur l'appareil et dans le navigateur où elles sont saisies. Elles ne sont pas automatiquement synchronisées dans le cloud. Utilise régulièrement « Exporter une sauvegarde » et conserve le fichier dans Fichiers/iCloud Drive ou ailleurs. Pour synchroniser automatiquement plusieurs appareils, il faut ajouter un backend/compte en ligne.

MISE EN LIGNE POUR L'INSTALLER SUR IPHONE
1. Décompresse liftlog-pwa.zip.
2. Publie le contenu du dossier sur un hébergeur HTTPS (par exemple GitHub Pages).
3. Sur l'iPhone, ouvre l'URL publiée dans Safari.
4. Appuie sur Partager > Sur l'écran d'accueil > Ajouter.
5. Lance LIFTLOG depuis l'icône. Après le premier chargement, le cache hors ligne peut permettre de l'ouvrir sans réseau.

Pour activer GitHub Pages : crée un dépôt GitHub, téléverse tous les fichiers du dossier à la racine, puis dans Settings > Pages, sélectionne le déploiement depuis la branche principale (root). Attends que l'URL HTTPS soit publiée.


NOUVEAU — STREAK SALLE
Le streak compte les dates distinctes où au moins une performance a été enregistrée. Le streak actuel reste actif si la dernière séance date d’aujourd’hui ou d’hier ; après une journée complète sans séance, il retombe à zéro. Le record est conservé localement et inclus dans les nouvelles sauvegardes exportées.

MISE A JOUR STREAK : le bouton « Je suis allé à la salle ! » confirme une seule présence par jour. Le streak et le record sont stockés localement dans le navigateur. Le bouton ne crée pas de performance de musculation. Les anciens jours contenant des performances sont importés comme jours de présence lors de la première mise à jour.


NOUVEAU — RECORDS PERSONNELS
- Détection automatique des records de poids et de répétitions, par exercice.
- Un record de répétitions se compare au même poids pour cet exercice.
- Le total additionne les records de poids ET de répétitions, comme demandé.
- Calendrier des jours où au moins un record a été établi, records récents et filtres par groupe musculaire.
- Animation de célébration à chaque nouveau record.
- Les records sont calculés à partir de l'historique déjà enregistré : pas de perte des performances précédentes.

MISE À JOUR
Remplace les fichiers du dépôt par ceux de cette archive. Le cache du service worker est versionné pour forcer la mise à jour. Les clés de sauvegarde locale des performances et du streak sont conservées. Ne supprime pas les données du site dans Safari.
