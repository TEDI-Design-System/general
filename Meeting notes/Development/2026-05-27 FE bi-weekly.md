# 2026-05-27 FE bi-weekly

## Osalejad: 
* Airike Jaska
* Märt Sessman
* Tõnis Tobre
* Ly Tempel
* Kaia Jallai
* Erki Dobrek
* Kristi Jõgeva
* Juri Gurjev
* Pearu Sarv
* Evelin Orgmets
* Oliver Vaga
* Priit Puru
* Marta Kisand-Ekmekci



## Teemad
* **Release**
  * REACTis: DateField; input Field, mis põhineb TextField alusel; Slider, TimeField, TimePickerit saab nüüd standaolne kasutada; EmptyState (communitys vist placeholder nimega), Pagination (osaliselt TEDI-READYs, sest modaali komponent puudu); Calendar, Header. HEaderis mõned uuendused, nt CustomRoleContent.
  * ANGULARis: HorizontalStepper, Filter, StatusIndicator. Selectil saab vaikimisi väärust muuta ja outpute tuli juurde. Collapse bugi parandused

* **Pooleli olevad komponendid**
  * REACTis:
    * Tabeli komponent ootab code reviewd, design reviewst läbi
    * Breadcrumbs on samamoodi code reviews
    * Uusim komponent on HorizontalNavigation
    * Footeri komponent ootab idsaineri inputi. Desktopi oma jääb nagu on, aga mobiili jaoks vaja uusi muutujaid.
    * DateTimeField ootas DateField ja TimeField järele
    * Modal on tulemas. Kplm haru sellest on ka tegemisel
    * Planeeritud HeaderPro
  * ANGULARis: 
    * Attachment oli varem community file droppzone'is, sai extractitud ja natuke ümber tehtud. Sinna sisse saab nüüd panna progress bari. Sellega seoses sai tehtud ka muudatus (vastavalt feedbackile võib revertida, aga oleks vaja tead, mis muuta). Asendatud sai built in versioon. Vanas versiooonis kuvati error ikooni nupu küljes ja sulgemise nupul oli label vale. Nüüd uus variant selline, et sõnum on alati attachmenti all, mitte tooltipis ning võimalik näidata failis suurust, eemaldamise nupp on nüüd prügikast. On nagu breaking change, aga sooviks teada kasutajatelt, kas see on suur asi, kui asendatakse või ei? Keegi midagi ei kommenteerinud
    * ButtonGroup on pooleli
    * DateField puhul avades kalendrit modaalis, saab määrata, mis breakingpointist avab vaikimisi. Samamoodi nativepickerid on olemas.
    * Suurim asi, mis töös, on Table
    * Acordioniga tegeletakse
    * Planeeritud HeaderPro
 
