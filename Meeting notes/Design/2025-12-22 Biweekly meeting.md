# 2025-12-22 Regulaarne disainikoosolek

## Osalejad
* Kärolin Kivisikk
* Helis Sepp
* Helis Lembe
* Kristel Ojamaa
* Joanna Joa

https://bitwebou-my.sharepoint.com/:v:/r/personal/karolin_kivisikk_bitweb_ee/Documents/Recordings/Disaineritele%20TEDI%20komponendid-20251222_160316-Meeting%20Recording.mp4?csf=1&web=1&e=aW0IgJ&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

## Päevakord
* Community faili kasutust ja selle tulevik
* Filtrikomponentide disain ja kasutusvõimalused nii desktopi kui mobiilseadmete jaoks

## Demo
* TEDI community Figma faili kasutamine ja selle tulevik (komponentide dubleerimine, kustutamine, õigused)
  * Tulevased plaanid community faili korrastamiseks ja komponentide haldamiseks
  * Community failis on praegu dubleeritud komponendid, mis on TEDI Redis failis juba olemas.
  * Plaan on community failist aegamisi eemaldada komponendid, mis on TEDI Redis olemas, et vältida segadust ja dubleerimist.
  * Mõned komponendid, näiteks erivärvilised tagid mkis kasutusel STARis, jäävad community faili, kuna TEDI-readysse neid ei too (nt WCAG nõuetele mittevastavus).
  * Kõikidele TEDI Figmas olevatele disaineritele saab külge TEDI Community edit õigus, et saaks seal uusi komponente arendada enne TEDI-Readysse viimist.
  * Community failist hakkab toimuma ka järkjärgult stiilide eemaldamine (fondid, värvid, vahed jms) sest TEDI-Readys on need muutujaidena olemas ja saab neid kasutada. Muuljuhul võib põhjustada segadust, kui mõlemad failid on korraga kasutuses ja tööfaili tulevad mõlemad muutujad/komponendid sisse (kaks buttonit jne).
* Filtrikomponentide disain ja kasutusmustrid mobiilis ja desktopis

## Vajadused ja muu tagasiside
Filtri komponendi tagasiside ja arutelud:
* Valitud filtrite tagid kuvatakse tavaliselt filtrite all ja neid saab üksikult eemaldada.
* Arutelus kas tagide kuvamine mobiilis on kohustuslik või vabatahtlik, jõuti järeldusele, et see peaks olema paindlik ja projektipõhine.
* Filtrite puhul on oluline ka grupeerimine ja sektsioonide eristamine, milleks kasutatakse separatorit (eraldusjoont).
* Arutati, et kui filtrite arv on suur (nt üle 15), võiks kasutada akordionlahendust või eraldi vaadet mobiilis, et hoida kasutajaliides kompaktne. Väiksema arvuga filtrite puhul võiks need olla kohe nähtavad.
* Filtrite kõrgused on erinevad: 24 px (väiksemad), 32 px (kompaktsemad) ja 40 px (koos vormielementidega sobivad).
* Arutati, kas filtrite kõrgused peaksid olema ühtlustatud või jääma erinevaks vastavalt kasutuskontekstile.
* Checkboxide kasutamine filtrites on eelistatud, sest see annab selgema visuaalse tagasiside valiku olekule (valitud vs mittevalitud).
* Mõned filtrid on ilma checkboxita, kuid valitud olekus lisatakse linnuke, et kasutajale selgemaks teha.
* Arutati ka filtrite ja sorteerimise nuppude visuaalset eristamist, et kasutajad saaksid neid hõlpsasti eristada.
* Filtrite suurused (24, 32, 40 px) ja nende sobivus erinevates kontekstides
* Multiselect valikute puhul lahendus peab arvestama 5 kuni 50 väärtusega
* Sorterimise ja tulemuste kuvamise lahendused filtrite juures
* Arenduslikud ja kasutajaliidese küsimused filtrite funktsionaalsuse osas
* Desktopis kasutatakse tavaliselt drop-down või ühe valikuga filtreid, mobiilis on plaan need wrappide kahele reale, et vältida horisontaalset kerimist aga ka lisada sidemodal pikemate multiselectide jaoks.
* Multiselektidega filtrid võimaldavad otsingut, valikute tühistamist ja valikute kuvamist tagidena (tägid)
* Tulemuste arv kuvatakse tavaliselt filtrite lähedal, et anda kasutajale tagasisidet valikute mõjust.
* Desktopis tabeli puhul on tulemuste arv tihti seotud paginatsiooniga, mobiilis võiks see olla eraldi nähtav päises mitte lõpus.
* Arutati, kas tulemuste arv peaks olema kohustuslik või vabatahtlik element filtrite juures, jõuti järeldusele, et see võiks olla paindlik ja projektipõhine.
* Sorteerimise nuppude kuvamine on planeeritud nii, et need oleksid eraldi nupuna, mis näitab aktiivset sorteerimiskriteeriumi.
* Arendajate jaoks on oluline, et filtrikomponendid oleksid ühtsed ja selged, et vältida segadust checkboxide ja radio nuppude vahel.
* Arutati, kuidas arenduslikult hallata filtrite kuvamist ja kas akordionlahendust saab paindlikult sisse/välja lülitada.
* Filtrite kuvamise reeglid (nt mitu valikut näidatakse, millal kasutatakse tagisid, millal akordionit) peaksid olema konfigureeritavad vastavalt projekti vajadustele.
* Arutati, et filtrite kuvamine võiks olla kasutajale intuitiivne, võimaldades kiiret valikute eemaldamist ja otsingut.
* Kontrollida ja koondada erinevad filtrite näited, sh ka need, mis ei kasuta praegust filtrikomponenti vaid kasutavad lihtsalt vormielemente (select, otsing, input jms), et luua ühtne näidiste kogu.
* Kas lisada filtrikomponendi valitud väärtustele linnuke (checkboxi stiilis) ja kasutada seda ühtselt nii filtrite kui vormielementide puhul?

## Otsused
* täiendada filtrikomponenti vastavalt vajadustele
* Uurida arendajate käest, kus ja kuidas kasutatakse väikest filtrisuurust ning kas seda on vaja hoida alles või võib eemaldada.

Eelmistest koosolekutest veel üleval:
* Otsing headerisse
* Vertical stepperi alamsammude kuvamine mobiilis
* Välisveebi komponentide vajaduste ja näidete kogumine
* Arvestada sooviga et arenduses saaks horisontaalset nav-i panna stickyma scrollimise peale
* Mõelda mis hetkest või loogika alusel horisontaalne menüü läheb mobiilseks - kas võimalik hallata arenduses et jääb kauemaks mittemobiilseks kui linke on vähem menüüs
* TTJA NBA, Rahvastikuregustri menetluskeskkond: vajadus tabelis/lingil eristada mida on külastatud mida mitte.
* Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis mingi konflikti kui headeris kõik väärtused sisselülitada, brand värvi peal pole searchi hinti näha

