# 2026-05-11 Regulaarne disainikoosolek

## AI kokkuvõte (kohandatud)

### Peamised punktid
- **Discussions: sweetAlert:** TEDI modaal katab vajaduse, upvotige kui on vajalik eraldi komponent.
- **Discussions: Command:** Praegust TEDI modaali saab selleks kohandada. Tagasiside: Mobiilis võiks dropdown lahendus olla mugavam ja lahendatud modaalina; Upvotige kui on vajalik eraldi komponent.
- **Discussions: Hierarhia komponendi vajalikkus:** Upvotige kui on vajalik eraldi komponent.
- **Claude Design ja Figma probleemid:** Ühtsusprobleemid tekivad, kuna protod ei kasuta alati TEDI komponente; vajalikud on selged reeglid.
- **Eesti App koostöö:** TEDIsse vajaduste ja näidete kogumine.
- **Mobiilitabeli arendus:** Mobiilitabeli arendus on taas käimas; 

## Päevakord
- Komponentide vajadused ja arendusprioriteedid (modaalid, autocomplete, hierarhia)
- Slotsi lahenduse laiendamine ja komponentide uuendused
- Prototüüpimise tööriistad: Claude Design ja Figma
- TEDI ja Eesti App koostöö
- Disainikanali haldus ja ligipääsuõigused
- Mobiilitabeli arendus ja kasutuselevõtt

## Komponentide vajadused ja arendusprioriteedid

Koosolekul keskenduti praegustele disaini- ja arendusvajadustele, eriti modaalide ja float-komponentide kasutusmugavusele ning prioriteetidele.

- Kärolin tõi välja uue modaalikomponendi discussionist, mille kasutusotstarve pole veel selge, kuid võib katta kinnituse ja teavituste vajadused
- Ta rõhutas, et TEDI olemasolev modaal võiks katta enamiku vajadustest, kui teha päise ja jaluse eraldus
- Paluti projektide tagasisidet, kas on vajadus eraldi modaalide või float-komponentide järele
- Einar selgitas, et mobiilis oleks dropdowni asemel modaal visuaalselt parem ja kasutajasõbralikum
- Kärolin märkis, et praegu saab TEDI modaaliga selliseid lahendusi juba teha, kui mobiilis võiks dropdown ümber lülituda modaaliks siis projektidel on võimalus seda teha 

## Hierarhilise info kuvamine ja tree-element

- Kärolin tõi välja, et Figma-s on olemas tree-element, kuid arenduses on see ainult sisemine alamkomponent ja seda ei saa eraldi kasutada
- Ta märkis, et võiks luua eraldi laialt kasutatava hierarhia komponendi, mis toetaks erinevaid projekte
- Einar pakkus, et parem ja olemasolev disain oleks kasulik, mida jagada teistele

## Slotsi lahenduse laiendamine ja komponentide uuendused

- Kärolin mainis, et Figma slotsid lisati alertidesse ning lisatakse peagi ka tooltipi ja dropdown itemitesse
- Reacti poolel valmisid toggle ja tabide komponendid, Angularis lisandus select ja radio 

## Prototüüpimise tööriistad: Claude Design ja Figma

Arutati Figma ja Claude Design tööriistade kasutamist prototüüpimisel ning probleemidest, mis on seotud komponentide ja stiilide ühtsusega.

- Claude Designi protod ei kasuta alati TEDI komponente - milles asi?
- Sten kirjeldas, et Claude Design kordab nullist elemente ja ei suuda alati korrektselt võtta disainisüsteemi elemente, mis raskendab ühtsuse hoidmist
- Kärolin selgitas, et mõned tööriistad loovad nullist elemente, mitte ei kasuta TEDI komponente, mis tekitab disainipraktikate ebaühtlust
- Ta rõhutas vajadust rangete piiride kehtestamiseks, et vältida isetehtud komponentide segamist disainisüsteemiga
- Sten tõi välja, et Claude ei saanud kätte õigeid nuppe ja värve kui ette anti githubi repo kuid peale mõningaid kaevtöid leidis Claude siiski üles stiilid
- Piret tõi välja probleemi et Figma make tahtis mingit ligipääsu git'i mida ei saanud/osanud anda - pöördus TEDI tiimi poole.

## TEDI ja Eesti App koostöö ning kohandamise strateegia

- Kärolin selgitas, et Eesti äpp on teinud stiililisi muutusi, näiteks suuremate nurkadega kaardid ja erinev padding, mis on mobiilis olulisemad
- Plaanitakse koostööd Eesti äpp meeskonnaga, et tuua head näited TEDI-sse tagasi ja vastupidi
- Rõhutati, et projekti enda otsustada, kui palju TEDI komponente kohandada, kuid riikliku rahastuse puhul eelistatakse algupärast kasutust
- Värvikohandused tuleb testida vastavuses WCAG keelega
- Suuremad kohandused võivad keerulisemaks muuta tugi- ja ühtsuse hoidmist, mistõttu on soovitav kasutada TEDI komponente enam-vähem originaalis
- Veera failid on kolitud dedikeeritud kausta, mis muudab ligipääsu ja säilitamise ühtsemaks; 

## Disainikanali haldus ja ligipääsuõigused

- Kärolin tõi välja, et palju on Gmail-kontode taotlusi, mille kaudu pole võimalik aru saada kasutajate organisatsioonist
- Kasutada töömeili kontosid, et vähendada segadust ja tagada parem jälgitavus
- Kärolin kontrollis, et uus koosolekusari on kõigil kalendrisse lisatud, ja rõhutas kommunikatsiooni Disainikanali kaudu

## Mobiilitabeli arendus ja kasutuselevõtt

- Kärolin märkis, et mobiilitabeli arendus oli seisnud kuna projektide poolt puudus huvi, kuid nüüd saab lõpuni tehtud

## Üldine disainisuhtlus ja kogemuste jagamine

- Kärolin kutsus meeskonda jagama kogemusi ja abi küsima disainikanalis
- Ta rõhutas, et koostöö aitab paremini mõista komponentide kasutust ja parandada disainilahendusi
- Samuti julgustati jagama Figma Make'i ja Claude Designi katsetusi, et ühiselt lahendusi leida
- Kärolin plaanib teha uusi näidiseid ja vaateid TEDI raames, et toetada projektide ühtset kasutust

## Otsused

### TEDI tiim
- Uurida ja selgitada GitHub'i repo ja Figma Make vahelist koostoimet - mis probleem esines?
- Jälgida ja vajadusel täiendada TEDI komponente ühenduses Claude Designi ja Claude'iga, parandades kasutuspiiranguid ja juhendmaterjale
- Luua mobiili versioon
- Saata Einarile Figma Community link hierarhiliste elementide jagamiseks

### Projektide disainerid
- Jagada tagasisidet, kas on vajadus eraldi modaalide või float-komponentide järele (vt discussions)
- Jagada infot TEDI ja AI koostöö kohta

## Eelmistest koosolekutest veel üleval
- Figma Make ja TEDI kooslus vajab veel testimist – testitud varasemas etapis, võimalik et Make on arenenud
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus
- Vertical stepperi alamsammude kuvamine mobiilis
- TTJA NBA, Rahvastikuregistri menetluskeskkond: vajadus tabelis/lingil eristada külastatud ja külastamata olekuid
- Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis konflikti kui headeris kõik väärtused sisse lülitada; brand värvi peal pole searchi hint näha
