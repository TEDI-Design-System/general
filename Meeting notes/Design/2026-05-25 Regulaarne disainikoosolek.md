# 2026-05-25 Regulaarne disainikoosolek

## AI kokkuvõte (kohandatud)

### Peamised punktid
- **Custom muutujate haldus:** Uus lahendus TEDI projektides võimaldab hallata muutujate ülekirjutusi Figma plugina kaudu, kõrvaldades varasemad kuvamisprobleemid ColorSpace kollektsioonis.
- **Filtri ja tabeli täiustused:** Lisati aktiivse valiku piirjoon ja disabled state; dark mode'is on primary ja secondary elemendid visuaalselt eristuvamad; tooltip sai sinise äärise võimaluse.
- **Checkboxi suurus:** Tabelis vähendati 24x24 → 18x18 pikslile, et ühtlustada mobiilse variandiga ja vastata WCAG nõuetele.
- **Arendusplaanid:** Date picker, TimeField, EmptyState ja Pagination on releseks valmis; tabeli komponent ei jõua neljapäevasele relesele; filter ja pagination tulevad Angulari ja Reacti harudesse.
- **Figma integratsioon:** Juhendfailid plaanitakse lisada repositooriumisse, et toetada Figma Make ja Cloud Design tööriistu ning arendajate-disainerite koostööd.
- **TEDI kogukond:** Eesti App teeb koostööd mobiilispetsiifiliste komponentide arendamiseks; diskussioonikanal on peamine infoallikas uute vajaduste tuvastamiseks.

## Päevakord
- Figma custom muutujate ülekirjutuste halduse uuendus
- Filtri, tabeli ja tooltip komponentide täiustused
- Checkboxi suuruse muudatus ja WCAG nõuded
- Neljapäevase relese ülevaade: date picker, filter, pagination, header
- Tabelite sorteerimise ja filtreerimise UX arutelu
- Button group / patterngrupi visuaalne identiteet
- Eesti App koostöö ja mobiilikomponendid
- Figma Make ja juhendmaterjalide planeerimine

## Komponentide ja disainisüsteemi uuendused

Peamised muudatused puudutavad komponentide funktsionaalsuse täiendamist ja Figma integreerimist, et parandada arendajate töövoogu.

- Custom muutujate ülekirjutamise lahendus TEDI projektides võimaldab nüüd luua uusi kollektsioone, kuhu saab teha ülekirjutusi – see lahendab varasema vea, kus TEDI kaust ei kuvanud extended kollektsioonis õigesti; parandus tehti Figma plugina kaudu
- Filtri ja tabeli komponentidele lisati aktiivse valiku piirjoon ning disabled state, mis parandab kasutajaliidese selgust – muudatused tulid arendajate tagasisidest; dark mode'is kohandati primary ja secondary elementide visuaalset eristuvust
- Tooltip komponent sai sinise äärise võimaluse, mis on mõeldud eriti päise kasutusjuhtudeks
- Checkboxi suurus tabelis langetati 24×24 pikslilt 18×18 pikslile, et ühtlustada mobiilse variandiga ja vastata WCAG nõuetele – muudatus käsitleb olukorda, kus klikitav label puudub

## Arendus- ja releseplaanid

Neljapäevase relese eel on mitmed uued komponendid valmis, kuid tabeli komponent vajab veel aega.

- Tabeli komponent on peaaegu valmis, kuid ei jõua neljapäevasele relesele; pagination ja filter jõuavad Angulari ja Reacti harudesse ning pagination saab ka mobiilse variandi
- Date picker ja seotud kuupäeva- ning kellaajaväljade komponendid on releseks valmis: DateField toetab kuupäevade ja vahemike valikut, TimeFieldil on kolm varianti (keritav, valikuga, dropdown)
- EmptyState ja Pagination komponendid on lisatud tabeli vajadustest lähtuvalt; EmptyState on lihtne ja kasutusvalmis, Pagination integreeritakse vastavalt vajadusele
- Header komponent tuleb Reacti harusse, Angulari poolele on täiendused plaanis

## Kasutajaliidese ja UX teemad

Tabelite sorteerimise ja filtreerimise funktsionaalsuse arutelu tõi välja kasutajate segaduse ning vajaduse parema lahenduse järele.

- Sorteerimise ja filtreerimise klikitavad alad peaksid laienema kogu veerupäisele, mitte piirduma väikese nupuga; Kärolin plaanib väikese kasutajauuringu, et valideerida laiendatud klikiala
- Vanemaealiste kasutajate testgrupp näitas, et mõiste "filter" ei ole alati selge, mis põhjustab valesid toiminguid; Helis ja Kristel rõhutasid, et filtreerimise ja sorteerimise segiaamine on levinud probleem
- Aktiivse tabelirea märgistamine tagasipöördumisel parandab kasutajakogemust – Kristel selgitas kliendisoovi aktiivsele reale visuaalse märgistuse säilitamiseks; lahendusena sobib stiiliklass, mis jätab rea siniseks
- Button group / patterngrupi arutelu näitas, et hetkel kasutatakse seda eelkõige vaatevahetuseks; Helis soovitas säilitada praegune vorm, Kärolin kogub rohkem tagasisidet enne muudatuse otsustamist

## Figma ja disainitööriistade integratsioon

Figma komponentide haldus ja koostöö arendajatega on arendamisel, et lihtsustada disainerite ja arendajate tööprotsessi.

- Figma plugina kaudu saab nüüd paremini hallata custom muutujate ülekirjutusi ja extended kollektsioone; tühja kausta funktsioon lahendab kuvamisprobleemid
- Dedicode repositooriumisse plaanitakse lisada juhendfailid (Guidelines.md), et toetada Figma Make ja Cloud Design tööriistu – Kärolin koordineerib vajalike failide loomist arendajatega lähinädalatel
- TEDI kogukonna fail jagab mobiili- ja veebirakenduste disainikomponentide arendust, et tagada ühtne stiil ja korduvkasutus

## Projektispetsiifilised integratsioonid ja koostöö

TEDI komponentide kasutuselevõtt laieneb ning tekib vajadus parema halduse järele suurte projektide jaoks.

- Eesti Appi meeskond kasutab TEDI muutujaid ja arendab mobiilispetsiifilisi komponente (alumised navigatsioonid, bottom sheetid), mis TED-is seni puudusid; plaan on need tulevikus TEDI süsteemi lisada
- 3D ja kaardirakenduste projektides kerkivad küsimused TEDI komponentide sobivusest; Kärolin tõstab teema arendustiimi diskussiooni prioriteetide ja vajaduste selgitamiseks
- TEDI kogukonna diskussioonikanal on peamine infoallikas uute vajaduste ja vigade tuvastamiseks; suurem arendustiim võimaldab kiiremat reageerimist

## Otsused

### TEDI tiim
- Uuendada TEDI muutujate ja ülekirjutuste haldust vastavalt arendajate tagasisidele
- Jätkata filtri, tabeli ja tooltip komponentide täiendamist ning valmistada ette neljapäevane reles
- Viia läbi väike kasutajauuring sorteerimisfunktsiooni laiendamiseks kogu veerupäisele
- Töötada välja juhendfailid (Guidelines.md) Figma tööriistade parema integratsiooni tarbeks repositooriumis
- Tõsta kaardikomponentide ja 3D-arenduse teema arendustiimi diskussiooni
- Jälgida Eesti Appiga koostöökomponente ja nende integreerimist TEDI süsteemi

### Projektide disainerid
- Jagada tagasisidet tabelite radio-buttonite, aktiivsete ridade ja patengruppide kasutuse kohta
- Kasutada TEDI kogukonna diskussioonikanalit uute vajaduste ja probleemide jagamiseks
- Saata näiteid tabeli aktiivsete ridade projektispetsiifiliste vajaduste kohta

## Eelmistest koosolekutest veel üleval
- Figma Make ja TEDI koosluse testimine – juhendfailide loomine on töös
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus
- Vertical stepperi alamsammude kuvamine mobiilis
- TTJA NBA, Rahvastikuregistri menetluskeskkond: vajadus tabelis/lingil eristada külastatud ja külastamata olekuid
- Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis konflikti kui headeris kõik väärtused sisse lülitada; brand värvi peal pole searchi hint näha
- Button group / patterngrupp: visuaalse identiteedi otsus edasi lükatud – Kärolin kogub rohkem tagasisidet
