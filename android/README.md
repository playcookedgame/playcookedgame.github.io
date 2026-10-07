# Cooked Android app

A thin native shell (WebView) around https://playcookedgame.github.io. Site updates show up in the app automatically;
rebuild the APK only when the icon, name or this shell changes.

Secrets required in the GitHub repo (Settings > Secrets and variables > Actions):
- ANDROID_KEYSTORE_B64      base64 of the PKCS12 keystore (alias: cooked)
- ANDROID_KEYSTORE_PASSWORD the keystore password

Keep a backup of the keystore: the same key must sign every future version, otherwise players cannot update.
Download link for players: https://github.com/playcookedgame/playcookedgame.github.io/releases/latest/download/Cooked.apk
