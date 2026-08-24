# Peamised punktid

## Disainisüsteemi komponendid ja arendus
- TableGuard sai nimeks mobiili tabeli komponent, mis ei seostu ainult mobiiliga. Hidden input komponent näeb välja nagu read-only tekst ja muutub klikiga sisestusväljaks; komponendi nimi on veel arutlusel.
- Tekstiredaktori komponenti TEDI ei arenda — soovitatakse kasutada väliseid teeke, mida saab TEDI stiilidega kohandada. Kasutus jääb projektipõhiseks ja sellega kaasneb juhend.
- Sheet komponent liigub Map Components alamsüsteemist TEDI põhikomponentide alla, kuna see pole kaardispetsiifiline. Lisanduvad color picker, icon picker ja resizer komponendid.
- Angularis käib tabeli ja külgmenüü refaktoreerimine; külgmenüü sügavust vähendatakse parema kasutuskogemuse nimel.
- Eelmise disainisüsteemi Choice Group komponent kaotatakse; radiod ja checkboxid liiguvad eraldi oma nimede alla.
- Figma Make disainikit uuendati, mis lihtsustab Reacti komponentide kasutust; Cloud Designi jaoks valmib juhend ja süsteemipõhi.

## Komponentide paindlikkus ja slot'ide süsteem
- Komponendid on üles ehitatud slot'idele (päised, jalused, ikoonid) ning neid saab projektipõhiselt laiendada ja muutujaid (nt värve, taustu) ülekirjutada.
- Kaardi komponent defineerib vaid välimuse (padding, border, raadius); kogu sisu on slot'is, nii saab teha näiteks klikitava toggle card'i.
- Card button on üles ehitatud slot'idele — hover- ja aktiivseisundi värvid on defineeritud, sisu ehitatakse slot'idega, mis vähendab propertite arvu.
- Table alert item on kaart tabeliridadest (värviline ikoon, vasak border), mida saab mobiili- ja tahvelvaates kasutada tabeli asemel.
- Popover komponendile lisatakse footer slot ja propertid asendatakse slot'idega, mis muudab komponendi paindlikumaks (võib mõjutada prototüüpimist — komponendiuuendustes on hoiatused).

## Värvid ja muutujad
- Tag komponentidele lisatakse positiivse oleku (success) värv senise danger-põhise kõrvale; projekte kutsutakse üles vajalikke värve ja omadusi arutelus üles märkima.
- Projektid saavad TEDI muutujaid ülekirjutada oma värvide, fontide ja semantiliste muutujatega (nt muuseumide infosüsteemil on oma disainisüsteem TEDI muutujate baasil); Figma ja arendus püsivad sünkroonis.
- Vaadatakse üle nupugruppide ja kaartide nurgaradiused ning sekundaarsete taustade kontrast (eesmärk 3:1); borderi laius muudetakse paindlikuks nii Figmas kui ka arenduses.
- Figma muutujate publishimise bug on lahendamisel; muutujate uuendusi hoitakse seni tagasi, et mitte mõjutada projekte.

## Prototüüpimine ja tööriistad
- TEDI Figma failis saab hallata mitut tiimi ja projekti; Riia projektil on oma pesa. Projekte julgustatakse TEDI failiga siduma, et uuendused jõuaksid automaatselt kätte.
- Spinneri komponendile soovitakse lisada laadimist kirjeldav tekst; praegu lahendatakse see placeholderi ja ikooni vahetusega, standardiseerimine on arutlusel.
- Küsimusi ja probleeme eelistatakse esitada disainikanalis, et teisedki näeksid ja saaksid aidata; konfidentsiaalsem suhtlus käib Slackis otsekontaktina.

# Otsused
- Tekstiredaktori komponenti ei arendata — soovitatakse väliseid teeke, mida saab TEDI stiilidega kohandada (projektipõhine, koos juhendiga).
- Sheet komponent tõstetakse TEDI põhikomponentide alla, kuna see pole kaardispetsiifiline.
- Eelmise disainisüsteemi Choice Group komponent kaotatakse; radiod ja checkboxid liiguvad eraldi oma nimede alla.
- Tag komponentidele lisatakse positiivse oleku (success) variant.
- Popover komponendile lisatakse footer slot ja propertid asendatakse slot'idega.
- Figma muutujate uuendusi hoitakse tagasi, kuni publishimise bug on lahendatud.

<!-- Eelmiste koosolekute Otsused lisatakse siia. Palun kleebi 2026-08-03 Biweekly meeting.md faili "Otsused" osa, et need edasi kanda. -->

# Tegevused

**Disainer**
- Jagada tekstiredaktori komponendi juhendit ja soovitatud teegi valikut projektidele.
- Kirjutada dokument tehniliste juhistega clear button'i haldamiseks (hover ja nähtavus).
- Näidata järgmisel kohtumisel TEDIS-EVI brändielemente ja selgitada nende rolli.
- Ümber paigutada ja refaktoreerida Sheet komponent Figmas ning jälgida komponentide veatut toimimist.
- Lahendada Figma muutujate publishimise bug ja hoida muutujate uuendused kontrolli all.
- Uuendada ja jagada Figma Make kit'i ning valmistada Cloud Designi juhend.
- Korraldada Figma diskussioonid värvide ja Accordioni osas ning vastata laekunud küsimustele.
- Täiendada Accordion komponendi slotte (header, footer), võimaldades paindlikke muudatusi.
- Toetada ja juhendada TEDI komponentide laiendamist ja ülekirjutamist projektides Figmas.
- Arendada ja tutvustada card button ja table alert item komponente vastavalt kasutusvajadustele.
- Aidata kasutajatel organiseerida TEDI Figma faile mitme tiimi ja projekti lõikes.
- Lisada Textgroup komponendile slot, et võimaldada erinevaid elemente (nupud, lingid).
- Koostada 24-pikslise kopeerimisnupu hover- ja fookusstaatustega variant.
- Algatada diskussioon spinneri komponendi tekstikirjelduse lisamise vajaduse üle.

**Arendusmeeskond**
- Viia läbi külgmenüü refaktooring ja disainiuuendused kolmanda taseme menüü lihtsustamiseks.
- Jätkata rating komponendi arendamist ja disainiuuenduste rakendamist.
- Teha radioknuppudel ja checkboxidel vajalikud muudatused ning eemaldada Choice Group komponent.
