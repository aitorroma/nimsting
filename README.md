# nimsting.nimbox360.com

Web estática servida con GitHub Pages: página de descarga de **NimRecord** (app Android de grabación de llamadas) y el propio `.apk`.

- `index.html` — página de descarga.
- `NimRecord.apk` — build de la app (se sirve en `/NimRecord.apk`).
- `NimRecord.apk.sha256` — checksum.
- `CNAME` — dominio personalizado (`nimsting.nimbox360.com`).

## Actualizar la APK

```sh
cp /ruta/a/app-debug.apk NimRecord.apk
sha256sum NimRecord.apk > NimRecord.apk.sha256
git commit -am "apk: nueva build" && git push
```
