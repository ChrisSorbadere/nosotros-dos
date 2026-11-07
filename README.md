# Nosotros Dos

Preguntas, juegos, salidas y rituales para Blanca y Chris.

Appli web : https://chrissorbadere.github.io/nosotros-dos/

## Appli Android (Capacitor)

- `android/`, `capacitor.config.json`, `package.json`, `app-shell/` : projet Capacitor. L'APK charge `chrissorbadere.github.io/nosotros-dos/` : les mises à jour web (cartes, design) arrivent sans réinstaller.
- `.github/workflows/apk.yml` : à chaque modification de la partie Android, GitHub construit l'APK signé (clé stockée dans les secrets `ANDROID_KEYSTORE_BASE64` et `ANDROID_KEYSTORE_PASSWORD` du dépôt) et le publie dans **Releases**.
- Installer : page **Releases** › dernier `NosotrosDos-….apk` › ouvrir › autoriser l'installation. Les versions suivantes s'installent par-dessus.
- Ne jamais changer la clé de signature : sinon l'APK ne s'installe plus par-dessus l'ancien.
