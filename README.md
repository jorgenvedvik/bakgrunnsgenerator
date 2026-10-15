# Bakgrunnsgenerator – Patentstyret

Nettside for å lage nye utsnitt av Patentstyrets logobakgrunn til Some-maler.
Utsnittet består av logosymbolet (#002b25) på bakgrunnsfargen (#00342e).

## Bruk
- Velg format: kvadrat 1:1, stående 4:5, story 9:16, lenke 1,91:1, bred 16:9 eller egendefinert størrelse.
- Trykk **Nytt utsnitt** (eller mellomrom) til du finner et du liker. **Forrige** henter tilbake det forrige.
- Tilfeldige utsnitt følger reglene fra de håndlagde utsnittene: symbolet forstørret 5,6–8,6×, innhugget
  (enden av den smale kanalen) nær en kant, minst to hjørner dekket og en rolig midtsone for tekst.
  Reglene står i `RULES` og `TIPS` i `index.html`.
- Formater, Forrige, Nytt utsnitt, **Juster** og **Last ned** ligger i dokken nederst. Juster åpner en skuff med
  skalering, rotasjon, speiling, posisjon, fargebytte og hjelpelinjer. Bytter man format, lages et nytt utsnitt
  automatisk, med mindre utsnittet er justert for hånd.
- Finjuster: dra i bildet for å flytte, scroll/klyp for å skalere, Shift + scroll for å rotere, piltaster for små steg.
- Eksporter som PNG (1×, 2× eller 3×), JPG eller SVG (vektor, åpnes i Figma/InDesign/Illustrator).
- **Kopier lenke til utsnittet** gir en lenke som åpner nøyaktig samme utsnitt hos en kollega.

## Teknisk
Én statisk fil (`index.html`), ingen byggesteg. Vercel publiserer den direkte fra `main`.
Farger og logosti ligger øverst i skriptet (`COLORS` og `PATHS`).
