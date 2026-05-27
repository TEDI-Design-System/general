# 2026-05-25 Biweekly meeting

## AI kokkuvõte (kohandatud)

### Peamised punktid
- **Custom muutujate haldus:** Uuendada muutujaid projektides et baasmuutujad kindlasti omaks prefixit/kausta 'TEDI' - vajalik custom üle kirjutatud muutujate jaoks. 
- **Filtri ja tabeli täiustused:** Lisati aktiivse valiku piirjoon ja disabled state; dark mode'is on primary ja secondary elemendid visuaalselt eristuvamad; tooltip sai sinise äärise võimaluse.
- **Checkboxi suurus:** Tabelis vähendati 24x24 → 18x18 pikslile, et ühtlustada mobiilse variandiga ja vastata WCAG nõuetele.
- **Arendusplaanid:** Date ja time picker, TimeField, Calendar, Input group, Slider, Header, Pagination, Empty state - Reactis tulemas;  Filter, Horizontal stepper - angularis tulemas. 
- **Figma integratsioon:** Juhendfailid plaanitakse lisada repositooriumisse, et toetada Figma Make ja Cloud Design tööriistu ning arendajate-disainerite koostööd.
- **TEDI kogukond:** Eesti App andis tagasisidet mobiilispetsiifiliste komponentide tarbeks; 

## Päevakord
- Figma custom muutujate ülekirjutuste halduse uuendus
- Filtri, tabeli ja tooltip komponentide täiustused
- Checkboxi suuruse muudatus ja WCAG nõuded
- Neljapäevase relese ülevaade
- Tabelite sorteerimise ja filtreerimise UX arutelu
- Button group visuaalne identiteet
- Eesti äpp ja mobiilikomponendid
- Figma Make ja juhendmaterjalide planeerimine

## Komponentide ja disainisüsteemi uuendused

- Filtri ja tabeli komponentidele lisati aktiivse valiku piirjoon ning disabled state, mis parandab kasutajaliidese selgust – muudatused tulid arendajate tagasisidest; dark mode'is kohandati primary ja secondary elementide visuaalset eristuvust
- Tooltip komponent sai sinise äärise võimaluse, mis on mõeldud eriti päise kasutusjuhtudeks
- Checkboxi suurus tabelis langetati 24×24 pikslilt 18×18 pikslile, et ühtlustada default variandiga

## Arendus- ja releseplaanid

Neljapäevase relese eel on mitmed uued komponendid valmis, kuid tabeli komponent vajab veel aega.
- Date ja time picker, TimeField, Calendar, Input group, Slider, Header, Pagination, Empty state - Reactis tulemas;  Filter, Horizontal stepper - angularis tulemas. 

## Kasutajaliidese ja UX teemad

- Sorteerimise klikitavad alad peaksid laienema kogu veerupäisele? Ehk variant on mitte piirduda vaid nupuga; 
- Vanemaealiste kasutajate testgrupp näitas, et mõiste "filter" ei ole alati selge, mis põhjustab valesid toiminguid; Angelica mainis et palus testil kasutajatel filtreerida ning nad hakkasid sorteerima - võimalus et nupud pole kasutajatele selged, kuid ka võimalus et mõiste pole kasutajale selge - mis on filtreerimise ja sorteerimise vahe, Kärolin vaatab üle testimise tulemused ja sihtgrupi. 
- Aktiivse tabelirea märgistamine tagasipöördumisel parandab kasutajakogemust – Kristel selgitas kliendisoovi aktiivsele reale visuaalse märgistuse säilitamiseks; lahendusena sobib stiiliklass, mis jätab rea siniseks (active olek).
- Button groupi arutelu näitas, et hetkel kasutatakse seda eelkõige vaatevahetuseks; Helis soovis säilitada praegune vorm, Kärolin kogub rohkem tagasisidet enne muudatuse otsustamist. Kristel soovis AKSis projektis samuti praegust visuaali et kasutaja ei ajaks tava-nunppudega segamini.
- Helis uuris kas selekteeritud rida peab olema sinine või võib ka vaid checkbox jääda valituks. Kärolin täpsustas et vaid checkbox saab ka jääda, arneduses sai samuti tehtud parandus.

## Figma ja disainitööriistade integratsioon

- TEDI repositooriumisse plaanitakse lisada juhendfailid (Guidelines.md), et toetada Figma Make ja Cloud Design tööriistu – Kärolin koordineerib vajalike failide loomist arendajatega lähinädalatel
- TEDI kogukonna faili lisame näidiseid mobiili jaoks kui Eesti äpilt luba saadakse, et tagada ühtne stiil ja korduvkasutus.

## Projektispetsiifilised teemad

- Eesti äpi meeskond kasutab TEDI muutujaid ja on loonud mobiilispetsiifilisi komponente (bottom nav, bottom sheetid), mis TED-is seni puudusid; plaan on need tulevikus TEDI süsteemi lisada
- 3D ja kaardirakenduste projektides kerkivad küsimused TEDI-ready komponentide puudulikkusest - hetkel on need communitys; Kärolin tõstab teema arendustiimi diskussiooni prioriteetide ja vajaduste selgitamiseks

## Otsused

### TEDI tiim
- Töötada välja juhendfailid AI tööriistade parema integratsiooni tarbeks
- Tõsta kaardikomponentide ja 3D-arenduse teema arendustiimi diskussiooni
- Uurida Eesti äpi protode jagamisõigust TEDI kogukonnaga

### Projektide disainerid
- Kasutada TEDI kogukonna diskussioonikanalit uute vajaduste ja probleemide jagamiseks

## Eelmistest koosolekutest veel üleval
- Figma Make ja TEDI koosluse testimine – juhendfailide loomine
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus
- Vertical stepperi alamsammude kuvamine mobiilis
- TTJA NBA, Rahvastikuregistri menetluskeskkond: vajadus tabelis/lingil eristada külastatud ja külastamata olekuid
- Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis konflikti kui headeris kõik väärtused sisse lülitada; brand värvi peal pole searchi hint näha
- Button group / patterngrupp: visuaalse identiteedi otsus edasi lükatud – Kärolin kogub rohkem tagasisidet
