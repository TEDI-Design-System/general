# 2026-03-16 Regulaarne disainikoosolek


    


_AI kokkuvõte (kohandatud)_
## Peamised punktid
**Figma muutujate lihtsustamine:** Projekti-põhised muutujad eemaldati, et vähendada segadust ja ühtlustada nimekasutust.
**Kollektsioonide laiendamine**: “Extend Collection” võimaldab projektidel luua oma muutujate kihte ilma disainisüsteemi lahti murdmata.
**Slots funktsionaalsu**s: Figma uus slotide võimalus lubab komponentides sisu muuta ilma neid detatchimata.
**Komponentide prioriseerimine**: TEDI arendus prioriseeritakse projektide hääletuse ja vajaduste põhjal.
**Tabi ja tekstiväljade arendus:** Tabi komponent saab horisontaalse mobiilse kerimise toe ning tekstiväljade paindlikkust uuritakse (laiendatavus vastavalt kirjutamisele).


## Päevakord
* TEDI vabanes projektipõhistest muutujatest (RIT, MUIS)
* Uute discussionite ülevaade
* Demo: Figma slots
* Tagasiside kogumine

## Figma muutujate ja kollektsioonide uuendused
* Figma disainisüsteemi muutujate haldus tehti lihtsamaks, eemaldades projektispetsiifilised muutujad.
* Projekti-põhised muutujad nagu TEDI Light ja TEDI Dark eemaldati.
* Kasutusele jäävad üldised Light ja Dark variatsioonid.
* Spetsiifilised muutujad (nt Rit ja Muis) eemaldati, et vältida nende juhuslikku kasutamist teistes projektides.
* Värvi- ja raadiuse, suuruse muutujad saab nüüd üle kirjutada Figma kollektsioonide kaudu.
* Arenduses tuleb kontrollida värvikontrasti ja accessibility testide vastavust.

## Extend Collection funktsionaalsus
* Figma uus Extend Collection võimaldab projektidel luua põhikollektsioonist oma laienduse.
* Tekib lapskollektsioon, mis pärib väärtused kõrgemast disainisüsteemist ja laseb üle kirjutada.
* Projektid saavad muuta ainult vajalikke muutujaid.
* See lahendus aitab säilitada ühenduse disainisüsteemiga.

## Slots funktsionaalsus komponentides
* Figma uus slotide funktsioon võimaldab komponentides sisu paindlikumalt muuta.
* Näiteks modalite ja alertide sisu saab lisada ilma komponenti lahti ühendamata.
* Kärolin alustas slots rakendamist TEDI komponentides.
* See vähendab komponentide detatchimise vajadust.
* Parandab komponentide uuendatavust ja korduvkasutatavust.

## Komponentide prioriteedid ja arendusplaan
* TEDI komponentide arendus prioriseeritakse projektide vajaduste järgi.
* Prioriteedid määratakse projekti hääletuse ja tagasiside põhjal.
* Arenduses on Time Picker, Date Picker, Tab ja Header komponendid.
* Table komponent on analüüsis – otsustatakse, kas kasutada kolmanda osapoole lahendust või TEDI oma.
* Homme selgub täpsem plaan kuid eesmärk on katta aasta jooksul puuduolevad baaskomponendid.

## Community komponentide eemaldamine
* Community komponendid plaanitakse järk-järgult asendada TEDI komponentidega.
* Näiteks spinner, modal ja stepper, pagination, footer on järgmised mis Community Figmast lähevad kustutamisele TEDI versiooni.
* Community komponendid eemaldatakse, kui vastavad TEDI komponendid on olemas.

## Komponentide detatchimise probleem
* Detatchimine on märk sellest, et komponent ei kata kasutusvajadust.
* Sageli detatchitakse tabeleid, dropdown-iteme, status badge ja checkboxe.
* Kärolin kogub infot detatchimise põhjuste kohta.
* Slots funktsioon peaks aitama seda probleemi vähendada.
* Kasutajatel palutakse jagada reaalseid näiteid detatchimisest.

## Komponentide leitavuse parandamine
* Figma komponentide struktuuri plaanitakse parandada.
* Suured kategooriad (nt form komponendid) võivad saada eraldi lehed. - kui vaja ja see aitab, disainerid ei näinud sellel vajadust kuna kergem on ühel lehel komponente otsida, aga hetkel osad komponendid on küll keerulisemalt leitavad kui asuvad nt Content või Layout lehel
* See vähendab ühe lehe koormust ja parandab navigeerimist.
* Plaanis on lisada visuaalne sisukord Figmasse. - Disaineritele see mõte meeldis

## Tabi komponendi uuendus
* React implementatsioon on töös.
* Mobiilis kaalutakse horisontaalset kerimist.
* Tabide sees dropdowni tuge hetkel peeti vajalikuks ainnult siis kui tabe on väga palju reas ja komponent ei mahuta - ehk responsive disaini osana.

## Tekstiväljade paindlikkuse parandus
* Vajadus kitsamate ja ühe rea tekstiväljade järele mis laieneb vastavalt tekstile.
* Kärolin uurib kas praegune komponent arenduses on expandable vastavalt teksti kõrgusele.

----

## Tagasiside kogumine
* Figma slots - mis komponente olete detachinud põhjusel et sinna sisse ei saa lisada sisu ise?
* Kas ja kus olete kasutanud veel kompaktsemaid tabeleid kui hetkel TEDI valikus on?
* Mis näite-vaateid projektides vajaksite TEDI poolt?
* Homme on TEDI tiimil aastaplaani koostamine - ootan tagasisidet mida TEDI'lt käesoleval aastal disainis poolelt ootate?
----

## Otsused
* Jätkata slots funktsionaalsuse rakendamist TEDI komponentides.
* Koondada projektide tabelinäited ja kitsad tabelimustrid Community Figmasse.
* Parandada komponentide leitavust Figma süsteemis. - visuaalne sisukord esimeseks sammuks lisada
* Uurida tekstivälja expandable funktsionaalsuse arendusvõimalust.
* Koguda infot komponentide detatchimise põhjuste kohta.

### Projektide disainerid ja arendajad
* Jagada näiteid kitsastest tabelitest ja muudest projektispetsiifilistest lahendustest.
* Osaleda TEDI tagasiside küsitluses.
* Jagada infot komponentide detatchimise põhjuste kohta.
* Anda tagasisidet komponentide leidmise ja struktuuri kohta Figma-s.

**Eelmistest koosolekutest veel üleval:**
* Figma make ja TEDI kooslus vajab veel testimist, testitud varasemas etapis võimalik et Make on arenenud. 
* Map componentsis külgpaneeli parem sulgemise/avamise lahendus
* Vertical stepperi alamsammude kuvamine mobiilis
* TTJA NBA, Rahvastikuregustri menetluskeskkond: vajadus tabelis/lingil eristada mida on külastatud mida mitte.
* Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis mingi konflikti kui headeris kõik väärtused sisselülitada, brand värvi peal pole searchi hinti näha
