# 2026-01-05 Regulaarne disainikoosolek

## Osalejad
- Saskia Sonnberg
- Kristel Ojamaa
- Gerli Liiv
- Katre Suits
- Fireflies AI notetaker
- Piret Tabor
- Kätrin Uduste
- Karis Karindi
- Lauri Tõnisson
- Joanna Joa
- Kärol-Milaine Puunurm
- Henry Semmel
- Norman Järve
- Helis Sepp
- Siret Tuula

https://bitwebou-my.sharepoint.com/:v:/r/personal/karolin_kivisikk_bitweb_ee/Documents/Recordings/Disaineritele%20TEDI%20komponendid-20260105_155752-Meeting%20Recording.mp4?csf=1&web=1&e=rAqKEy&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
Kokkuvõte on koostöös Fireflies AI-ga koostatud

# Kokkuvõte
* Filtrikomponentide eristamine checkbox cardist, nii nimetuselt kui visuaalilt - läheb ka arendajate lauale arutelule
* Otsingupäise täiustused: otsingu lisamine headerisse
* Tagasiside vormi komponendi lisandumine
* Komponentide haldus: Jaanuari lõpuks eemaldatakse vananenud komponendid, vähendades dubleerimist.

# Filtrikomponentide uuendus ja standardiseerimine
* Filtrikomponentid ja checkbox cardi komponendi nimed ja funktsionaalsus vajavad selgemat jaotust. Arenduses on nende nimeks choicegroup - ei ole üldtuntud nimetus. Nime ja atribuutide muutus lõhub protosid seega kõige ohutum on eelmine komponent TEDI-Readyst kustutada ning luua 2 uut - checkbox card/radio card ning filter.
* Kärolin Kivisikk tegi ettepaneku eristada filtrikomponent (multiselektiga ja linnukese indikaatoriga) ja checkbox kaart (alati checkboxiga, ilma automaatse linnukeseta), et vältida segadust ja prototüüpide katkestamist (06:01)
* Filtrikomponendil kuvatakse indikaator kui filter on valitud
* Checkbox kaart jääb samasuguseks nagu praegu, aga sellel ei oleks võimalik ilma indikaatorita varianti enam kasutada, see property oleks sisse lülitatud ning eemaldada seda ei saaks
* Kärolin koostab koos arendajatega plaani nimede ja komponentide lõplikuks kinnistamiseks ja avalikustamiseks
* Joanna Joa toetas kahte uut komponenti ning rõhutas, et vastutus korrektsuse eest jääb projektide tiimidele (20:25)
* Piret Tabor tõi välja keerulisema kasutusjuhtumi, kus checkbox kaart on kombineeritud lisateavituse mummuga - tegu on custom lahendusega (23:20)
  * Selle lahendamiseks sai soovitatud tagi kasutamist numbriga või mummu liigutamist filtri lõppu, kuna algusesse tuleb nüüd linnukese ikoon
  * Arutleti, kas lisateavitused nagu "mummuke" või täg võiksid filtreerimise selgust parandada, kuid selgus, et neid tuleks kasutajatega testida, kuna tähendused võivad jääda segaseks
  * Kärolin soovitas teha kasutajauuringuid, et mõista selgelt, kuidas kasutajad selliseid visuaale tõlgendavad
  * Sellised täiendavad indikaatorid võivad parandada tähelepanu juhtimist, kuid võivad ka tekitada segadust, kui pole piisavalt selged
* Joanna Joa ja Kärolin arutasid filtrite ühtlustamist süsteemis, eriti tabeli kohal olevate ja lehe ülemiste filtrite vahel - neid kasutatakse nt STARis ristirästi. Osad filtrid on tabelis osad tabeli kohal, lisaks peaks või võiks olla lahendatud ka tabeli filtrite korraga tühistamine. (28:11)
  * Nähti vajadust ühise nupu järele, mis tühistab kõik filtrid korraga, et parandada kasutuskogemust
  * Rõhutati, et filtrite ristkasutus eri vaadetes võib tekitada segadust, mistõttu peaks olema selge, kus ja kuidas filtrid kuvatakse
  * Kärolin kavatseb lisada näidise ühise filtrite tühistamise nupuga ka filtrite sektsiooni

# Otsing päisesse
* Uus otsingupäis toetab nii desktopi kui mobiilivaateid ja võimaldab kasutajatel mugavalt otsida üle süsteemi
* Kärolin Kivisikk lisas desktopile ja tahvelarvutile otsinguväljale mugavuse, mobiilile aga nupu, mis avab otsingu modaalaknas, vältides ruumipuudust (39:14)
* Mobiiliversioon võimaldab otsingut avada eraldi vaates, mis ei koorma navigeerimisriba
* Desktopiversioonis on otsing nähtav navigeerimisriba kõrval, kuid vajadusel saab seda laiendada
* Kasutajate tagasiside kogumine selgitab, kas olemasolev lahendus katab erinevate projektide vajadused
* Piret Tabor tõi välja, et nende sisemises süsteemis on otsing väga oluline, kuid navigeerimisribal on vähe ruumi kuna headerisse on lisatud ka lingid.
* Kärolin kavandab vajaduspõhiseid kohandusi, kuid praegu ootab, kas keegi soovib uut otsingukomponenti aktiivselt kasutusele võtta (46:10)
* Ta rõhutas, et lahendus on ehitatud Veera Designi ideede põhjal ja ootab täiendavat tagasisidet
* Henry Semmel pakkus välja otsingu nagu tallinn.ee kasutab ehk et tegu on vaid otsingunupuga kuid peale klikates muutub terve päis otsinguväljaks, selliselt võtab see algupäraselt vähem ruumi.
  
# Uus tagasisidevormi komponent
* Tagasiside vormi komponent võimaldab kasutajal valida tähekeste ikoonidega hinnanguid ja saata tagasisidet, laiendades kasutajate kaasamist.
* Kärolin Kivisikk tutvustas uut tagasisidevormi komponenti, mis võimaldab tähtede abil hinnata ja lisaks valida lisavõimalusi (48:23)
* Komponent on ehitatud olemasolevate elementide põhjal ja võimaldab kasutajatel hinnata erinevaid kategooriaid
* Disain võimaldab tähtedele lisada taustavärvi või muuta läbipaistvust vastavalt vajadusele
* Helis Sepp tõi välja vajaduse erinevate skaalade järele, näiteks 1–10, sest 5-tärni süsteem ei pruugi kõigile sobida (52:53)
* Kärolin lubas uurida ja vajadusel lisada ka numbrilise skaalaga variante, sest 10-tärni puhul võib visuaalne loetavus kannatada
* Kärolin plaanib viia tagasisidevormi veel viimasele disaini ülevaatusele ja juurdepääsetavuse kontrollile (VCAG), enne kui avalikustada (49:03)

# Muutujate haldus, Figma uuendused disainisüsteemis ja muu
* Muutujate haldus muutub selgemaks ja paindlikumaks, võimaldades projektidel iseseisvalt värve, suuruseid, kumerusi, paksus, kaugusi kohandada
  * Projektitiimidel on nüüd võimalik Figma uue funktsiooni abil lokaalselt muuta ja üleväärtustada TEDI-Readys olevaid muutujad (58:55)
  * See võimaldab näiteks muuta nupu värvi või nurga raadiust projektipõhiselt ilma põhikomponenti muutmata
  * Kärolin plaanib järgmisel koosolekul näidata, kuidas seda funktsiooni kasutada, mis aitab arendajatel ja disaineritel projektipõhiseid erisusi paremini hallata
  * See muudatus vähendab TEDI tiimi koormust ja toetab paindlikkust erinevate projektide vajaduste rahuldamisel
* Kärolin Kivisikk teatas, et jaanuari lõpus kustutatakse community failist osad vananenud komponendid, millel on TEDi redis juba vasted olemas (55:55)
  * See puhastab komponente ja vähendab dubleerimist, parandades süsteemi haldamist
* Kõik TEDi kasutajad saavad nüüd community faili redigeerida, mis soodustab uute komponentide kiiremat loomist ja jagamist

## Otsused
* Filtrikomponendi nimetamine, uue loomine, arutelud arendusega - breaking change
* Uurida arendajate käest, kus ja kuidas kasutatakse väikest filtrisuurust ning kas seda on vaja hoida alles või võib eemaldada.
* Otsingu desgin review
* Feedback komponendi design review ja 10 arvuga arvestamine

Eelmistest koosolekutest veel üleval:
* Vertical stepperi alamsammude kuvamine mobiilis
* Välisveebi komponentide vajaduste ja näidete kogumine
* Arvestada sooviga et arenduses saaks horisontaalset nav-i panna stickyma scrollimise peale
* Mõelda mis hetkest või loogika alusel horisontaalne menüü läheb mobiilseks - kas võimalik hallata arenduses et jääb kauemaks mittemobiilseks kui linke on vähem menüüs
* TTJA NBA, Rahvastikuregustri menetluskeskkond: vajadus tabelis/lingil eristada mida on külastatud mida mitte.
* Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis mingi konflikti kui headeris kõik väärtused sisselülitada, brand värvi peal pole searchi hinti näha
