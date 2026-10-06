# OmniTCG — sito

Pagina di presentazione dell'app [OmniTCG](https://github.com/TheJack95/tcg-scanner), pubblicata con GitHub Pages su <https://thejack95.github.io/>.

Sito statico, nessuna build: `index.html` e `icon.png`, serviti così come sono (`.nojekyll` disattiva Jekyll).

## Link all'APK

Il pulsante "Scarica l'APK" punta a `APK_URL`, in fondo a `index.html`:

```
https://github.com/TheJack95/tcg-scanner/releases/latest/download/omnitcg.apk
```

Scarica il file `omnitcg.apk` allegato all'ultima release di `tcg-scanner`, quindi per una nuova versione basta pubblicare una release con un file con lo stesso nome. Funziona solo se quel repository è pubblico.

## Loghi dei giochi

`games/` contiene i loghi che l'app usa nei riquadri della Collezione (`assets/*.png` di `tcg-scanner`), ridotti a 360 px di larghezza.

## Icona

`icon.png` è l'icona dell'app ridotta a 512 px (`assets/icon.png` di `tcg-scanner`, generata da `scripts/make-icon.ps1`).
