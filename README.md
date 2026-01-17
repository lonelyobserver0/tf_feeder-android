# TF Feeder

App Android per accedere a [frontek.dev/tf_feeder](https://frontek.dev/tf_feeder), un aggregatore di feed RSS.

## Funzionalità

- Accesso diretto al sito TF Feeder tramite WebView
- Login e registrazione per sincronizzare i preferiti
- Navigazione interna al sito
- Link esterni aperti nel browser di sistema
- Supporto cookies per mantenere la sessione
- Pulsante back per navigare nella cronologia

## Fonti RSS supportate

- ANSA
- Repubblica
- HW Upgrade
- BBC News
- NY Times

## Build

### Requisiti

- Android Studio
- JDK 11+
- Android SDK 35

### Debug

```bash
./gradlew assembleDebug
```

L'APK sarà in `app/build/outputs/apk/debug/app-release.apk`

### Release

Crea un file `keystore.properties` nella root del progetto:

```properties
storeFile=/path/to/keystore.jks
storePassword=your_password
keyAlias=your_alias
keyPassword=your_password
```

Poi esegui:

```bash
./gradlew assembleRelease
```

L'APK sarà in `app/build/outputs/apk/release/app-release.apk`

## Autore

lonelyobserver0
