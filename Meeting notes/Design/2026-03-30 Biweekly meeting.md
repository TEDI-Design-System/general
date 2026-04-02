# 2026-03-30 Regulaarne disainikoosolek

## AI kokkuvõte

### Peamised punktid
- **Figma komponentide uuendused:** Lisatud spetsiifilised muutujad (sh horizontalnav tekstisuurus) ning visuaalne komponentide sisukord, mis lihtsustab leidmist ja uuendamist.
- **Slotsi funktsionaalsus:** Slotid lisati mitmetesse komponentidesse (header, modal, akordion jms Release notes'is väljatoodud), võimaldades vabas vormis sisu ilma komponenti lahti ühendamata.
- **Tabelikomponendid:** Lisati slotid ja mobiili variandid ootavad tagasisidet. 
- **Baaskomponentide prioriteedid:** Fookus Angular ja React baaskomponentidel; prioriteedid määratakse kasutajate hääletuse põhjal.
- **AI tööriistad Figmas:** Testitakse Claude'i AI tööriista prototüüpimiseks, mis kasutab TEDI komponente tõhusamalt kui Figma Make.
- **Teadmiste jagamine:** Loodi Figma-spetsiifiline tugikanal kiireteks küsimusteks ning koostati juhend muutujate ja teemingu kasutamiseks.

## Päevakord
- TEDI release uuenduste ülevaade
- Slotsi funktsionaalsuse demo ja arutelu
- Akordionikomponentide täiustused
- Tabelikomponentide mobiililahendused
- Baaskomponentide prioriteedid ja arendusplaan
- Figma AI tööriistade kasutamine prototüüpimisel
- Uue Figma tugi- ja teadmiste jagamise kanali tutvustus

## Komponentide ja Figma uuendused

TEDI projektis on tehtud mitu uuendust, et parandada töövoogu ja toetada eri projektide brändivajadusi.

- Mõned komponendid said eraldi muutujad – näiteks horizontalnav tekstisuurus – et projektid saaksid brändi spetsiifiliselt tekste kohandada ilma, et kõik small text väärtused üle kirjutataks
- Figma lehele on lisatud visuaalsete komponentide kataloog, mis lihtsustab komponentide leidmist ja uuendamist, eriti uutele kasutajatele
- Slotsi funktsionaalsus lisati mitmetesse komponentidesse (header, modal, akordion jne), võimaldades sinna vabas vormis sisu lisada
- Muutujate süsteemis tehtud muudatused võimaldavad alamprojektidel spetsiifilisi väärtusi üle kirjutada, mis aitab paremini hallata eri brändi nõudeid
- Kalender ja pickerid eraldati disainis ja arenduses, et paremini kajastada nende erinevaid funktsioone

## Akordionikomponentide vajadus:
- Einar Arro tõi välja vajaduse võimaldada kõigi sektsioonide samaaegne avamine, mitte ainult ühe aktiivse oleku hoidmine
- Kärolin kinnitas, et nii avatud kui ka suletud oleku vaikimisi seadistamine saab olema mõlema raamistikuga toetatud ja seda saab iga akordioni kohta eraldi määrata
- Helis Sepp arutas pealkirja ja ikooni vahelise suhtluse küsimusi – kasutajale peaks olema selge, kas pealkiri avab detailvaate või navigeerib eraldi lehele
- Arutleti, et kui pealkiri navigeerib teisele lehele, peaks selle kõrval olema eraldi link või nupp, et vältida kasutaja segadust

## Tabelikomponentide arendus ja mobiililahendused
- Tabelitele lisati slotid, mis võimaldavad lisada erinevaid elemente (vormid, pildid, ikoonid), suurendades paindlikkust
- Helis Sepp tõi välja alamridade toetuse ja checkboxide märkimise tähtsuse, mis vajab veel täiendavat lahendust mobiilis
- TEDI kogub ja ootab projektidelt mobiilivaajdusi

## Prioriteedid ja arendusplaanid baaskomponentidele

Sel aastal on fookus baaskomponentide arendamisel, et katta Angular ja React platvormide põhivajadused.

- Kasutajatel paluti jagada oma soovid diskussionikanalisse, et paremini hinnata oluliste baaskomponentide arendusprioriteetide järjestust
- Arendusprotsessi aluseks on hääletustulemuste järgi järjestatud prioriteedid – enim vajalikud komponendid saavad esmajärjekorras arenduse

## Figma prototüüpimise ja AI tööriistad

Figma AI-põhiste tööriistade kasutamine prototüüpimisel on olnud keerukas, mistõttu otsitakse alternatiivseid lahendusi.

- Kärolin testib Claude'i AI tööriista, mis loob reaalseid prototüüpe ja kasutab TEDI komponente paremini kui Figma Make
- Figma tokenid on kasutajapõhised ja kiiresti ammenduvad, mis piirab AI tööriistade kasutust prototüüpimisel
- Claude'i kontod ei kasuta Figma tokeneid, mis annab paindlikkuse, kuid nõuab asutuse otsust kasutuselevõtuks

## Kommunikatsioon ja teadmiste jagamine (figma-support kanal Slackis)

Loodi uus kanal ning koostati materjalid, et parandada projektide vahelist koostööd Figma teemal.

- Loodud Figma-spetsiifiline tugi- ja teadmiste jagamise kanal, et projektid saaksid üksteist aidata ja küsimusi kiiremini lahendada
- Kanal on mõeldud just Figma-spetsiifilistele küsimustele, vältides suuremate disainikanalite ülekoormust
- Kärolin koostas juhendi muutujate ja themingu kasutamiseks TEDI Figma projektides

## Otsused

### TEDI tiim
- Jätkata tabelikomponendi mobiiliversiooni disaini ja koguda projektide sisendeid mobiilsete tabelite vajaduste kohta
- Parandada pagination-i vaikimisi valikut (lisada vaikimisi esimene number, numbri bugi parandada)
- Jätkata AI-põhiste prototüüpimise katsetustega Claude'i kaudu ja jagada tagasisidet teistele
- Hallata Figma support kanalit
- Korraldada baaskomponentide prioriteetide arutelu ja koguda vajadusi diskussionikanalisse
- Koguda ja vormistada näidiste komplektid korduvate küsimuste ja disainilahenduste kohta

### Projektide disainerid
- Jagada tabeli ja muude komponentide spetsiifilisi lahendusi TEDI meeskonnaga
- Lisada komponentide arendussoovid diskussionikanalisse prioriteetide hääletamiseks
- Kasutada uut Figma tugikanalit Figma-spetsiifiliste küsimuste lahendamiseks

## Eelmistest koosolekutest veel üleval
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus
- Vertical stepperi alamsammude kuvamine mobiilis
- TTJA NBA, Rahvastikuregistri menetluskeskkond: vajadus tabelis/lingil eristada külastatud ja külastamata olekuid
- Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis konflikti kui headeris kõik väärtused sisse lülitada; brand värvi peal pole searchi hint näha
