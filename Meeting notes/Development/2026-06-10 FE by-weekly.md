# 2026-06-10 FE by-weekly

## Osalejad:
* Valdo Taevere
* Märt Sessman
* Airike Jaska
* Tõnis Tobre
* Ivar Kallejärv
* Pearu Puru

## Teemad

* **Komponendid valmis releasiks** – uued RC-komponendid (filter, DateTime-väljad: date/time/date-time, modal, tabel) toetavad Angularit ja ootavad releasi. Top Nav sai nimemuudatuse, et paremini Side Naviga sobituda.
* **Töös olevad komponendid** – Horizontal Stepper ja Table of Contents disaini-/koodikontrollis; Progress Bar sai animeeritud väljundid; LII disainikontrollis.
* **React/Angular täiendused** – Time Field (Angulari enim hääli saanud komponent) lisatud RCS-i variatsioonidega; Paginator sai lehekülje suuruse valikud ja kohandatava tulemuste kuva; lisatud võimalus tulemuste malli üle kirjutada.
* **Tabelikomponent** – tagasiside põhjal jõudluse ja mobiilikogemuse parandused; dokumentatsiooni lisatud state-halduse juhised (sh kollapsitavad read vaikekuval) ja rohkem vabadust veergude renderdamisel.
* **Angular 22 + Float UI** – tugi lisatud, kuid toob breaking change'e. Float UI eemaldamine on prioriteet (PR olemas aprillist, aga konfliktid pidurdavad). Float UI-l põhinevad kalender-/popover-komponendid vajavad põhjalikku testimist.
* **Storybook v10** – parem laadimiskiirus, iga story kohta eraldi koodiblokk, lisatud puuduvad näited ja custom story'd.
* **Dropdown-triggeri direktiiv** – varem toimis ainult button-elementidel, nüüd ka custom-nuppude ja linkidega; lisatud aria-tähed ja tab-indeksite haldus. Mõned fookuse edge-case'id ootavad veel parandust.
* **Ellipsis-komponent** – uued positsioonivalikud (algus/lõpp); kasutusele võetakse ka datefieldis ja selektis.
* **Release** – hoitakse stabiilsena, ei kiirustata (välditakse eelmise jaanuari olukorda). Märt: ärilist kahju edasilükkamisest ei teki, kuna RTC kasutajad saavad juba testida. Tootjatele/disaineritele tuleb RC mõistet selgemalt kommunikeerida.

## Action items
* Float UI PR-i konfliktide lahendamine ja integreerimine järgmisesse RC-sse
* Datefield/Timefield modaalide toe lisamine
* Tabeli dokumentatsiooni ja Storybooki parandused
* Dropdown-triggeri direktiivi parandamine ja klaviatuurinavigatsiooni testimine
* Ellipsise viimine Angularisse (Datefield, selekt)
* RC-nimekirja ja disainilahenduste lihtsustamine tootjatele
* Release-kuupäeva planeerimine (vajadusel edasilükkamine)
