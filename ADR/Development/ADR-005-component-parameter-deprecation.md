# ADR-005: Komponendi API parameetrite deprecate'imine

- **Staatus:** Proposed
- **Kuupäev:** 2026-10-05
- **ADR ID:** ADR-005
- **Otsuse tegijad:** Märt Sessman, Airike Jaska, Ly Tempel, Tõnis Tobre

---

## 1. Kontekst

[ADR-004](ADR-004-deprecation-process.md) kirjeldab terve komponendi deprecate'imist. Mõnikord on deprecated
aga ainult komponendi üksikud API parameetrid (Reactis propid, Angularis inputid ja outputid). Nende kohta
ühest reeglit ei ole.

Praktikas muudetakse parameetri nimi enamasti kohe ja see on *breaking change*. Harvem on vana nimi jäetud
`@deprecated` annotatsiooniga alles, kuigi ka need on olnud lihtsad ümbernimetamised.

---

## 2. Otsus

**Nime muutmine:** kui parameetri nimi muutub ja käitumine jääb samaks, eemaldatakse vana nimi kohe. Muudatus
on *breaking change* ja release notes kirjeldab migratsiooni (vana nimi → uus nimi). Vana nime ei jäeta
`@deprecated` annotatsiooniga alles.

**Suurem API muudatus:** kui komponendi API muutub rohkem kui ainult nime poolest, võib TEDI tiim otsustada
anda tarbijatele migratsiooniks aega. Sel juhul järgitakse ADR-004 akent ja samme.

---

## 3. Tagajärjed

**Positiivsed:**

- Teeki ei kogune vanu parameetrinimesid, mida tuleks uute kõrval hooldada.
- Ümbernimetamise järel on migratsioon väike ja release notes'i järgi kiiresti tehtav.

**Negatiivsed:**

- Ka väike ümbernimetamine on *breaking change*: uuendades peab tarbija oma koodi muutma.

---

## 4. Alternatiivid

| Alternatiiv | Miks ei valitud |
|-------------|-----------------|
| ADR-004 aken kõigile parameetrimuudatustele | Nii väikese muudatuse jaoks on hoolduskulu liiga suur. |

---

## 5. Seotud dokumendid

- [ADR-004: Komponentide deprecate'imise aken ja sammud](ADR-004-deprecation-process.md)
