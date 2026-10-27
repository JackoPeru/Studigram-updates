# Studigram Updates

Public update feed for the Studigram Android app.

This repository is intentionally public so installed clients can check new
versions without accessing the private source repository (`JackoPeru/studigram`).

## Schema di `latest.json`

```json
{
  "versionCode": 10001,
  "versionName": "1.0.0",
  "tagName": "autoupdate-10001",
  "apkUrl": "https://github.com/JackoPeru/Studigram-updates/releases/download/autoupdate-10001/Studigram-1.0.0-android.apk",
  "assetName": "Studigram-1.0.0-android.apk",
  "assetSize": 3288724,
  "sha256": "...",
  "publishedAt": "2026-10-27T15:50:00Z",
  "notes": ["..."]
}
```

L'app (plugin nativo `AppUpdatePlugin`) consulta `latest.json`, confronta il
`versionCode` con quello installato, scarica l'APK da GitHub Releases e lo
installa solo dopo verifica di package, versionCode, sha256 e firma che
coincide con l'app installata.

Le release `autoupdate-NNNN` di questo repo sono le release delle APK:
`studigram-updates` è il canale di distribuzione, il repo sorgente resta privato.
