# 2026-01-21 FE bi-weekly

## Teemad

* **Komponentide uuendused ja migratsioon**
  * Otsustati eemaldada neli Reacti community komponenti ja asendada need TEDI-READY ekvivalentidega.
  * Valmis on põhjalikud migratsioonijuhised, mis lingitakse järgmise release’i märkustesse, et üleminek oleks arendajatele selge ja sujuv.

* **Angulari breaking change’id ja ligipääsetavus**
  * Number field’i ja toggle’i komponentides tehakse breaking change’id, mis parandavad ID-de kasutust.
  * Muudatuste eesmärk on vähendada topelt-ID probleeme ja parandada WCAG nõuetele vastavust.
  * Üleminekut on võimalik teha sammhaaval, vajadusel säilitades ajutiselt tagurpidi ühilduvuse.

* **Figma integratsioon ja arendusprotsess**
  * Tutvustati Figma uut loogikat, mis võimaldab projektipõhist muutujate üle kirjutamist.
  * See loob eeldused projektipõhiseks sünkroonimiseks disaini ja frontendi vahel ning vähendab käsitsi tehtavat tööd.
  * Arutati vajadust tööriista või käsu järele, mis võimaldaks Figma projektist muutujad automaatselt frontendi tuua.

* **Bugid ja kvaliteedikontroll**
  * Tõstatati probleem akkordeoni värvimuutusega valitud olekus, mis võib olla bugi või disainimuutus.
  * Arutati close-nupu paigutuse ja overflow probleemi, mis mõjutab kasutajakogemust ja ligipääsetavust.
  * Otsustati teha vastavad issue’d ja lahendada probleemid esimesel võimalusel.

* **Koosoleku protsess ja koostöö**
  * Lepiti kokku, et edaspidi saadetakse enne koosolekuid välja agenda.
  * Hakatakse kasutama AI-põhiseid koosolekukokkuvõtteid, mis lisatakse avalikult GitHubi.
