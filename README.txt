ASV RÉGIE Mobile V0.2 — prototype autonome, lecture seule

MISE A JOUR GITHUB PAGES
Dans le dépôt GitHub existant asv-regie-mobile, remplacer à la racine : index.html, sw.js, manifest.webmanifest. Ajouter production-demo.json. Conserver les icônes. Après commit, attendre la coche verte Actions puis rouvrir le site avec Internet, attendre 15 s, fermer/réouvrir. Le cache hors connexion est versionné.

TEST
Accueil > Charger la production fictive intégrée. Parcourir Planning (jour/lieu), Personnel, Contacts, Devis (PDF). Fermer l'app, activer mode Avion, relancer : données et PDF doivent rester disponibles.

IMPORT
Accueil > Importer un fichier de production > choisir production-demo.json depuis Fichiers iOS. Une seule production est stockée localement dans IndexedDB. Le fichier est du JSON avec format asv-regie-mobile, version 1, production, events, people, contacts, quotes. PDF intégré en base64. Aucune donnée de production n'est envoyée au serveur. Le JSON de démonstration est public et fictif.

LIMITES
Prototype de validation, pas encore compatible avec un export direct de l'application ASV RÉGIE ordinateur. Les PDF sont intégrés au JSON, taille max du fichier 18 Mo, 10 Mo par PDF encodé. Les données sont propres à cet appareil/navigateur et peuvent être supprimées par iOS si stockage effacé. Ne pas utiliser comme sauvegarde unique. Ne pas publier de données réelles sur GitHub.
