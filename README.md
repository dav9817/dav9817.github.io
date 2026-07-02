# GIS Portfolio — Davide Bortoletto

Sito portfolio (GitHub Pages, **sito utente**). Pronto per la pubblicazione.

## Struttura

```
portfolio-site/
├── index.html                      Home: bio + 4 progetti
├── projects/
│   ├── solar-pv-verona.html        Solare (tema chiaro)
│   ├── powerline-lidar.html        LiDAR (tema chiaro)
│   ├── no2-nightlights.html        NO₂ (tema scuro)
│   └── mars-suitability.html       Marte (teaser "in arrivo", non linkato)
└── assets/img/                     immagini ottimizzate (.webp)
```

## Stato

- Tutte le pagine complete, HTML valido, immagini presenti (nessun riquadro vuoto).
- Immagini ottimizzate in **WebP alta qualità** (q92): sito ~47 MB invece di ~169 MB.
- Gli **originali** (PNG/JPG a piena risoluzione) sono conservati fuori dal sito,
  in `../_portfolio_img_originali/` (cartella `03_NO2_N_lights`) — non vengono pubblicati.
- Link **Email**, **LinkedIn** e **GitHub** già impostati nella home.
- La card **Marte** è visibile ma non cliccabile ("In arrivo").

## Pubblicare su GitHub Pages (sito utente)

1. Crea un repository pubblico chiamato **`dav9817.github.io`**.
2. Copia **il contenuto** di questa cartella `portfolio-site/` nella radice del repo
   (quindi `index.html` deve stare in cima, non dentro una sottocartella).
   ⚠️ Non copiare `_portfolio_img_originali` (sono i backup, non servono online).
3. `git add . && git commit -m "portfolio site" && git push`
4. Su GitHub → **Settings → Pages** → Source: *Deploy from a branch* →
   branch `main`, cartella `/ (root)`. Salva.
5. Dopo ~1 minuto il sito è online su `https://dav9817.github.io`.

## Note

- Le pagine sono file singoli (HTML + CSS inline): nessuna dipendenza esterna
  a parte i caratteri di sistema.
- Per aggiungere il progetto **Marte** in futuro: completa `projects/mars-suitability.html`
  e riattiva il link nella home (la card è già pronta, basta ripristinare `<a href=…>`).
