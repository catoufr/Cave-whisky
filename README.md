# Ma Cave à Whisky : appli web installable (version 0.1)

Appli personnelle, gratuite, qui fonctionne hors connexion. Les fiches sont enregistrées **sur l'appareil**
(il n'y a pas encore de synchronisation entre téléphone et PC).

## Contenu du dossier
- `index.html` : toute l'appli (fiches, photos, notes, amis, consultation, export / import)
- `manifest.webmanifest` : nom, couleurs et icônes pour l'installation
- `sw.js` : service worker (cache hors connexion). Changer `VERSION` à chaque mise à jour des fichiers
- `vendor/jszip.min.js` : lecteur et créateur de ZIP (copie locale)
- `icons/` : icônes de l'appli

## Mise en ligne
Une appli installable doit être servie en HTTPS depuis une adresse web (un double-clic sur `index.html` ne suffit pas).
Il faut donc déposer ce dossier tel quel sur un hébergement statique gratuit. Garder la même adresse ensuite :
les fiches sont rattachées à cette adresse, et en changer fait repartir l'appli à vide (exporter avant).

## Installation sur Android
Ouvrir l'adresse dans Chrome, puis menu ⋮ > Installer l'application (ou Ajouter à l'écran d'accueil).

## Reprendre les fiches du prototype
Dans le prototype (artefact), onglet Échange : exporter (ZIP). Dans cette appli, onglet Échange : importer le ZIP.

## Sauvegarde
Onglet Échange > Exporter, au moins une fois par mois. L'appli affiche un rappel au bout de 30 jours.

## Pas encore là
Synchronisation Google Drive, lecture de l'étiquette par IA gratuite, alertes promos.
