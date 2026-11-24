# KitVital : actualités officielles

Fichier public lu par la page https://kitvital.fr/actualites. Écrit deux fois par jour (vers 6 h et 14 h, heure de Paris) par la veille automatique de KitVital.

- `actualites.json` : les dernières publications officielles (France, Union européenne, pays voisins) sur la préparation aux crises, le risque de conflit, les pénuries, la météo et la santé. Chaque entrée est datée et renvoie à sa page officielle. Depuis le 14 novembre 2026, le fichier contient aussi, à part (`"nature": "evenement"`), les grands événements du moment rapportés par une institution ou un média de référence, résumés sans commentaire.
- `a-traiter.md` : ce que la veille propose de changer dans les guides du site.

Méthode et règles : `docs/actualites.md` du dépôt du site. Les textes sont des résumés neutres ; seule la page liée fait foi.

## Baromètre KitVital : risque de guerre et de catastrophe

- `barometre.json` : le relevé quotidien du baromètre lu par la page https://kitvital.fr/barometre-des-risques et par l'accueil. Écrit chaque matin (vers 6 h, heure de Paris) par le script `npm run barometre:releve` du dépôt du site : valeurs de l'année en cours, actualité et analyse de chaque domaine, historique des scores, dernière alerte. Les scores sont toujours recalculés par le site avec sa méthode fixe.

Méthode : `docs/barometre.md` du dépôt du site.

## Visuels des réseaux sociaux

- `reseaux/instagram/` : les visuels JPEG (1080 × 1350) des publications Instagram de @kitvital.fr, nommés `<publication>-<numéro de diapositive>.jpg`. Ils sont lus par l'API de publication de Meta, qui exige une adresse publique. Les textes et sources de chaque publication sont tenus dans le projet KitVital (note `reseaux-sociaux.md`).
  Depuis le 24 novembre 2026, le dossier contient aussi les Reels (`kitvital-reel-<sujet>-v<n>.mp4`, 1080 × 1920, H.264 et AAC 128 kb/s, lus par Meta à leur adresse jsDelivr figée sur un commit ; sources des vidéos de la série « guerre et kit de survie » : dépôt pare-72h, `reseaux/videos/`) et `file.json`, la file d'attente de la publication quotidienne (une publication par jour à 12 h 15, heure de Paris) : date, format, adresses des images ou de la vidéo, légende, empreinte SHA-256 tronquée et statut (`a_valider`, `valide`, `publie`, `tache_dediee`). Seul le porteur fait passer une publication à `valide`.
- `reseaux/pinterest/` : les visuels JPEG (1000 × 1500) des épingles du compte Pinterest « kitvital », nommés `<épingle>.jpg`. Pinterest les télécharge depuis leur adresse publique au moment de créer l'épingle. Textes, tableaux et liens : projet KitVital (note `reseaux-sociaux.md`).
