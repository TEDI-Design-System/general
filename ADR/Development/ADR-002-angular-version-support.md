# ADR-002: Uuendatud Angulari versioonitoe poliitika

- **Staatus:** Accepted
- **Kuupäev:** 2026-03-17
- **ADR ID:** ADR-002
- **Otsuse tegijad:** Märt Sessman, Tõnis Tobre

---

## 1. Kontekst

ADR-001 kehtestas poliitika, mille kohaselt TEDI toetab kuni ühe major-versiooni võrra vanemat Angulari versiooni paralleelselt uusimaga (kokku 2 versiooni).

Angular ise toetab ametlikult kolme viimast major-versiooni korraga (nt Angular 21 väljastamisel toetatakse v21, v20 ja v19). See tähendab, et paljud tarbijarakendused võivad vastata Angulari enda toepoliitikale, kuid jääda TEDI toepoliitikast välja.

Lisaks puudus selge ajakava, millal TEDI uue Angulari versiooni toe lisab ja vana eemaldab.

---

## 2. Otsus

TEDI hakkab Angulari puhul järgima [**Angulari enda versioonitoe mudelit**](https://angular.dev/reference/releases) — toetatakse **kolme viimast major-versiooni** korraga.

Ajakava:
- TEDI lisab uue Angulari major-versiooni toe **hiljemalt ühe kuu jooksul** pärast Angulari ametlikku väljalaset
- Vanima toetatud versiooni tugi eemaldatakse samal ajal uue versiooni toe lisamisega

Näide: kui Angular 22 ilmub, siis hiljemalt kuu aja jooksul lisatakse TEDI-sse Angular 22 tugi ja eemaldatakse Angular 19 tugi. Toetatakse v20, v21 ja v22.

Vanimate versioonide puhul kehtivad samad reeglid nagu ADR-001-s:
- Ainult hädavajalikud parandused (bugfixid, ligipääsetavuse parandused)
- Ei lisata uusi funktsioone ega komponente

---

## 3. Tagajärjed

**Positiivsed:**
- Tarbijarakendustel on rohkem aega migratsiooniks (3 versiooni aken vs 2)
- Ühtlustab TEDI toepoliitika Angulari enda omaga — vähem segadust tarbijate jaoks
- Selge ja prognoositav ajakava uue versiooni toe lisamiseks
- Migratsiooniaeg on paremini kooskõlas Reacti toepoliitikaga, kus major-versioonid ilmuvad oluliselt harvemini

**Negatiivsed:**
- Kolme versiooni paralleelne hooldus on suurem koormus kui kahe
- CI/CD peab tagama testide jooksmise kolme Angulari versiooni vastu

---

## 4. Alternatiivid

| Alternatiiv | Miks ei valitud |
|-------------|-----------------|
| Jätkata 2 versiooni toega (ADR-001) | Liiga kitsas aken tarbijarakenduste jaoks, ei ühti Angulari enda poliitikaga |

---

## 5. Järeldus

Kolme versiooni tugi on mõistlik kompromiss tarbijarakenduste vajaduste ja TEDI tiimi ressursside vahel. Kuuajaline puhver pärast ametlikku väljalaset annab piisavalt aega testimiseks ja migratsiooniks ilma et tekiks pikka viivitust.

---

## 6. Seotud dokumendid / Tulevikutöö

- ADR-001: Reacti ja Angulari versioonitoe poliitika
- [Angular versioning and releases](https://angular.dev/reference/releases)
