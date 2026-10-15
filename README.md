# Bakgrunnsgenerator – Patentstyret

Nettside for å lage nye utsnitt av Patentstyrets logobakgrunn til Some-maler.
Utsnittet består av logosymbolet (#002b25) på bakgrunnsfargen (#00342e).

## Bruk
- Velg format: kvadrat 1:1, stående 4:5, story 9:16, lenke 1,91:1, bred 16:9 eller egendefinert størrelse.
- Trykk **Nytt tilfeldig utsnitt** (eller mellomrom) til du finner et du liker.
- Finjuster: dra i bildet for å flytte, scroll/klyp for å skalere, Shift + scroll for å rotere, piltaster for små steg.
- Eksporter som PNG (1×, 2× eller 3×), JPG eller SVG (vektor, åpnes i Figma/InDesign/Illustrator).
- **Kopier lenke til utsnittet** gir en lenke som åpner nøyaktig samme utsnitt hos en kollega.

## Teknisk
Én statisk fil (`index.html`), ingen byggesteg. Vercel publiserer den direkte fra `main`.
Farger og logosti ligger øverst i skriptet (`COLORS` og `PATHS`).
