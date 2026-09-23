# 2026-08-03 Regulaarne disainikoosolek

## AI kokkuvõte (kohandatud)

### Peamised punktid
- **Komponentide nimed:** Hidden field võiks ümber nimetada hover input, editable input, hover edit, on-hover edit, read-edit - sest komponent on nähtav ja interaktiivne, mitte päris peidetud väli.
- **Table card:** "Mobile" nimetus eemaldada, sest komponent visualiseerib ühe tabelirea kaardina ja võib olla kasutusel mitmel platvormil.
- **Tekstieditor:** TEDI pakub lihtsaid stiilijuhiseid; tekstieditori peaks iga projekt välisest libraryst ise võtma.
- **Clear button inputväljal:** kas X-nupp peaks olema vaikimisi nähtav tekstiväljal kus tekst on lisatud?
- **Värvide ja tagide probleemid:** Kliendil on 8 staatusevärvi, TEDI värvid ei kata vajadust.

## Komponentide nimetamine ja kasutus

Nimetamisküsimused ja selgitused komponentide funktsionaalsuse osas on vajalikud, et vältida segadust arenduses ja disainis.

- Hidden field on visuaalselt nähtav, kuid käitub nagu read-only tekst, millel on hover-efekt ja klikitavus; "hidden field" nimetuse all oodatakse arenduses midagi peidetut, kuigi tegu on interaktiivse väljaga
- Arutati nime "Hover edit" või "on hover edit", mis kirjeldaks komponendi käitumist paremini; komponent on mõeldud stiili rakendamiseks erinevatele sisenditele (tekst, valik jne), mitte ainult tekstiväljale
- Table mobile puhul soovitakse eemaldada "mobile" nimetus, sest komponent võib olla kasutusel ka kitsamates tingimustes, mitte ainult mobiilis; pakuti nime "table card", "table row card", "table compact", "data row card", kuna komponent visualiseerib ühe tabelirea kaardina, mitte kogu tabelit
- Tekstieditor: TEDI ei plaani arendada keerukat tekstieditorit, vaid pakub stiilijuhiseid lihtsatele vormingutele (nt bold, italic, listid); projektid saavad valida enda vajadustele vastava teegi ja stiilida selle TEDi reeglite järgi
  - Lauri ja Helis rõhutasid, et lihtsam tekstieditor võiks TEDi paketti siiski kuuluda baastaseme funktsionaalsuse tagamiseks; Kärolin lubas info arendajatele edasi anda ja vajadusel teema uuesti avada
- File previewer ei tule TEDi arendatud komponendina, vaid stiilijuhisena; iga projekt valib ise, millist teeki failide vaatamiseks kasutab. Vastuargumente ei esitatud

## Arenduspraktikad ja UX detailid

Selgitati arenduse ja kasutajakogemuse ühtlustamise vajadusi, et tagada mugav ja ühtlane kasutus üle projektide.

- Clear button (x): praegu on Angularis ja Reactis erinev praktika, kas nupp on vaikimisi nähtav või vajab arendaja lisalülitust; disainerid pooldasid, et x oleks automaatselt nähtav, kui väli sisaldab teksti
- TEDI poolt on pakutud veel variant et clear button ilmub nähtavale siis kui väli on täidetud ja kasutaja hoverdab - see hoiab ära liigse müra vaatest kus on palju väljasid.
  - Telefonis hover puudub, seega peaks x alati nähtav olema või ilmuma klikil; projekti tasandil võiks see olla propertina seadistatav, kuid üldine vaikimisi peaks olema x olemasolu
- Figma bugi kuvab muutujate osas valesti muutusi ja takistab komponentide avaldamist; Kärolin jälgib ja suhtleb Figmaga vea lahendamiseks, seni pole see bugi projektidesse jõudnud sest Figmat ei ole peale seda avaldatud.
- Arutati, kas TEDI võiks projekti alguses välja tuua läbimõeldavad disainipõhimõtted (nt modaalide asukoht ja kasutus), määramata täpset paigutust; osalejad ei näinud hetkel suurt vajadust, pigem kaalutakse vastavalt projektile

## Värvid ja staatus-tagid

- Ühes projektis tuli kasutada 8 erinevat staatusevärvi, mis ei tohi kattuda standardvärvidega (error, success, warning); värvivalikul kasutati open color paletti ja kontrastitestimist, kuid klient ütles et tagide tekst on liiga väike, värvid ka ei sobi. Vaja on TED tiimi kinnitust, kas teha uus label-komponent või jätta vana;
  - Projekt teeb ise vastavalt vajalikud kohandused ja jagab seda TEDI meeskonnaga.
 
## TEDi kasutus ja projektide integratsioon

TEDI disainisüsteem on paindlik, kuid vajab projektide vahel head koordineerimist ja muutujate haldust.

- Mõned projektid kopeerivad TEDI komponendid oma Figma failidesse, mitte ei kasuta master-faili otse;
- TEDI võimaldab muuta kõrgema taseme muutujad projektispetsiifiliseks, nii et näiteks RMK projekt saab oma värviskeemi lisada
- Arendus toetab muutujate muutmist, mis lubab projektidel säilitada oma stiili, kuid hoida ühtset komponenti; Kärolin julgustas kliente andma tagasisidet puuduolevate semantiliste muutujate kohta;
- Ligipääsetavuse link: kliendid soovisid tõsta ligipääsetavuse lingi menüüst jalusesse; TEDi arendus lubas seda vabalt teha, kuna TEDI ei sea lingi sisule ega paigutusele piiranguid. 

## Otsused

### TEDI tiim (Kärolin)
- Jätkata Figma vea uurimist, mis takistab uute komponentide publitseerimist, ning valmistada ette komponentide uus avaldamine
- Otsustada tekstiredaktori komponendi minimaalsete funktsioonide osas (nt paks, kaldkiri, loendid) ja edastada otsus arendajatele
- Koondada disaini ja arenduse tagasiside "hidden field" komponendi ümbernimetamiseks ning koguda ideid sobiva nime leidmiseks
- Lisada TEDi stiilijuhiste alla file previeweri juhised koos soovitustega sobivate teekide kohta, jättes valiku projektidele
- Edastada arendajatele otsus "clear button" (x) kuvamise ja selle property-te juhtimise kohta projektides

### Projektide disainerid
- Saata Kärolinile TEDi komponente kasutavate projektide lingid, et koguda reaalseid kasutusnäiteid ja mõista paremini kasutusolukordi
- Suunata kõik disainiga seotud küsimused TEDi ühisesse disainikanalisse, et tagada parem infovahetus ja koordineeritus

## Eelmistest koosolekutest veel üleval
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus
- Vertical stepperi alamsammude kuvamine mobiilis
- TTJA NBA, Rahvastikuregistri menetluskeskkond: vajadus tabelis/lingil eristada külastatud ja külastamata olekuid
- Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis konflikti kui headeris kõik väärtused sisse lülitada; brand värvi peal pole searchi hint näha
