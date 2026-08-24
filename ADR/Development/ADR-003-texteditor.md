# ADR-003: TextEditor (WYSIWYG) komponenti TEDI-READY's ei pakuta

- **Staatus:** Proposed
- **Kuupäev:** 2026-08-24
- **ADR ID:** ADR-003
- **Otsuse tegijad:** Märt Sessman, Tõnis Tobre, Airike Jaska

---

## 1. Kontekst

Disainisüsteemis Figmas on **TextEditor**'i (WYSIWYG / rich text redaktor) disainikomponent olemas ja projektid on küsinud, kas see peaks tulema ka TEDI-READY-sse.

TextEditor on selleks erandlik komponent: funktsionaalsuse ulatus on praktiliselt piiramatu (vormindus, tabelid, pildid, HTML-i puhastus, ligipääsetavus jne) ja iga projekt vajab neist erinevat alamhulka. Küpsed teegid on osalt tasulise litsentsiga (TinyMCE, CKEditor, Froala), avatud alternatiivid (Lexical, TipTap, Quill, Slate) erinevad arhitektuuriliselt oluliselt. Teek ise on mahult üks suuremaid front-end sõltuvusi.

---

## 2. Otsus

**TEDI-READY ei paku TextEditor'i komponenti ega sisalda ühtegi WYSIWYG teeki sõltuvusena.**

- TextEditor'i disainikomponent jääb disainisüsteemi (Figma) alles ja on projektidele visuaalseks aluseks.
- Teostus on projektimeeskonna vastutus: lokaalne komponent või community/kolmanda osapoole teek.
- Projekt vastutab ise litsentsi, versioonihalduse, turvalisuse ja ligipääsetavuse eest.

---

## 3. Tagajärjed

**Positiivsed:**

- TEDI-READY maht ja sõltuvuste hulk ei kasva, harva kasutatava komponendi tõttu.
- Ei teki pidevalt kasvavat funktsionaalsussoovide järjekorda, mis sööks arendusmahtu muudelt komponentidelt.
- Ükski projekt ei ole sunnitud kasutama teeki, mis tema nõuetele ei sobi.
- TEDI ei võta endale litsentsi- ega hinnariski kolmanda osapoole toote pealt.

**Negatiivsed:**

- Iga projekt lahendab sama probleemi ise — dubleeriv töö.
- TextEditor'ite ühtsus projektide vahel ei ole tagatud, kuigi disainikomponent on olemas.
- Ligipääsetavuse (WCAG) tagamine jääb projektide kanda.
- Võib jätta mulje disainisüsteemi lüngast: disainis komponent on, arenduses mitte.

---

## 4. Alternatiivid

| Alternatiiv | Miks ei valitud |
| --- | --- |
| Oma lihtne TextEditor TEDI-READY-s | "Lihtne" ei jää lihtsaks — kohe järgnevad soovid tabelite, piltide jm osas. Piiritlematu hooldus- ja arenduskoormus. |
| Wrapper ühe konkreetse teegi (nt TinyMCE, CKEditor) ümber | Litsentsi- ja hinnarisk, sundvalik kõigile projektidele, kasvav bundle ja sõltuvus välise toote versioonipoliitikast. |
| Abstraktsioonikiht mitme teegi toetamiseks | Ebamõistlik hooldus- ja testimiskoormus; jääks teekide vähima ühisosa tasemele. |
| Eemaldada TextEditor ka disainist | Disainivajadus on reaalne; juhise puudumine muudaks lahendused veelgi ebaühtlasemaks. |

---

## 5. Järeldus

Nõuded on projektiti liiga erinevad, et neid keskselt mõistliku mahuga katta. Keskne lahendus tähendaks kas piiramatut arendusnõudlust või kõigi projektide sidumist ühe välise tootega, mille litsents ja tulevik ei ole TEDI kontrolli all. Kuna TextEditor'it vajab vaid osa projektidest, kaalub dubleeriv töö need riskid üles.

Otsus on tagasipööratav: kui selgub, et enamik projekte kasutab sama teeki, saab tuge järk-järgult lisada.

---

## 6. Seotud dokumendid / Tulevikutöö

- Disainisüsteemi TextEditor komponent (Figma).
- **Tulevikus võimalik:** pakkuda TEDI teemat (CSS/tokenid) populaarsetele teekidele, ilma teeki ennast sõltuvusena kaasamata. Kandidaadid: TinyMCE, CKEditor, TipTap, Lexical, Quill.
- Koguda projektidelt ülevaade reaalselt kasutatavatest teekidest, et teemastamise prioriteet paika panna.
