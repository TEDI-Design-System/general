# 2026-01-19 Regulaarne disainikoosolek

## Osalejad
- Kristel Ojamaa
- Gerli Liiv
- Katre Suits
- Einar Arro
- Daisy Pukkonen
- Liina Kukk
- Helis Lembe
- Kärol-Milaine Puunurm
- Joanna Joa
- Lauri Tõnisson
- Piret Tabor
- Maris Jool
- Karis Karindi

https://bitwebou-my.sharepoint.com/:v:/r/personal/karolin_kivisikk_bitweb_ee/Documents/Recordings/Disaineritele%20TEDI%20komponendid-20260119_160122-Meeting%20Recording.mp4?csf=1&web=1&e=q8l34X&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

## Päevakord
* Demo: top header, headerisse linke juurde lisatud ja search lisatud ja variandid kaotatud ning selle asemel mode'idega lahendatud, feedback vormi komponent
* Communityst kustutatavad komponendid ja nende migratsiooniplaan 

# Küsimused disaineritelt
* Einar Arro, tellija: KEMIT
  * Kaardirakenduse kihtidega külgmenüü kuvamine peitmine UX lahendus vajaks parandamist - praegune on 3vaate vahel vahetamiseks mõeldud ja ei ole intuitiivne
    * Vastus: teha enda projektis sobiv lahendus hetkel TEDI tiim ei jõua seda muuta kuid nõus et see vajab lahendus juhul kui tegu ei ole 3 vaatega vaid ongi tarvis vaid külgmenüüd peita/kuvada, siis vajab palju kergemat ja intuitiivsemat lahendust. 
  * Kaardirakendus on uputatud ning omav 2 sammulist protsessi -> 1) vormiväljad 2) kaardil märkimine. Küsimus oli et kui kaardil märkimist tehakse siis kuidas pärast vormiväljade ssammuni tagasi saab?
    *  Vastus: TEDI seda ei reguleeri, projektipõhine lahendus, soovitus on kasutada kas lehe all või üleval ääres keskel floativaid nuppe (Tühista, Salvesta) mis siis viivad tagasi vormivaatesse peale joonistamist. Võib ka kasutada TEDI kaardikomponentidesse loodud kaardinuppe 'tagasi' noolega.
  * Kui kaardikihte kõiki korraga peita tahta mis lahendus tuleks teha, kus on näide?
    * Vastus: Kasutada switch nuppu näiteks külgpaneelis kus kõik ülejäänud kaardikihid ja nende kuvamine/peitmine, kuid see tuleb ise kokku panna, TEDI seda usecase-i ei kata ja see on projektivajadus
  * Kui kasutaja kihtide grupis linnutab alamkihte ja eemaldab neid kuid kihi gruppide visibility siwtch on väljas siis see funktsionaalsus kaardil ei kuva midagi?
    * Vastus: Jah X-GIS vajaduste järgi sai see selliselt tehtud et switch toggle kuvab visibilityt, kui seal alla seadistada kihte ja visibility on välja lülitatud siis kaardil ei kuvata seadistusi, kui visbility on sisselülitatud siis kuvatakse. Kui on soov selle käitumist muuta siis on see projekti enda teha TEDI pakub vaid komponente mitte ei defineeri käitumist. Küll aga kui X-GIS üks rakendus töötab selliselt siis on see KEMITi enda sisemiste kokkulepete teema et rakendused käitumuslikult oleksid sarnased sest tegu on ühe organisatsiooni erinevate rakendustega.
    * Kaardikomponendid on loodud tugevalt X-GIS kaardirakenduse vajadusi silmas pidades ning projekti vajadustest pole kõrvale kaldutud sest tegu on konkreetse hanke korras tellitud komponentidega.
* Kristel Ojamaa, tellija: MaRu, projekt: AKS
 * Kas toaste võib mujale paigutada sest vormis on veateated ja hooiatused ja hetkel ei paista see silma?
    * Vastus: Ei ole hea kui üle projekti on toastid erinevates kohtades siis tuleb leida sobiv koht vastavalt projektivajadustele ja TEDI komponent üle kirjutada. TOastis ei ole soovituslik kasutada warninguid ja erroreid kuid kui muudmoodi ei saa siis tasub jah toast nähtavamasse kohta panna kas siis keskele üles või üles paremasse nurka et toast jääks rohkem väljavaatesse.

# Discussionitest vajadus: sidenav jalus
* Hetkel kahes projektis vaja: KEMITis ja Rahvastikuregistri menetlustarkvara
* Teistes projektides vajadus puudub.

## Otsused
* Sidenavile lisada jalus ja päis
* Map componentsis külgpaneeli parem sulgemise/avamise lahendus

Eelmistest koosolekutest veel üleval:
* Vertical stepperi alamsammude kuvamine mobiilis
* Välisveebi komponentide vajaduste ja näidete kogumine
* TTJA NBA, Rahvastikuregustri menetluskeskkond: vajadus tabelis/lingil eristada mida on külastatud mida mitte.
* Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis mingi konflikti kui headeris kõik väärtused sisselülitada, brand värvi peal pole searchi hinti näha
