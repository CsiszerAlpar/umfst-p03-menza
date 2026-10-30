# Kollégiumi Menza Heti Menü – Projektjelentés

Repo: https://github.com/CsiszerAlpar/umfst-p03-menza
Élő demó: https://csiszeralpar.github.io/umfst-p03-menza/
Készítette: Hallgató Neve, Csoport

## A projekt áttekintése
A feladat célja egy akadálymentes, szemantikus HTML-en alapuló heti menza táblázat kialakítása volt, amely modern reszponzív dizájnnal (mobil kártyanézet), nyomtatási optimalizációval és Schema.org Menu strukturált adatokkal támogatja a felhasználókat, a képernyőolvasókat és a keresőmotorokat.

## Miért pont ezek az elemek?
- **`<abbr>` (Allergének):** Lehetővé teszi a képernyőolvasók számára, hogy a rövidítések helyett a teljes allergén nevet olvassák fel (`title="..."` attribútum révén), miközben vizuálisan kompakt marad a táblázat.
- **`<data value="...">` (Árak):** Gépileg olvasható értéket biztosít (`value` attribútum a precíz értékhez és valutanemhez), míg a felhasználók számára a szokásos emberi szöveget ("X lej") jeleníti meg.
- **`<time datetime="...">` (Dátumok):** Gépek és naptárak számára szabványosított időformátumot biztosít, javítva a keresőmotorok és asszisztensek általi feldolgozhatóságot (SEO / GEO).

## Tesztelés és Validáció
- **W3C HTML / CSS Validator:** 0 hiba (hibátlan szintaxis).
- **validator.schema.org:** A JSON-LD Menu struktúra 0 hibával és figyelmeztetéssel lefutott (Rich Results kompatibilis).
- **Lighthouse Accessibility audit:** Elért pontszám: **100**.
- **Képernyőolvasó (NVDA / VoiceOver):** A `scope="col"` és `scope="row"` attribútumoknak köszönhetően a cellák felolvasásakor a képernyőolvasó pontosan bemondja a napot és a fogás típusát is.

A validációs eredményekről készült képernyőképek a `docs/schema.png` útvonalon találhatók.
