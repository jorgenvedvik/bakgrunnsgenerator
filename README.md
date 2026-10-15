# Bakgrunnsgenerator – Patentstyret

Nettside for å lage nye utsnitt av Patentstyrets logobakgrunn til Some-maler.
Utsnittet består av logosymbolet (#002b25) på bakgrunnsfargen (#00342e).

## Bruk
- Velg format: kvadrat 1:1, stående 4:5, story 9:16, lenke 1,91:1, bred 16:9 eller egendefinert størrelse.
- Trykk **Nytt utsnitt** (eller mellomrom) til du finner et du liker. **Forrige** henter tilbake det forrige.
- Tilfeldige utsnitt følger reglene fra de håndlagde utsnittene: symbolet forstørret 5,6–8,6×, innhugget
  (enden av den smale kanalen) nær en kant, minst to hjørner dekket og en rolig midtsone for tekst.
  Reglene står i `RULES` og `TIPS` i `index.html`.
- **Finjuster utsnittet** (sammenleggbart panel) har skalering, rotasjon, speiling, posisjon og fargebytte.
- Finjuster: dra i bildet for å flytte, scroll/klyp for å skalere, Shift + scroll for å rotere, piltaster for små steg.
- Eksporter som PNG (1×, 2× eller 3×), JPG eller SVG (vektor, åpnes i Figma/InDesign/Illustrator).
- **Kopier lenke til utsnittet** gir en lenke som åpner nøyaktig samme utsnitt hos en kollega.

## Teknisk
Grensesnittet bruker PUI, Patentstyrets designsystem (`@patentstyret/designsystem` 1.2.0, https://pui.patentstyret.no).
Komponentene ligger i `vendor/pui/` (uten kildekart), så siden ikke er avhengig av en ekstern CDN.
Brukt: `ps-logo`, `ps-button`, `ps-toggle`, `ps-text-field`, `ps-accordion`, `ps-toast`, `ps-material-symbol` og PUI-tokenene (`--ds-*`).
Formatkortene og gliderne finnes ikke i PUI, og er bygget med PUI-tokenene.
For å oppgradere PUI: `npm pack @patentstyret/designsystem@<versjon>` og kopier `dist/ps-designsystem/` og `dist/global/global.css` til `vendor/pui/`.

Én statisk fil (`index.html`), ingen byggesteg. Vercel publiserer den direkte fra `main`.
Farger og logosti ligger øverst i skriptet (`COLORS` og `PATHS`).
