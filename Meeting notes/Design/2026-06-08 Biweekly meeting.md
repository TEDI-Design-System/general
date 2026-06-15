# 2026-06-08 Biweekly meeting

## AI kokkuvõte (kohandatud)

## Komponentide ja Figma muudatused

- Kärolin selgitas, et footeri komponentidele lisati slotid, mis võimaldavad paindlikumat sisu lisamist ilma olemasolevaid footereid mõjutamata
- Slotid võimaldavad paigutada mis tahes sisu, näiteks logod või lingid
- Footeril säilitati eraldi propertid nagu "show logo right/left"
- Näidiste sisu muudeti eestikeelseks, kuigi komparandi nimed jäävad ingliskeelseks
- Footeris eemaldati mitmed keerukad variatsioonid ja akordionid asendati slotipõhise lahendusega, mis lihtsustab komponenti ja võimaldab kasutajal ise sobivaid elemente lisada
- Kärolin tutvustas ka transparent pagination komponenti, kus eraldi eraldati ja sisse-välja lülitatav separaator, mis mõjutab prototüüpe kuna vaikimisi on transparent paginationil separaator sisse lülitatud

## Figma komponentide struktuuri ümberkorraldus ja Tedi-readysse liikumine

- Kärolin teavitas, et mitmed kaardi komponendid liiguvad kaardi komponentide hulgast mingi hetk TEDI-readysse baaskomponentide hulka, näiteks karussell ja colorpicker, sest tegu ei ole kaardispetsiifiliste komponentidega. Komponentide ümberpaigutus ei riku prototüüpe, sest algfaili asukoha muutmine ei mõjuta visuaali
- TEDI Figma Kit sisaldab nüüd ka Figma Make jaoks mõeldud guideline'ide komplekti, mis kasutab TEDI-ready reacti komponente

## Otsinguväljale tulemusteta otsingu teadete kuvamine

- Piret küsis otsingu tulemuste puudumise teatamise viisi kohta, kas kuvada errorina või lihtsalt teadet
- Kärolini soovitus on mitte panna otsinguvälja error-staatusse, vaid kuvada tulemuste alal selge teadet, et "tulemusi ei leitud"
- Kui otsingutulemusi kuvatakse kogu lehel, siis võib kuvada vastava teadete ala, mis ei sega otsinguvälja kasutamist ega tekitaks vääritimõistmisi

## Tooltipide taustavärvi valikud ja disainiarutelu

- Sten tõi välja, et TEDI projektis on tooltipide taust värvitud tumedamaks halliks, kuid sooviks Tedis lisada ka heledat varianti
- Kärolin selgitas, et popover on abitekstina mõeldud heledas toonis, popoveri pind on suurem ja selle sisse on sobiv lisada ka muud sisu peale abiteksti. Samas kui tooltipid on lühemate tekstide jaoks loodud ning tumedad et eristuksid taustast.
- Tooltipi värvi on vajadusel võimalik disainis ja arenduses üle kirjutada.
- Luua selle kohta Discussionite alla postitus kui on soov et TEDIs sisalduks ka hele tooltip.

## Tegevusnuppude ja teksti paigutuse probleemid Timeline komponendis

- Helis tõi esile, et ühes projektis on muuda ja kustuta nupud paigutatud paremale ülesnurka, kuid pealkirja pole, ainult description-tekst ning description tekst pikkusest tulenevalt võivad nupud olla kas üleval või all kuna asuvad descriptioni järel.
- Kärolin soovitas, et Helis võiks teha Discussioni, lisades prototüübid ja ekraanipildid, et täpsemalt lahendusi leida ning vajadusel teha komponentidesse täiendusi
- Kiire lahendus on tegevusnupud desciptioni kõrvale jätta, vertikaalselt ülesjoondusega kuid pikemas perspektiivis võiks komponent toetada kõrvale paigutust

## Disaini muutuste ja kommunikatsiooni kokkulepped

- Kärolin pakkus, et komponentide ümber paigutusest lehtedel võib teavitada disaini kanalites, disainerid sel põhjust ei näinud ning leiavad, et otsing võimaldab komponente kiirelt üles leida, seega eraldi teavitusi pole vaja. 
- Kärolin rõhutas, et slotide lisamine olemasolevatesse komponentidesse võib mõjutada prototüüpe, mistõttu on oluline anda märku kui prototüüp saab mõjutatud ja aidata leida võimalikke anomaaliaid varakult.
- Prototüüpide katki minemise vältimiseks mõningate komponentide puhul kaalutakse komponentide täielikku asendamist uute versioonidega, et hoida prototüüpide stabiilsust.

## Otsused

### TEDI tiim
- Uurib TEDI Kiti Figma Make keskkonna uuendamise kohta, kas reacti komponendid uuenevad automaatselt või peab neid manuaalselt uuendma
- Claude design 

### Projektide disainerid
- Uus discussion luua: hele tooltip
- Uus discussion: timeline komponent pealkirjata, kuid nuppudega
 
### Eelmistest koosolekutest üleval
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus
- Vertical stepperi alamsammude kuvamine mobiilis
- TTJA NBA, Rahvastikuregistri menetluskeskkond: vajadus tabelis/lingil eristada külastatud ja külastamata olekuid
- Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis konflikti kui headeris kõik väärtused sisse lülitada;
- brand värvi peal pole searchi hint näha
