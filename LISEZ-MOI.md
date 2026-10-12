# Obtenir le fichier APK (Android) — sans Play Store, sans Android Studio

Le fichier APK est construit gratuitement par GitHub (vous n'installez rien sur votre ordinateur).

1. Créez un compte gratuit sur https://github.com puis un nouveau dépôt (bouton « New »), nom au choix, en « Private ».
2. Dans le dépôt : « Add file » → « Upload files », puis glissez TOUT le contenu de ce dossier `android-apk`
   (y compris le dossier caché `.github`, `www`, `assets`, `package.json`, `capacitor.config.json`). Cliquez « Commit changes ».
   Si `.github` n'a pas été envoyé : « Add file » → « Create new file », tapez le nom `.github/workflows/build-apk.yml` et collez le contenu du fichier du même nom.
3. Onglet « Actions » → « Construire l'APK » → « Run workflow ». Attendez environ 5 à 8 minutes (pastille verte ✓).
4. Cliquez sur l'exécution terminée → en bas, « Artifacts » → téléchargez « MR-Service-Manager-APK » (un .zip contenant `app-debug.apk`).
5. Envoyez `app-debug.apk` sur le téléphone (WhatsApp, câble, Drive), ouvrez-le et autorisez « Installer des applications inconnues » pour cette source.
6. L'application « MR Service Manager » apparaît avec son icône. Elle fonctionne entièrement hors ligne.

Sur Android : « Exporter JPG/PNG/PDF » et « Partager l'image » ouvrent la feuille de partage (enregistrer dans Fichiers/Drive, envoyer sur WhatsApp…).
« Envoyer sur WhatsApp » ouvre la conversation du numéro de la fiche avec le message prérempli.
Les données restent sur le téléphone : Paramètres → Exporter / Importer une sauvegarde pour les transférer.
