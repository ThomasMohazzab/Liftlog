LIFTLOG — VERSION 4

NOUVEAU DANS LA VERSION 4 — PHOTO DU REPAS ANALYSÉE PAR L'IA
Dans l'onglet Calories, le bouton « Photo du repas » envoie la photo à Claude (Haiku 5.5 par défaut, Sonnet 5.5 en option). Claude estime les calories et les protéines, aliment par aliment, et remplit les champs. Tu vérifies, tu corriges si besoin, puis tu touches « Ajouter le repas ». Tu peux ajouter des précisions (quantités, sauce, huile) pour une estimation plus juste.

MISE EN ROUTE (une seule fois)
1. Va sur console.anthropic.com et crée un compte (séparé de ton abonnement Claude Pro).
2. Dans Billing, ajoute un peu de crédit.
3. Dans API Keys, crée une clé et copie-la (elle commence par « sk-ant- »).
4. Dans Liftlog : roue ⚙️ sur l'accueil > « Analyse IA des repas » > colle la clé > Enregistrer.
5. Choisis le modèle : Haiku 5.5 (rapide, ≈ 0,01 $/mois pour 2 photos par jour) ou Sonnet 5.5 (plus précis, ≈ 0,25 $/mois).

SÉCURITÉ DE LA CLÉ
La clé reste uniquement sur ton iPhone. Elle n'est pas dans le code publié sur GitHub et n'est pas incluse dans les sauvegardes exportées. Si tu changes de téléphone, recolle-la dans les réglages. Si tu penses qu'elle a fuité, supprime-la sur console.anthropic.com et crée-en une nouvelle.

DÉJÀ PRÉSENT (VERSION 3)
- Onglet Calories :
  • Objectifs de calories et de protéines (et calories de maintien, 2 500 kcal par défaut), modifiables avec « Modifier ».
  • Saisie des repas de chaque jour (nom, kcal, protéines) avec deux barres de progression vers tes objectifs. La barre des calories passe en rouge si tu dépasses.
  • Les flèches ‹ › changent de jour, pour compléter un oubli.
  • Calendrier : vert = objectif respecté (égal ou en dessous), rouge = objectif dépassé. Touche un jour pour l'ouvrir.
  • Bilan de la semaine (lundi → dimanche) : déficit ou surplus par rapport au maintien. Calcul : somme, pour chaque jour où tu as noté des repas, de (calories mangées − maintien). Les jours sans repas ne comptent pas. La journée en cours est incluse. Estimation en kg avec 7 700 kcal ≈ 1 kg.
- Galerie photos : bouton en haut à droite de l'accueil (et du calendrier). Toutes tes photos, classées par mois avec leur date. Touche une photo pour l'agrandir, passer à la suivante ou ouvrir ce jour dans le calendrier.
- La barre d'onglets passe à 6 onglets : Accueil · Calendrier · ＋ · Perfs · Calories · Notes.
- Les repas sont inclus dans l'export de sauvegarde.

DÉJÀ PRÉSENT (VERSION 2)
- Navigation par onglets en bas de l'écran : Accueil · Calendrier · ＋ Ajouter · Perfs · Notes.
- Accueil : personnage « chibi » qui prend du muscle à chaque jour de streak (7 stades, forme maximale à 6 jours, de « Brindille » à « Légende ») et redevient maigre quand la streak retombe à zéro. On y trouve aussi la streak en cours, le record de streak, la charge maximale avec son exercice et les boutons « Jour de salle » / « Jour de repos ».
- Calendrier : vert = salle, bleu = repos, flamme animée autour des jours de record. Touche un jour pour voir les exercices de ce jour (les exercices et séries record sont en or) et pour y attacher une photo de progression.
- Ajouter : saisie série par série (poids + reps). Les valeurs de la dernière séance s'affichent en gris pour servir de repère.
- Perfs : filtre par groupe musculaire. Touche un exercice pour ouvrir sa page : courbe (charge max, reps totales, volume), détail de chaque séance série par série, modification ou suppression d'une séance.
- Notes : inchangées.
- Supprimés : l'historique et la case « Performances enregistrées ».
- Sauvegarde : roue ⚙️ en haut de l'accueil (export/import, photos comprises).

RÈGLE DE LA STREAK
Un jour de salle ajoute 1. Un jour de repos isolé est toléré (il ne compte pas). Deux jours de repos d'affilée, ou une journée sans rien valider, remettent la streak à zéro.

TES DONNÉES
- Tes anciennes performances sont converties automatiquement en séances (une série chacune) au premier lancement. Les anciennes données ne sont pas effacées.
- Streak, jours de repos, record et notes sont conservés.
- Les photos sont réduites puis stockées sur l'iPhone. Elles sont incluses dans l'export (le fichier sera donc plus lourd).
- Ne supprime pas les données du site dans Safari, et exporte une sauvegarde de temps en temps.

MISE À JOUR SUR GITHUB
1. Dans ton dépôt GitHub, remplace index.html, sw.js et README-FR.txt par ceux de ce dossier (manifest.json et les icônes sont inchangés).
2. Attends une minute que GitHub Pages republie.
3. Sur l'iPhone, ouvre l'appli, ferme-la complètement, puis rouvre-la. Le cache est passé en version 11 pour forcer le chargement de la nouvelle version.
