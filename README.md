# play.gamesit.no

Spillsidene til Andersen Games & IT: https://play.gamesit.no

Kopiert fra `eirikya/eirikya.github.io` (branch `main`) 18.10.2026. Den gamle siden ligger fortsatt oppe fordi appene lenker dit. Endringer i personvernsidene må gjøres begge steder til appene er oppdatert med nye lenker.

- `index.html` – oversikt med ett kort per spill og generell brukerstøtte (`/#support`). Gamle lenker som `/#zoopop` sendes videre til spillets side.
- `<spill>/index.html` – egen side per spill med beskrivelse, skjermbilder, brukerstøtte og spørsmål og svar. Bruk `https://play.gamesit.no/<spill>/` som support- og markedsførings-URL i App Store og Google Play.
- Én personvernerklæring per spill, i en egen mappe per spill, på norsk og engelsk:
  - `zoopop/personvern.html` – Zoo Pop: Animal Merge
  - `tumble-numbers/personvern.html` – Tumble Numbers
  - `slippery-paws/personvern.html` – Slippery Paws
  - `minisudoku/personvern.html` – Minisudoku
- `personvern.html` og `privacy.html` – gamle adresser for Zoo Pop, sender videre til `zoopop/personvern.html` (så gamle lenker virker)
- `app-ads.txt` – bekrefter overfor annonsørene at appene er dine. Gjelder alle appene i samme AdMob-konto (linjen fra AdMob: Apper → Vis alle apper → app-ads.txt)
- `assets/` – stil og språkbytte, `img/` – ikoner og skjermbilder

Språket velges automatisk etter nettleseren og kan byttes øverst til høyre. `?lang=no` eller `?lang=en` i adressen tvinger et språk.

## Nytt spill
1. Lag mappen `<spill>/` med `personvern.html` (kopier et av de andre spillene, rett navn, dato og det som lagres, og stiene `../assets/` og `../img/`).
2. Lag `<spill>/index.html` (kopier et annet spills side, bytt tekst, skjermbilder og spørsmål og svar). Legg til et kort i `index.html`, en lenke i bunnen og spill-ID-en i skriptet som sender `/#<spill>` videre.
3. Privacy Policy URL i App Store Connect: `https://play.gamesit.no/<spill>/personvern.html`. Samme adresse i AdMob-samtykkemeldingen og i appen.
