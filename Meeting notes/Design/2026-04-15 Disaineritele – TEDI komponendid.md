# 2026-04-15 Disaineritele – TEDI komponendid

## AI kokkuvõte (kohandatud)

### Peamised punktid
- **Komponentide uuendused:** Tekstiredaktor toetab nüüd kolmandate osapoolte lahendusi TEDI stiilis; alertidele lisati slotid tegevusnuppude ja linkide jaoks; AutoGrow tekstiväljadele parandab kasutajamugavust.
- **Pagination parandus:** Vaikimisi aktiivne number on nüüd 1 (mitte 2), mis vähendab käsitsi kohandamise vajadust projektides.
- **AI integratsioon Figmas:** Kärolin tutvustas Figma Make ja Claude'i integratsiooni – AI suudab genereerida TEDI komponente, kuid vajab täpsemaid stiili- ja värvijuhiseid ning on tokenipiirangu tõttu aeglane.
- **Dropdownide dokumenteerimine:** Mitmikvaliku ja üksikvaliku visuaalset erinevust hetkel ikooniga ei eristata – vajab paremat dokumenteerimist või visuaalset lahendust.
- **EU rahastuslogode kuvamine:** Puudub ühtne standard logode paigutamiseks – teema läheb diskussiooni ja näidislahenduste kogumisele.
- **Protsessid ja kanalid:** Iganädalane prioriteetide ülevaatus, Figma support kanal ja Wishlist kanal parandavad disaini-arenduse koostööd.

## Päevakord
- Komponentide uuendused: tekstiredaktor, AutoGrow, alertide slotid, pagination
- AI prototüüpimine Figma Make ja Claude'iga
- Dropdownide ikonograafia ja valikurežiimide dokumenteerimine
- Filterkomponendi arendusjärjekord
- EU rahastuslogode kuvamine rakendustes
- Kaardikomponentide tagasiside
- Kanalid ja koostöövood

## Komponentide uuendused

Mitmed komponendid said funktsionaalseid ja visuaalseid täiendusi, mis parandavad nii kasutajamugavust kui ka arendajate paindlikkust.

- Tekstiredaktori arendust laiendatakse nii, et kolmandate osapoolte lahendusi on võimalik visuaalselt kohandada TEDI disainistiiliga – arendajatele edastatakse vastavad juhised
- AutoGrow funktsionaalsus lisati tekstiväljadele, võimaldades sisestamisel automaatset kõrguse muutmist; Figmas vähendati minimaalkõrgust 40 pikslile, mis vastab tavapärasele sisendvälja kõrgusele
- Alertide komponentidele lisati uued slotid tegevusnuppude ja linkide toetamiseks, mis võimaldab keerukamat kasutajaliidest (nt kinnituse ja tühistamise toimingud); joondus ja paigutus on arenduses täpsustamisel
- Pagination sai paranduse: vaikimisi aktiivseks numbriks on seatud 1, mitte 2, mis vähendab vajadust projektides käsitsi kohandada

## AI prototüüpimine ja Figma integratsioon

Kärolin tutvustas Figma Make integratsiooni Claude'i ja TEDI disainikirjastusega, mis automatiseerib disainielementide loomist.

- AI suudab genereerida komponente kompleksselt, kuid vajab täpsemaid stiili- ja värvijuhiseid ning on praegu tokenipiirangu tõttu aeglane
- Sten Rõngelep tõi välja vajaduse parema dokumenteerimise järele, et AI suudaks automaatselt valida õiged värvid ja fondid; TEDI veebilehel on muutujad olemas, kuid AI vajab täpsemat juhendamist
- Kärolin plaanib testida branchimist Figmas – muudatused tehakse harudena, vaadatakse üle ja integreeritakse, mis parandab ülevaatlikkust ja koostööd
- Arutati tulevikuvisiooni, kus AI abil saab üks inimene juhtida analüüsi, disaini ja arendust tervikuna – see võib muuta meeskondade struktuuri ja tööjaotust
- AI ei asenda disainereid täielikult: visuaalne tunnetus ja täpne detailide kontroll vajavad inimest, kuid prototüüpimise kiirus ja maht kasvab märkimisväärselt

## Kasutajaliidese komponendid ja UX küsimused

Arutati mitmeid spetsiifilisi komponentide funktsionaalseid detaile, keskendudes kasutajamugavusele ja visuaalsele selgusele.

- Dropdownide puhul ei eristata mitmikvalikut ja üksikvalikut ikooniga – kasutajale selgub valikutüüp alles menüü avanemisel, mis on tavapärane lahendus, kuid vajab paremat dokumenteerimist või kaalumist visuaalselt paremaks lahendamiseks
- Filterkomponent on Angularis arenduses, kuid Reacti versiooni prioriteet on lahtine – Piret rõhutas vajadust hääletada komponentide järjekorra üle vastavalt projektide ootustele
- Kaardirakenduste komponendid on Maa-ameti tellituna valdavalt kasutusel, kuid on vajadus väiksemate ja kasutajasõbralikumate elementide järele; projektide tagasiside aitab arendust suunata

## EU rahastuslogode kuvamine

Rahastusnõuete täitmine logode nähtavuse osas on keeruline teema, kuna puudub ühtne standard ja erinevad rakendused on leidnud erinevad lahendused.

- Paljud rakendused on sisemised ja neil puudub tavapärane footer, mistõttu logosid kuvatakse külgmenüüs, fade-komponentides või eraldi aladel
- Einar Arro tõi välja, et külgmenüü on sageli avatud ja sobib logode kuvamiseks, kuid taustavärvide ja läbipaistvuse tõttu tekib kontrasti probleem – sinise taustaga rakendustes kasutatakse sageli valget tausta logode taga
- Juhendites puuduvad selged reeglid sinise tausta kohta, mis tekitab segadust ja tõlgendamisruumi; mõned projektid on valinud konservatiivse lähenemise valge taustaga
- Mobiilivaated esitavad täiendavaid väljakutseid, kus ruum on piiratud ja menüüd sageli kokku pandud, mistõttu logode nähtavus võib varieeruda
- Kärolin võtab teema diskussiooni alla ja kogub näidislahendusi, et luua selgem ülevaade parimatest praktikatest

## Protsessid ja kanalid

Meeskond on täiustanud töövooge, et parandada informatsiooni jagamist ja disaini-arenduse koostööd.

- Iga nädala alguses toimub prioriteetide ülevaatus, kus kasutajate häälestus ja projekti vajadused määravad arendusse tulevate ülesannete järjekorra
- Figma support kanal on loodud Figma-spetsiifilisteks küsimusteks ja teadmiste jagamiseks, vähendades info killustumist
- Wishlist kanal toob automaatselt teavitusi uutest arendusvajadusest, hoides kõiki kursis ja koordineerides vajadusi
- Kärolin rõhutas, et disaini ja arenduse vahelise koostöö sujuvuse parandamine on jätkuv eesmärk, eriti AI ja prototüüpimise tööriistade kasutamisel

## Otsused

### TEDI tiim
- Edastada arendajatele info tekstiredaktori visuaalse kohandamise juhise vajaduse kohta
- Täiendada alertide slottide joondust ja paigutust arenduses
- Jätkata Figma Make ja Claude'i integratsiooni testimist ning jagada kogemusi meeskonnaga
- Koguda diskussiooni alla EU rahastuslogode paigutamise näidislahendused ja kujundada ühised praktikad
- Administreerida Wishlist kanalit ja tagada, et projektide vajadused saavad hääletatud ning prioriseeritud
- Testida Figma branchimist ja arendada AI võimekust disainijuhiste järgimiseks

### Projektide disainerid
- Hääletada filterkomponendi ja teiste vajalike komponentide arenduse prioriteedi üle Figma diskussioonides
- Saata tagasisidet kaardi- ja tekstipõhiste komponentide kasutamise kohta
- Kasutada Figma support kanalit Figma-spetsiifiliste küsimuste lahendamiseks
- Jagada lahendusi ja kogemusi dropdown valikute eristamise ning rahastuslogode kuvamise kohta

## Eelmistest koosolekutest veel üleval
- Figma Make ja TEDI koosluse testimine – praegu pooleli, Claude'i integratsioon testfaasis
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus
- Vertical stepperi alamsammude kuvamine mobiilis
- TTJA NBA, Rahvastikuregistri menetluskeskkond: vajadus tabelis/lingil eristada külastatud ja külastamata olekuid
- Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis konflikti kui headeris kõik väärtused sisse lülitada; brand värvi peal pole searchi hint näha
