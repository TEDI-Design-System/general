# 2026-02-16 Regulaarne disainikoosolek

## Osalejad
- Kristi Jõgeva
- Gerli Liiv
- Henry Semmel
- Lauri Tõnisson
- Karis Karindi
- Joanna Joa
- Kristel Ojamaa
- Liis Ots
- Sten Rõnglep
- Maris Jool
- Siret Tuula
- Piret Tabor
- Katre Suits

https://bitwebou-my.sharepoint.com/:v:/r/personal/karolin_kivisikk_bitweb_ee/Documents/Recordings/Disaineritele%20TEDI%20komponendid-20260216_160012-Meeting%20Recording.mp4?csf=1&web=1&e=Ap51t6&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

## Päevakord
* Demo: töös lingi, accordioni ja separatori refacto

# TEDI poolt info
* Käimas on komponentide sisemine refaktoreerimine ja disaini ühtlustamine.
* Refaktoreerimise eesmärk on jõuda järgmisesse tarnesse (ca nädal pärast koosolekut).
* Mobiilivaate linkide uuendus suurendab eraldiseisvate linkide klikkimisalasid ja parandab kasutatavust.
* Separaatori komponendis on ühtlustatud property-nimed ja muutujad.
* Filtri- ja reitingukomponent on arendusepoolses kontrollis.
* Uute teemade ülevaatamine Discussionsi alt.
  * Rangelt soovituslik kasutajatel ise luua Figma diskussioone komponentide muudatusvajaduste kohta.
  * Hääletamine aitab prioriseerida arendust läbipaistvalt.
  * TEDI kasutajate arvu kasv suurendab vajadust struktureeritud tagasisideprotsessi järele.
  * Eesmärk on vältida dubleerimist ja arvestada mitme projekti vajadustega.

# Küsimused disaineritelt
**Kas Figma Make’i kasutamiseks on olemas üldised juhendid?**
Hetkel ametlikke juhendeid ei ole. Figma Make sobib visuaalsete prototüüpide loomiseks, kuid vajab hilisemat käsitsi silumist. Arendajate jaoks jäävad GitHub ja Storybook usaldusväärsemateks infoallikateks ning komponentide põhjalik dokumentatsioon on peamine töövahend. Make’i ja TEDI library integratsioon vajab täiendavat uurimist ning kogemuste jagamine disainikanalis on oodatud.

**Kas TJT projekti custom header võiks muutuda üldiseks TEDI komponendiks? Kuidas lahendada mobiilivaate headeri probleemid**
Lahendus on keerukas ja toetab mitut rolli ning teavituste loogikat. Enne üldistamist on vaja laiemat arutelu, et hinnata, kas see sobib universaalseks komponendiks või jääb projektispetsiifiliseks.
Teavitused tuleb muuta nähtavamaks ning rollide eristus selgemaks. Võimalik on kaaluda täiendavat top-header lahendust, hetkel tegu projektipõhise custom lahendusega. 

**Kas headeri logo peab alati nähtav olema?**
Arutati vajadust võimaldada logo nähtavuse sisse/välja lülitamist - nii Figmas kui arenduses. Lahendus peab jääma tehniliselt toimivaks ja paindlikuks, et sobituda erinevate projektide vajadustega.

# Discussionitest vajadus: sidenav jalus
* Hetkel kahes projektis vaja: KEMITis ja Rahvastikuregistri menetlustarkvara
* Teistes projektides vajadus puudub.

## Otsused
* Arenduse Headeri arenduses arvestada vajadust logo sisse-välja lülitada (mobiilis teemaks ruumipuuduse tõttu) - sama ka figmas
* Figma make ja TEDI kooslus vajab veel testimist, testitud varasemas etapis võimalik et Make on arenenud. 

Eelmistest koosolekutest veel üleval:
* Koguda projektidest chati/sõnumi disainid kokku üle projektide.
* Sidenavile lisada jalus ja päis
* Map componentsis külgpaneeli parem sulgemise/avamise lahendus
* Vertical stepperi alamsammude kuvamine mobiilis
* Välisveebi komponentide vajaduste ja näidete kogumine
* TTJA NBA, Rahvastikuregustri menetluskeskkond: vajadus tabelis/lingil eristada mida on külastatud mida mitte.
* Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis mingi konflikti kui headeris kõik väärtused sisselülitada, brand värvi peal pole searchi hinti näha
