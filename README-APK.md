# Mathématiques interactives — application Android

Ce projet transforme le site de cours en application Android (WebView), avec les pages HTML intégrées dans l'application. Les élèves n'ont pas besoin de compte. La plupart des pages sont consultables hors ligne ; les éléments distants (par exemple certaines polices) demandent Internet.

## Générer l'APK

Le fichier APK n'a pas pu être compilé directement dans l'environnement de préparation, car Android SDK/Gradle ne sont pas installés ici. Le projet contient un workflow GitHub Actions qui construit l'APK.

1. Créer un dépôt GitHub et y envoyer tout le contenu de ce dossier.
2. Ouvrir l'onglet **Actions** du dépôt.
3. Sélectionner **Construire l'APK Android**, puis **Run workflow** (ou attendre la fin du build après un push).
4. Ouvrir le run terminé et télécharger l'artefact `mathematiques-interactives-apk`.
5. Extraire le ZIP de l'artefact : il contient `app-debug.apk`, installable sur Android après autorisation d'installation depuis cette source.

## Contenus

- 4e — classe 416
- 3e — classe 312
- 3e — classe 306 (page provisoire : le dossier source de la 306 n'était pas présent parmi les fichiers reçus)
- Seconde
- Première spécialité

Pour ajouter le contenu réel de la 306, remplacer `app/src/main/assets/site/cours/maths-3e-306.html` par son fichier HTML et conserver le nom du fichier, ou mettre à jour le lien dans `cours.js` si le fichier principal porte un autre nom.
