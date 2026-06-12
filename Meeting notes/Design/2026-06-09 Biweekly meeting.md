# 2026-06-09 Biweekly meeting

## AI kokkuvõte (kohandatud)

### Peamised punktid

- **Slotide lisamine:** Futterite lisati slotid, mis suurendavad paindlikkust ja võimaldavad sisu hõlpsammat kohandamist.
- **Komponentide liikumine:** Rikkalikud komponendid liiguvad community-st Teddy Redisse, järgides arendusstandardeid.
- **Otsinguteate kuvamine:** Eelistatud on kuvada teadet "tulemusi ei leitud" mitte errorina.
- **Tooltipide värvi arutelu:** Lisada heledat varianti, et eristada abiteksti tumehallist.
- **Nuppude paigutuse probleem:** Tegevusnupud võivad kattuda katkeva tekstiga; arutelud lahendustest on vajalikud.
- **Kommunikatsiooni kokkulepped:** Suurematest muudatustest tuleb teavitada; prototüüpide stabiilsus on oluline.

## Päevakord

## Komponentide ja Figma muudatused

- Kärolin selgitas, et futteri komponentidele lisati slotid, mis võimaldavad paindlikumat sisu lisamist ilma olemasolevaid futtere rikkumata (00:23)
- Slotid võimaldavad paigutada mis tahes sisu, näiteks logod või linke, ning need asendavad eelnevaid propertite piiranguid, suurendades kohandatavust
- Footeril säilitati eraldi propertid nagu "show logo right/left", et olemasolevaid futtere ei rikuta, kuid sloti kasutamine annab rohkem vabadust sisu paigutamisel
- Näidiste sisu muudeti eestikeelseks, sest see sobib paremini arenduse ja prototüüpimise vajadustega, kuigi komparandi nimed jäävad ingliskeelseks (02:15)
- Footeris eemaldati mitmed keerukad variatsioonid ja akordionid asendati slotipõhise lahendusega, mis lihtsustab komponenti ja võimaldab kasutajal ise sobivaid elemente lisada (05:08)
- Kärolin tutvustas ka transparent pagination komponenti, kus eraldi eraldati ja sisse-välja lülitatav separaator, mis mõjutab prototüüpe (08:36)
- Transparent variandil tuleb sama funktsionaalsus nagu valgel variandil, sest border on seal vaikimisi sees, kuid kasutaja saab eraldi määrata separaatori kuvamise
- Uuendus peaks jõudma prototüüpidesse selle nädala või järgmise alguses, mille kohta antakse ka muudatuste info

## Komponentide struktuuri ümberkorraldus ja Teddy Redise liikumine

- Kärolin teavitas, et mitmed komponendid liiguvad community-st Teddy Redisse, näiteks karussell ja kolori-ikoonpicker, et tagada paremat vastavust Tediredi arendusstandarditele (18:01)
- Teddy Kit sisaldab nüüd ka Figma Make jaoks mõeldud kaidlaine komplekti, mis kasutab Tediredi ja community komponente ning aitab arendust vastavalt WCAG nõuetele suunata
- Teddy Redise uuendusi plaanitakse teha igakuise release raames, et hoida stabiilsust ja kaasajastada komponente pidevalt (24:38)
- Komponentide ümberpaigutus ei riku prototüüpe, sest algfaili asukoha muutmine ei mõjuta visuaali otseselt, kuid mõnda komponendi allikat tuleb vahetada (21:05)

## Otsinguväljale tulemusteta otsingu teadete kuvamine

- Piret küsis otsingu tulemuste puudumise teatamise viisi kohta, kas kuvada errorina või lihtsalt teadet (25:49)
- Kärolini soovitus on mitte panna otsinguvälja error-staatusse, vaid kuvada tulemuste alal selge teadet, et "tulemusi ei leitud" või "kontrolli sisestatud numbrit"
- Kui otsingutulemusi kuvatakse kogu lehel, siis võib kuvada vastava teadete ala, mis ei sega otsinguvälja kasutamist ega tekitaks vääritimõistmisi
- Arutelu jätkub, kuid hetkel kaldutakse eelistama tulemuste ala selgitust, mitte otsinguvälja errorit (27:54)

## Tooltipide taustavärvi valikud ja disainiarutelu

- Lauri tõi välja, et TED-i projektis on tooltipide taust värvitud tumedamaks halliks, kuid sooviks Tediredis lisada ka heledat varianti (29:48)
- Kärolin selgitas, et tooltip on abitekstina mõeldud heledas toonis, et eristuda ja jääda loetavaks, samas kui popoverid on pikemate tekstide jaoks tumedamad
- Tooltipi värvi on võimalik disainis ja arenduses üle kirjutada, kuid selgitustöö disainiaruteluks on vajalik, sest hele värv aitab juhendavat teksti esile tõsta
- Lauri märkis, et arendajate seas on tekkinud küsimusi halli värvi kasutamise kohta, seega lisavärvi valik toetaks erinevaid vajadusi ja kasutusjuhtumeid (32:49)

## Tegevusnuppude ja teksti paigutuse probleemid nimekirjakomponendis

- Helis tõi esile, et ühes projektis on muuda ja kustuta nupud paigutatud paremale ülesnurka, kuid pealkirja pole, ainult description-tekst (34:01)
- Probleem on, et tegevusnupud võivad katkeva teksti tõttu katta või olla kehvasti nähtavad, kuna nuppude paigutus ei toeta kõrvale lisamist
- Kärolin soovitas, et Helis võiks teha diskusiooni, lisades prototüübid ja ekraanipildid, et täpsemalt lahendusi leida ning vajadusel teha komponentidesse täiendusi
- Kiire lahendus on tegevusnuppe all jätta, kuid pikemas perspektiivis võiks komponent toetada kõrvale paigutust, kus descriptioni tekst kitseneb ja nupud joondatakse ülemisse paremasse nurka (41:15)

## Disaini muutuste ja kommunikatsiooni kokkulepped

- Kärolin pakkus, et väiksemate komponentide muudatustest ja failide ümberpaigutustest võiks teavitada disaini kanalites, kuid Helis ja Lauri leiavad, et otsing ja Figma võimaldavad muudatusi kiirelt üles leida, seega eraldi teavitusi pole vaja (15:43)
- Kärolin rõhutas, et slotide lisamine olemasolevatesse komponentidesse võib mõjutada prototüüpe, mistõttu on oluline märkida suuremad muudatused ja aidata leida võimalikke anomaaliaid varakult (48:06)
- Samuti on plaanis uurida ja vajadusel uuendada Figma Make ja Teddy Redise vahelisi integratsioone ning versioonihaldust, et tagada sujuvam arendusprotsess (24:38)
- Prototüüpide katkemise riski puhul kaalutakse komponentide täielikku asendamist uute versioonidega, et hoida prototüüpide stabiilsust ja vältida ootamatuid rikkeid (14:52)

## Otsused

### TEDI tiim

- Kärolin Kivisikk
  - Mõõdab ja testib slotide kasutuse mõjusid footer komponendis ja nende mõju prototüüpidele (00:00)
  - Täiendab ja otsustab asseti sisu eestikeelsete näidiste osas ning teavitab grupi valitud lähenemisest (03:00)
  - Jälgib transparent pagination separaatori lisandite ja selle kasutuselevõttu ning informeerib uuendustest (08:00)
  - Uuendab accordion ja collapse komponentide sidusust ning kaalub breaking change riske prototüüpidele (12:00)
  - Korraldab komponentide kaustade korrastamise protsessi ning otsustab disainiteavituste vajaduse (15:00)
  - Korraldab TEDI ja Teddy Redisse komponentide ülekandmise ning jälgib arendusesüsteemi uuendusi (18:00)
  - Uurib Teddy Kiti Figma Make keskkonna uuendamise võimalusi ja stabiilsust (21:00)
  - Arutab otsingu error state lahenduse kohta ja avaldab soovitusi otsingu käitumise optimeerimiseks (26:00)
  - Korraldab tooltipi värvivalikute diskussiooni ning pakub välja eri variandit kasutamiseks projektide erinevates tingimustes (29:00)
  - Kogub ja analüüsib inpute tegevusnuppude paigutuse probleemide kohta ning kutsub üles arendama vastavaid lahendusi (33:00)
  - Jälgib Euroopa Liidu toetuse logo sobivust footer/is headeri paigutustesse ja vajadusel arutab disainilahenduse kohta (44:00)
  - Teavitab design-kanalisse võimalikest prototüüpide mõjust (slotid, paigutused) ja parandustest (47:00)

### Projektide disainerid

- Piret Tabor
  - Selgitab otsingu error state'i kasutajateadete osas ja teeb täpsustusi vajadustele (25:00)
- Helis Sepp
  - Kogub infot ja dokumenteerib tegevusnuppude paigutuse probleemid konkreetsetes rakendustes, paneb vajalikud info ja prototüübid diskussiooni (33:00)
  - Osaleb tooltipi teemalises disainikõnes (29:00)
- Lauri Tõnisson
  - Esitab ettepaneku tooltipi värvivalikute osas Teddy Redis ja TEDi keskkondade ühtlustamiseks (29:00)
