# 📚 Közelítő és Szimbolikus Számítások - Vizsga Segéd

Interaktív webalkalmazás a "Közelítő és Szimbolikus Számítások" tantárgy vizsgájára való felkészüléshez.

## ✨ Funkciók

### 🎲 Vizsga szimuláció
- **2 tétel kiválasztása** - Mint egy valódi vizsgán, válassz ki 2 tételt
- **Véletlenszerű húzás** - "Véletlenszerű 2 tétel" gombbal szimulálhatod a vizsgahelyzetet
- **29 vizsgatétel** - A teljes tételsor elérhető

### 🎤 Hangalapú keresés
- Beszélj a mikrofonba magyarul
- 2 másodperc csend után automatikusan keres
- Web Speech API (Chrome böngészőben működik legjobban)

### 🤖 AI-alapú válaszok (GPT-4.5 Preview)
- Intelligens válaszok a kérdésekre
- A jegyzet tartalmát figyelembe veszi
- Ha nincs elég info a jegyzetben, általános tudásból válaszol
- Tétel-specifikus kontextus kezelése

### 📄 PDF jegyzet integráció
- OCR feldolgozás (Tesseract.js)
- Automatikus szöveg-cache localStorage-ban
- PDF oldalak megtekintése a találatoknál

## 🚀 Telepítés és használat

### Előfeltételek
- Modern böngésző (Chrome ajánlott a hangfelismeréshez)
- OpenAI API kulcs (GPT-4.5 Preview hozzáférés)
- Helyi webszerver

### Indítás

1. **Klónozd/másold a fájlokat** a kívánt mappába

2. **Helyezd el a jegyzetet**: `sources/koszikicsi_pp.pdf`

3. **Indíts egy helyi szervert**:
   ```bash
   npx http-server
   # vagy
   npx serve
   # vagy
   python -m http.server 8080
   ```

4. **Nyisd meg a böngészőben**: `http://localhost:8080`

5. **Add meg az OpenAI API kulcsot** a weboldalon

## 📁 Fájlstruktúra

```
koszi_seged/
├── index.html      # Fő alkalmazás
├── tetelek.json    # 29 vizsgatétel adatbázisa
├── README.md       # Ez a fájl
└── sources/
    └── koszikicsi_pp.pdf   # Jegyzet PDF
```

## 📋 Vizsgatételek (29 db)

1. A számítógépes hiba különböző fajtái
2. Számítógépes számábrázolás és kerekítés
3. Numerikus stabilitás, a hiba továbbterjedése, kondíciószám
4. Intervallum aritmetika
5. Automatikus differenciálás
6. Lineáris egyenletrendszerek megoldása Gauss eliminációval
7. LU felbontás, eliminációs mátrixok, főelemkiválasztás
8. Mátrixinvertálás, mátrixnormák, mátrixok kondíciószáma
9. Cholesky felbontás, QR ortogonális felbontás
10. Mátrixok sajátértékei, sajátvektorai, a sajátértékek korlátai, a hatványmódszer
11. A mátrixok típusai, hasonlósági transzformáció
12. A sajátértékek és a sajátvektorok kondícionáltsága
13. LR transzformáció
14. Lineáris egyenletrendszerek iterációs módszerei, a Jacobi iteráció
15. Lineáris egyenletrendszerek iterációs módszerei konvergenciája
16. A Gauss-Seidel iteráció, mátrixok reguláris szétvágásai
17. Konjugált gradiens módszer
18. Lineáris egyenletek iterációs módszerei a Matlabban
19. Polinomok zérushelyei, Horner elrendezés, Ruffini sorozat, iterált Horner elrendezés
20. Polinomok kezelése a Matlabban
21. Függvényközelítések, Lagrange interpoláció
22. A Lagrange interpoláció hibája, interpoláció a Matlabban
23. Newton módszer, szelőmódszer, húrmódszer
24. Legkisebb négyzetek módszere
25. Spline közelítés, megvalósítása a Matlabban
26. Numerikus integrálás, kvadratúra-formulák
27. Interpolációs kvadratúra-formulák, ezek hibája
28. Véges differenciák, Newton-Cotes formulák
29. Numerikus integrálás a Matlabban

## 🎯 Használati tippek

### Vizsga szimuláció
1. Kattints a **"🎲 Véletlenszerű 2 tétel"** gombra
2. Kérdezz az adott tételekről: *"Mi a Gauss elimináció lényege?"*
3. Az AI a kiválasztott tételek kontextusában válaszol

### Hangalapú keresés
1. Kattints a **"🎤 Beszélj"** gombra
2. Mondd be a kérdést, pl.: *"5. tétel, hogyan működik az automatikus differenciálás?"*
3. A rendszer automatikusan felismeri a tételt és keres

### Tétel-specifikus keresés
- Mondd/írd: *"5. tétel"* → automatikusan kiválasztja
- Vagy kattints a tétel számára a rácsban
- Egyszerre max. 2 tétel választható

## ⚙️ Beállítások

### OpenAI API kulcs
- Szerezz kulcsot: https://platform.openai.com/api-keys
- GPT-4.5 Preview hozzáférés szükséges
- A kulcs biztonságosan a localStorage-ban tárolódik

### OCR újrafuttatás
Ha a jegyzet szövege rosszul lett felismerve:
1. Kattints az **"🔄 OCR újrafuttatás"** gombra
2. Várj az újra feldolgozásra

## 🛠️ Technológiák

- **PDF.js** - PDF renderelés
- **Tesseract.js** - OCR (magyar nyelv)
- **Web Speech API** - Hangfelismerés
- **OpenAI GPT-4.5 Preview** - AI válaszok
- **LocalStorage** - Cache tárolás

## ⚠️ Fontos megjegyzések

- A hangfelismerés **Chrome böngészőben** működik legjobban
- Az első betöltés lassabb lehet az OCR feldolgozás miatt
- Az OCR eredménye cache-elődik, következő betöltés gyors
- Az AI válaszok nem helyettesítik a tanulást!

## 📝 Licensz

Személyes és oktatási célú használatra.

---

*Készült a "Közelítő és Szimbolikus Számítások" vizsga sikeres teljesítéséhez! 🎓*
