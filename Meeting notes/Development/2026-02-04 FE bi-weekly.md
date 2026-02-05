# 2026-02-04 FE bi-weekly

AI genereeritud

## Teemad

* **Staatus update**
  * Angulari komponentides tehakse testidest tulenevaid parandusi.
  * Theme provideri loogikat lihtsustatakse – üldised teemad kaovad ning muutujad hallatakse edaspidi ainult Figmas ja tiimipõhiselt.
  * Tiimiga liitus uus frontend-arendaja Ly, kes tegeleb accordion-komponendiga.

* **Wishlist ja upvote protsess**
  * Arutati keerukust erinevate projektide soovide prioriseerimisel.
  * Otsustati lähtuda põhimõttest: mida rohkem sooviavaldajaid, seda kõrgem prioriteet.
  * Tõnis tutvustas uuesti GitHub Discussions’i kasutamist soovide kogumiseks.
  * Protsess aitab vähendada subjektiivseid otsuseid ja tõstab läbipaistvust.

* **Vue komponendid**
  * RIK on avaldanud soovi Vue komponente arendada ja alustab nende ehitamist.

* **Storybook ja Reacti versioonid**
  * Storybook kasutab hetkel React 18.3.1, kuid TEDI toetab ka React 19.
  * Ilmnesid erinevused komponentide käitumises React 18 ja 19 vahel, sh probleemid iPhone’i vaates.
  * Leiti, et osad komponendid töötavad Storybookis, kuid mitte rakenduses.
  * Paluti teha vastav bugi, et probleem saaks jälgitavaks ja lahendatavaks.
  * Arutati vajadust võtta Storybooki versioonikonfliktid eraldi taskina ette.

* **Header ja mobiilivaade**
  * Community headeri mobiilivaade ei skaleeru hästi ning ei toeta kogu desktopi funktsionaalsust.
  * Probleemiks on custom-contenti kuvamine mobiilis ja info koondamine kasutajamenüü alla.
  * Leiti, et lahendus vajab esmalt disainikoosolekul lahtimõtestamist.
  * Tarmo demonstreeris konkreetset probleemi ekraanil.

* **Muud teemad**
  * TEDI Ready komponente võib ja võib igaüks parandada.
  * Pakuti ideed motiveerida aktiivsemaid wishlisti kasutajaid auhindadega.
  * Chromaticu snapshotide limiit on endiselt täis ja vajab eraldi lahendust.
  * Arutati, et release notes’i “source of truth” on Zeroheight, kuid sellele tuleb arendajaid paremini suunata.
  * Puudub selge ülevaade RC release notes’idest, mis tekitab segadust versioonide vahel liikumisel.
