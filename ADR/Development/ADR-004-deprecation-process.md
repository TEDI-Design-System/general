# ADR-004: Komponentide deprecate'imise aken ja sammud

- **Staatus:** Proposed
- **Kuupäev:** 2026-09-18
- **ADR ID:** ADR-004
- **Otsuse tegijad:** Märt Sessman, Airike Jaska, Ly Tempel, Rando Leppik, Tõnis Tobre

---

## 1. Kontekst

### 1.1 Kuidas praegu käib

Komponendi mahakandmine koosneb täna kolmest tegevusest, mis kõik toimuvad **ühel ja samal hetkel**:

1. **Koodis** lisatakse `@deprecated` JSDoc-kommentaar, mis nimetab asenduse:

   ```
   // React, community/dropdown
   @deprecated Use `Dropdown` from `@tedi-design-system/react/tedi` instead.

   // Angular, community/tag
   @deprecated Use Tag from TEDI-ready instead. This component will be removed from future versions.
   ```

2. **Storybookis** märgitakse story staatusega
   `parameters: { status: { type: ["deprecated"] } }`. Märgise tekst on kõigil
   deprecated komponentidel ühine ja üldine: *"This component is deprecated and will be removed in a future
   release. Migrate to its replacement."*
3. **Main release'i märkmetes** tekib `### Deprecations` plokk: tabel veergudega Deprecated / Replacement /
   Since / Migration guide ja lause *"targeted for removal in {Kuu} {Aasta}"*, kus kuu on **kuus kuud**
   release'i kuupäevast. Migratsioonijuhised pannakse vastava rc-release'i kirjeldusse GitHubis.
4. **tedi.ee lehte** [Aeguvad komponendid](https://www.tedi.ee/1ee8444b7/p/87e621-aeguvad-komponendid)
   uuendatakse release'i protseduuri osana (issue #111).

### 1.2 Mis on puudu

- **Teavitus toimub ainult üks kord.** Deprecate'imise ja eemaldamise vahele jääb kuus (6) kuud, mille jooksul
  ühtegi meeldetuletust ei saadeta. Kui tarbija just release'i märkmeid ei lugenud, ei tea ta midagi.
- **Puudub vahesamm.** Komponent on kas täiesti tavaline (kuigi deprecated) või täielikult eemaldatud. Sõnumeid
  "ära hakka seda kasutama" ja "see lakkab töötamast" ei ole eristatud.
- **Puudub reegel selle kohta, mis juhtub, kui teavitus jäi tegemata.** Tähtaeg saabub, aga otsust ei ole
  millelegi toetada.

### 1.3 Konkreetne ajend

2026. aasta märtsi release'ides kuulutati välja esimesed eemaldamised septembriks. Väljakuulutamise järel
rohkem kommunikatsiooni ei toimunud. Seetõttu ei saa neid komponente septembris ohutult eemaldada:
eemaldamine võib olla tarbijarakendustele ootamatu *Breaking change*.

---

## 2. Otsus

### 2.1 Aken: 6 + 3 kuud

Deprecate'imise ja koodist eemaldamise vahele jääb üheksa kuud, mis jaguneb kaheks:

- **T0 kuni T+6:** komponent on deprecated, kuid dokumenteeritud ja Storybookis nähtav.
- **T+6 kuni T+9:** komponent on dokumentatsioonist eemaldatud, kuid koodis alles ja töötav. Viimane
  hoiatus on antud, migratsioon on kiireloomuline.

Aken hakkab jooksma main release'ist, mille märkmetes deprecate'imine välja kuulutatakse. Tähtajad on kuu täpsusega. Koodist eemaldamine on *breaking change*.

### 2.2 Kolm sammu

| Samm | Millal | Mis tehakse | *Breaking change* |
|------|--------|-------------|--------------------------|
| **1. Deprecate** | T0 | `@deprecated` koodis koos asendusega, runtime-hoiatus, deprecated-staatus Storybookis, rida release notes'i Deprecations-tabelis, migratsioonijuhis, kanne lehel Aeguvad komponendid | Ei |
| **2. Eemalda dokumentatsioon + viimane teavitus** | T+6 | Storybooki stoorid ja dokumentatsiooniviited eemaldatakse, komponent jääb ekspordituks ja töötavaks. Teates nimetatakse kuu, mil komponent koodist lõplikult eemaldatakse | Ei |
| **3. Eemalda koodist** | T+9 | Komponent eemaldatakse teegist, release notes'ides BREAKING CHANGE kirje | Jah |

Samm 2, dokumentatsiooni eemaldamine lõpetab komponendi leviku, sest uus arendaja ei leia seda enam Storybookist, kuid ei lõhu veel ühtegi olemasolevat rakendust.


### 2.3 Runtime-hoiatus

Deprecate'imisel lisatakse komponendile **arenduskeskkonna konsoolihoiatus**. `@deprecated` ja Storybooki
märgis eeldavad, et arendaja satub IDE tooltipi või Storybooki peale. Hoiatus jõuab kohale ka siis, kui ta
ainult jooksutab rakendust.

- Ainult arenduskeskkonnas: Angularis `isDevMode()`, Reactis `process.env.NODE_ENV !== 'production'`.
- Üks kord komponendi kohta, mitte iga renderdusega.
- Sisu on sama mis `@deprecated` tekstis: komponendi nimi ja asendus, ilma eemaldamise kuuta.

Muster on mõlemas teegis juba olemas, näiteks `tedi-radio-group` Angularis ja `TableCard` Reactis.

### 2.4 Viimane hoiatus ja edasilükkamine

Sammu 2 teade on sõnastatud tingimuslikult: komponent eemaldatakse koodist kuul X, kui ei ole mõjuvat põhjust
edasi lükata. Kes vajab migratsiooniks rohkem aega, annab sellest kolme kuu jooksul teada ja põhjendab. TEDI tiim
arutab selle arenduskoosolekul läbi ja kuulutab vajadusel välja uue tähtaja. Kui keegi ei reageeri, toimub
eemaldamine plaanipäraselt.

Komponenti **ei eemaldata koodist, kui samm 2 on tegemata**. Sellisel juhul tehakse samm 2 esimeses
võimalikus release'is ja sellesama teatega kuulutatakse välja uus eemaldamise kuu, mis ei ole varem kui kolm
kuud sellest teatest. Tegemata kommunikatsiooni tagantjärele ei kompenseerita. Just selle reegli puudumine
tekitas 2026. aasta septembri olukorra.

### 2.5 Teavitus ja tähtaegade jälgimine

Teavitus käib olemasolevaid kanaleid pidi: release notes, Slack, uudiskiri. Sammude 2 ja 3 puhul
on Slacki postitus eraldi postitus, mitte ainult release'i teade, ja nimetab komponendi, asenduse,
eemaldamise kuu ning lingi migratsioonijuhisele. Leht
[Aeguvad komponendid](https://www.tedi.ee/1ee8444b7/p/87e621-aeguvad-komponendid) on ainus koht, kus
nimekirja tervikuna hoitakse, ja seda uuendatakse igal sammul.

Eemaldamise kuud ei dubleerita `@deprecated` tekstis ega Storybooki märgisel. Teavitused ja release notes
katavad selle ära ning kuupäeva hoidmine mitmes kohas läheks paratamatult lahku.

Tähtaegu jälgitakse **release checklist'i** kaudu ([#112](https://github.com/TEDI-Design-System/general/issues/112)).
Checklist sisaldab punkti: luua iga release'i kohta üks issue, mis katab kõik komponendid, mille kuuekuuline
aken selles release'is täitub, ja mille sisu on nende dokumentatsiooni eemaldamine.

### 2.6 Üleminekuotsus

Seni välja kuulutatud kuupäevad on antud vana, ühesammulise mudeli järgi: release notes ütleb
*"targeted for removal in {kuu}"*, mis oli mõeldud koodist eemaldamise kuuna.

**Kõik seni väljakuulutatud tähtajad loetakse edaspidi dokumentatsioonist eemaldamise kuupäevadeks
(samm 2). Koodist eemaldamine toimub kolm kuud hiljem (samm 3).**

Näide: partii, mis deprecate'iti 2026. aasta märtsi release'is ja mille kohta öeldi "targeted for removal in
September 2026", eemaldatakse septembri release'is dokumentatsioonist ja jääb koodi alles. Sama release'i
märkmetes antakse viimane hoiatus, et koodist eemaldamine toimub detsembri 2026 release'is.

---

## 3. Tagajärjed

**Positiivsed:**

- Teine teade tuleb hetkel, mil sellega on veel võimalik midagi ette võtta, ja see ei ole ainult tekst:
  komponent kaob samal ajal Storybookist.
- Uus projekt ei saa enam kogemata kasutusele võtta komponenti, mis kolme kuu pärast kaob.
- Tarbijal on formaalne koht, kus öelda "vajame veel aega", ja see ei ole enam eskalatsioon vaid protsessi
  osa.
- Ükski juba välja kuulutatud tähtaeg ei lükku rohkem kui kolm kuud ja partiid liiguvad ühekaupa edasi.

**Negatiivsed:**

- Deprecated kood elab teegis üheksa kuud kuue asemel, seega on kaks lahendust kauem paralleelses hoolduses.
- Sammu 2 ja 3 vahel on komponent kasutatav, kuid dokumenteerimata. Leevendus: leht Aeguvad komponendid ja
  migratsioonijuhis jäävad kättesaadavaks.
- Tingimuslik sõnastus võib tekitada ootuse, et tähtaega saab alati venitada. Leevendus: põhjendus peab olema
  konkreetne ja otsustab tiim, mitte tarbija.

---

## 4. Alternatiivid

| Alternatiiv | Miks ei valitud |
|-------------|-----------------|
| Jätkata senise praktikaga | Eemaldamine oleks tarbijatele ootamatu murdev muudatus. |
| Jätta aken kuue kuu peale ja lisada ainult meeldetuletus | Dokumentatsiooni eemaldamine ei mahuks kuhugi: kas koos koodist eemaldamisega, mis ei anna mingit hoiatust, või enne seda, mis lühendaks dokumenteeritud perioodi alla kuue kuu. |

---

## 5. Järeldus

Senine protsess oli täielikult välja töötamata. Kuuekuuline aken oli mõistlik, kuid akna sees ei teavitatud kasutajaid
ja lõpus pidi korraga juhtuma kaks asja: tarbija pidi saama teavituse ja komponent pidi kaduma.

Uus mudel jagab selle kaheks. Kuue kuu pärast kaob komponent dokumentatsioonist ja sellega koos antakse
viimane hoiatus konkreetse kuuga. Kolm kuud hiljem kaob komponent koodist. Vahepealne olek, kus komponent
töötab, aga on dokumentatsioonist kadunud, ongi see sõnum, mida seni ei olnud võimalik edastada: ära hakka
seda enam kasutama, aga sinu rakendus ei ole veel katki.

---

## 6. Seotud dokumendid

- [2026-09-16 FE bi-weekly](../../Meeting%20notes/Development/2026-09-16%20FE%20bi-weekly.md)
- [Aeguvad komponendid](https://www.tedi.ee/1ee8444b7/p/87e621-aeguvad-komponendid) (issue
  [#111](https://github.com/TEDI-Design-System/general/issues/111))
- Issue [#112](https://github.com/TEDI-Design-System/general/issues/112): release checklist
