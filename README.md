# OmniTCG — sito

Pagina di presentazione dell'app [OmniTCG](https://github.com/TheJack95/tcg-scanner), pubblicata con GitHub Pages su <https://thejack95.github.io/>.

Sito statico, nessuna build: `index.html` e `icon.png`, serviti così come sono (`.nojekyll` disattiva Jekyll).

## Link all'APK

Il pulsante "Scarica l'APK" punta a `APK_URL`, in fondo a `index.html`:

```
https://storage.googleapis.com/omnitcg-apk/omniTCG-1.4.0.apk
```

Il file sta nel bucket GCS `omnitcg-apk`, che deve essere leggibile da tutti (`allUsers` → *Storage Object Viewer*). Il nome contiene la versione: a ogni release si carica il nuovo APK e si aggiorna `APK_URL`.

```bash
gcloud storage cp omniTCG-X.Y.Z.apk gs://omnitcg-apk/ --content-type=application/vnd.android.package-archive
```

## Loghi dei giochi

`games/` contiene i loghi che l'app usa nei riquadri della Collezione (`assets/*.png` di `tcg-scanner`), ridotti a 360 px di larghezza.

## Icona

`icon.png` è l'icona dell'app ridotta a 512 px (`assets/icon.png` di `tcg-scanner`, generata da `scripts/make-icon.ps1`).
