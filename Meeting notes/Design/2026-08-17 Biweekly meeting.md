# Peamised punktid

## Disainisüsteemi komponendid ja arendus
- TableCard sai tabeli komponendi nimeks, mis ei seostu ainult mobiiliga. Hidden input komponent näeb välja nagu read-only tekst ja muutub klikiga sisestusväljaks; komponendi nimi on veel arutlusel.
- Tekstiredaktori komponenti TEDI ei arenda — soovitatakse kasutada väliseid teeke, mida saab TEDI stiilidega kohandada. Kasutus jääb projektipõhiseks ja sellega kaasneb juhend.
- Sheet komponent liigub Map Components alamsüsteemist TEDI põhikomponentide alla, kuna see pole kaardispetsiifiline. Lisanduvad kaardi alt TEDI-Readysse ka color picker, icon picker ja resizer komponendid.
- Angularis käib külgmenüü refaktoreerimine; külgmenüü 3. tase taab uue näo parema kasutuskogemuse nimel.
- Eelmise disainisüsteemi Choice Group komponent kaotatakse Reactist -> radiod ja checkboxid liiguvad eraldi oma õigete nimede alla.
- Figma Make disainikit uuendati, mis lihtsustab Reacti komponentide kasutust; Claude Designi jaoks valmib juhend ja süsteemipõhi.

## Komponentide paindlikkus ja slot'ide süsteem (dicussionitele vastamine)
- Komponendid on üles ehitatud slot'idele (päised, jalused, ikoonid) ning neid saab projektipõhiselt laiendada ja muutujaid (nt värve, taustu) ülekirjutada -> kõiki vajadusi ei tule TEDisse kuid selleks on võimalus ise täiendada.
- Kaardi komponent defineerib vaid välimuse (padding, border, raadius); kogu sisu on slot'is, nii saab teha näiteks klikitava toggle card'i.
- Card button on üles ehitatud slot'idele — hover- ja aktiivseisundi värvid on defineeritud, sisu ehitatakse slot'idega, mis vähendab propertite arvu.
- Table alert item on kaart (värviline border), mida saab mobiili- ja tahvelvaates kasutada tabeli asemel -> selle saab samuti Card komponendist ise ehitada.
- Popover komponendile lisatakse footer slot ja propertid asendatakse slot'idega, mis muudab komponendi paindlikumaks (võib mõjutada prototüüpimist — komponendiuuendustes on hoiatused).

## Värvid ja muutujad
- Tag komponentidele võib tulla juurde positiivse oleku (success) värv senise danger-põhise kõrvale kui ka teistel projektidel on huvi selle vastu; projekte kutsutakse üles vajalikke värve ja omadusi arutelus üles märkima.
- Projektid saavad TEDI muutujaid ülekirjutada oma värvide, fontide ja semantiliste muutujatega (nt muuseumide infosüsteemil on oma disainisüsteem TEDI muutujate baasil); Figma ja arendus püsivad sünkroonis.
- Juhul kui projekt muudab värve siis kontrollida taustade kontrast (eesmärk 3:1); 
- Figma muutujate publishimise bug on lahendamisel; muutujate uuendusi hoitakse seni tagasi, et mitte mõjutada projekte.

## Prototüüpimine ja tööriistad
- TEDI Figma failis saab hallata mitut tiimi ja projekti; Projekte julgustatakse TEDI failiga siduma, et uuendused jõuaksid automaatselt kätte.
- Spinneri komponendile soovitakse lisada laadimist kirjeldav tekst; praegu lahendatakse see placeholderi ja ikooni vahetusega, standardiseerimine on arutlusel.
- Küsimusi ja probleeme esitada disainikanalis, et teisedki näeksid ja saaksid aidata; konfidentsiaalsem suhtlus käib Slackis otsekontaktina või porjekti grupis.

# Otsused
- Tekstiredaktori komponenti ei arendata — soovitatakse väliseid teeke, mida saab TEDI stiilidega kohandada (projektipõhine, koos juhendiga).
- Sheet komponent tõstetakse TEDI põhikomponentide alla, kuna see pole kaardispetsiifiline.
- Eelmise disainisüsteemi Choice Group komponent kaotatakse; radiod ja checkboxid liiguvad eraldi oma nimede alla.
- Popover komponendile lisatakse footer slot ja propertid asendatakse slot'idega.
- Figma muutujate uuendusi hoitakse tagasi, kuni publishimise bug on lahendatud.

## Eelmine koosolek
- Edastada arendajatele otsus "clear button" (x) kuvamise ja selle property-te juhtimise kohta projektides

**Projektide disainerid**
- Saata Kärolinile TEDi komponente kasutavate projektide lingid, et koguda reaalseid kasutusnäiteid ja mõista paremini kasutusolukordi
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus
- TTJA NBA, Rahvastikuregistri menetluskeskkond: vajadus tabelis/lingil eristada külastatud ja külastamata olekuid
- Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis konflikti kui headeris kõik väärtused sisse lülitada; brand värvi peal pole searchi hint näha

**Arendusmeeskond**
- Viia läbi külgmenüü refaktooring ja disainiuuendused kolmanda taseme menüü lihtsustamiseks.
- Jätkata rating komponendi arendamist ja disainiuuenduste rakendamist.
- Teha radionuppudel ja checkboxidel vajalikud muudatused ning eemaldada Choice Group komponent.
