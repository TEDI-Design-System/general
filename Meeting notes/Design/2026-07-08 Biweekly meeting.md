# 2026-07-08 Regulaarne disainikoosolek

## AI kokkuvõte (kohandatud)

## Päevakord
- Release notes ülevaade
- Komponentide arendus ja disaini täiendused (card stepper, button group, pagination, footer)
- Disainisüsteemi refaktoreerimine ja komponentide liigitus
- Uued funktsioonid (slider error, attachment slot, card button slot, läbipaistvad variandid)
- Komponentide tarned Reactis ja Angularis
- Kommunikatsiooni ja protsesside täiustused

## Komponentide arendus ja disaini täiendused

Peamine fookus oli uute ja olemasolevate komponentide täiendamisel ning nende eraldamisel sõltumatuteks kasutusjuhtudeks.

- Card stepper ja vertikaalne stepper on Figma's nüüd eraldi frame-il, eraldi komponendid
- Propertite abil saab juhtida sammude numbrinäitamist, progressibaari kuvamist ja navigeerimisnuppe
- Komponent toetab alumise sloti lisamist olekute ja nuppude jaoks, mis laiendab kasutusvõimalusi
- Button group erineb tavalisest nupust väikese nurgakraadi ja värviskeemiga; Figma's lisati variatsioon tavaliste nuppude hulka juurde, et hoida disain ja arendus sünkroonis
- Tulevikus plaanitakse button groupi komponendi sees Figmas nupud ümber vahetada
- Pagination komponent sai eraldi separatori propertid ja sloti, mis võimaldab kuvada erinevaid teavitusi ja olekuid
- Footeri struktuur lihtsustati ja lisati slotid – enne oli mitu varianti, nüüd saab dividereid ja logosid lisada sloti kaudu

## Disainisüsteemi refaktoreerimine ja komponentide liigitus

Suur osa tööst keskendus komponentide ümberpaigutamisele, lihtsustamisele ja nimetuste ühtlustamisele.

- Kalendri päevade suurus sai muudetud skaleeritavaks;
- Horizontal navigation muudeti top navigationiks;
- Stepperid said selgemad nimetused;
- Collapse muudeti collapse buttoniks;
- Näidete keel muudetakse järk-järgult eestikeelseks, et parandada arusaadavust projektides
- Community Figma muutujaid eemaldati ristkasutuse vältimiseks;
- Legend ja sheet komponendid liiguvad TEDI-readysse dubleerimise vähendamiseks
- Resizer komponenti kaalutakse värvimuudatuseks, et sobiks neutraalsemate keskkondadega

## Uued funktsioonid ja kasutusvõimaluste laiendused

- Sliderile lisati errori olek, mis vastab teistele vormielementidele (kuigi kasutus on pigem harv) – näitab valimata või sobimatu väärtuse situatsioone
- Attachment komponent sai võimaluse nuppe lisada action sloti kaudu; Close asendati Delete'ga, mis on kasutajale arusaadavam
- Card button sai sloti, mis võimaldab lisada paindlikult erinevat sisu ja olekuid ilma keeruliste propertideta
- See mõjutas ka card stepperi mobiilse lahenduse lihtsustamist, asendades varasemad eraldi mobiilipatternid
- Lisati läbipaistev variant sisukorrale ja teistele kaartidele – säilitab visuaalse piiri, kuid kaotab jäiga valge tausta
- Mitmed vananenud või dubleeritud variandid eemaldati: mobiili card stepperid asendati card buttoniga, karusselli mobiiliversioonid vähendati

## Komponentide tarned Reactis ja Angularis

Arenduse poolelt valmis märkimisväärne hulk komponente mõlemas raamistikus.

## Kommunikatsioon ja protsessid

- Kärolin palus küsimuste korral eelistada disainikanalit, mitte otse temale kirjutamist tema puhkuse ajal
- Marta ja teised disainerid on valmis küsimustele vastama, mis parandab reageerimiskiirust

## Otsused

### TEDI tiim
- Parandada kalenderi weekcount kuvamise skaleeritavust
- Koordineerida komponentide üleviimist Map componentsist TEDI-readysse (colorpicker, legend, sheet, resizer)

## Eelmistest koosolekutest veel üleval
- Figma Make ja TEDI kooslus vajab veel testimist – testitud varasemas etapis, võimalik et Make on arenenud
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus
- Vertical stepperi alamsammude kuvamine mobiilis
- TTJA NBA, Rahvastikuregistri menetluskeskkond: vajadus tabelis/lingil eristada külastatud ja külastamata olekuid
- Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis konflikti kui headeris kõik väärtused sisse lülitada; brand värvi peal pole searchi hint näha
