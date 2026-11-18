# Historique des versions

Les fichiers de chaque version sont sur la page [Releases](https://github.com/guerinbruno1-wq/suivi-recharges-ve/releases). Utilisez de préférence la **dernière version**.

## 1.2.13 — fiabilité et sécurité
- Synchronisation : une recharge saisie ou corrigée pendant une synchronisation n’est plus perdue.
- Android : les codes d’accès à la borne et à la voiture ne sont plus inclus dans la sauvegarde Google ni dans le transfert vers un nouveau téléphone (à ressaisir sur un nouvel appareil).
- Autorisation de la borne Legrand : contrôle renforcé de l’adresse de retour.
- Export CSV : une note commençant par « = », « + », « - » ou « @ » ne peut plus être interprétée comme une formule par Excel.

## 1.2.12 — écran « Voiture »
- Nouvel onglet **Voiture** (Hyundai, Kia, Genesis connectées) : % de batterie et autonomie, charge en cours et temps restant, objectifs de charge, kilométrage, position sur la carte, verrouillage et ouvrants, pression des pneus, climatisation, température extérieure, voyants d’alerte.
- Lecture seule, par l’accès officiel (EU Data Act) : les commandes à distance restent dans l’application du constructeur.

## 1.2.11 — synchronisation téléphone ↔ PC
- Les recharges, véhicules et tarifs se synchronisent **automatiquement** entre Android et Windows, par un fichier placé dans votre cloud (kDrive, OneDrive…).
- Réglages → « Synchronisation téléphone ↔ PC » : « Créer le fichier » sur le premier appareil, « Choisir le fichier existant » sur l’autre.
- Les recharges déjà importées par CSV sont reconnues (pas de doublons) ; les suppressions sont reportées.
- Les codes d’accès à la borne et à la voiture restent propres à chaque appareil.

## 1.2.10 — nom générique
- L’application s’appelle **« Suivi Recharges VE »** sur Android, comme sur Windows (avant : « Recharge Ioniq 5 »).
- Le véhicule créé à la première installation s’appelle « Ma voiture » (à renommer et régler dans Réglages).
- Une installation existante garde ses données et son véhicule.

## 1.2.9 — durée de charge mesurée par la borne
- Borne Legrand : la durée de charge mesurée est lue (ex. 33,0 kWh en 4 h 49).
- Bouton « Fin = début + durée » pour fixer l’heure de fin à partir de l’heure de début réelle.
- Messages de réussite en couleur neutre.

## 1.2.8 — autorisation directe de la borne
- Bouton « Autoriser l’accès à la borne » : demande à Netatmo l’autorisation `read_boreal`, absente du « Token generator ».
- Sur PC, l’autorisation est récupérée automatiquement ; sur téléphone, il suffit de coller l’adresse affichée.

## 1.2.7 — diagnostic de la borne
- Instructions corrigées : la borne Green’Up Home relève de l’autorisation `read_boreal`.
- Le test de connexion indique les autorisations du jeton et le nombre de maisons / appareils vus.

## 1.2.6 — voiture connectée plus fiable
- Le VIN devient facultatif : il est détecté automatiquement.
- Message clair quand la clé Pleos est refusée ; diagnostic étape par étape.
- Le téléphone et le PC ne se « déconnectent » plus l’un l’autre.

## 1.2.5 — voiture connectée
- Bouton « Lire la voiture » : kilométrage et % de batterie lus via l’accès officiel Hyundai / Kia / Genesis (EU Data Act).

## 1.2.4 — borne Legrand
- Bouton « Remplir depuis la borne Legrand » : kWh mesurés par la borne Green’Up Home (via Netatmo).

## 1.2.3 — photo entière sur Windows
- La photo du véhicule s’affiche en entier, sans recadrage.

## 1.2.2 — installeur Windows
- Première version publiée avec l’installeur Windows (`.msi`).

## 1.2.1 — version Windows 11
- Version Windows 11, avec les mêmes écrans que la version Android.
- Export / import CSV pour échanger les recharges entre téléphone et PC.
- (Cette version ne contenait que le fichier Android.)

## Avant 1.2.1 (versions Android distribuées à la main)
- Suivi de plusieurs véhicules.
- Km parcourus par mois ; consommation aux 100 km par recharge et par mois.
- Saisie du % de batterie au clavier ; bandeau avec photo du véhicule.
- Première version : pré-enregistrement et fin de recharge, coût EDF heures creuses / pleines, bornes rapides, graphiques mensuels.
