# 2025-11-24 Regulaarne disainikoosolek

## Osalejad
* Kärolin Kivisikk
* Gerli Liiv
* Maris Jool
* Kristel Ojamaa + mitu inimest
* Norman Järve
* Lauri Tõnisson
* Johhanna Loomets
* Helis Lembe
* Henry Semmel
* Kätrin Uduste

https://bitwebou-my.sharepoint.com/:v:/r/personal/karolin_kivisikk_bitweb_ee/Documents/Recordings/Disaineritele%20TEDI%20komponendid-20251124_160109-Meeting%20Recording.mp4?csf=1&web=1&e=zDeYm1&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

## Demo
* Figjam protsessijoonis
* _Discussion_ - valge infonupu loomine + külgmenüüsse lisamine: https://github.com/orgs/TEDI-Design-System/discussions/54
  * Vajadus: Rahvastikuregistri menetlustarkvaral, Kristel tõi välja aadresside süsteemis vajaduse (selgub alles lõppkliendiga) ning fakti et kaardikomponentides on hele infonupp olemas - üle vaadata
* _Discussion_ - horisontaalne timeline: https://github.com/orgs/TEDI-Design-System/discussions/60
  * Vajadus: E-ehitus, MSA 
* _Discussion_ - fikseeritud külgmenüü päis ja jalus: https://github.com/orgs/TEDI-Design-System/discussions/55
  * Vajadus: Rahvastikuregistri menetlustarkvaral, Aadresside süsteemil on potentsiaalne huvi (Kristel Ojamaa) aga hetkel pole vajadust olnud kuna on header kasutusel
* Horisontaalne navigatsioon 
  * Vajadus: RIT, RIK, MUIS, MSA
  * Lauri tõi välja et tuleks läbi mõelda ka tahvli suurus - millal see menüü läheb mobiili peale? Sest vahel on parem kui nav itemid on näha sest ruumi on kuid vahel võib alamlinkidega dropdown minna liiga pikaks nii et kasutaja peab scrollima hakkama.
  * Helis ja Kätrin soovivad et horisontalne menüü oleks sticky või sticky funktsionaalsus rakenduks üles scrollides
  * Kirstel tõi välja et neil on horisontaalse menüü vajadus kuid praegu on eristatud vanad ja uued lingid vasaku ja parempoolse joondusega - pole hea UX lahendus, TEDI lisab divideri menüüsse
  * Praegune variant katab olemasolevate projektide vajadused
* Lokaalse komponendi loomine kasutades sisemiselt TEDI komponenti

## Vajadused ja muu tagasiside
* Kristel Ojamaa, MaRu projekt, Aadresside ja Kohanimede Süsteem (AKS, MaRu): 
  * Külgmenüül hakkavad olema pikad alamsammud, alamsamme on väga palju - täpsustab TEDI tiimiga eraldi vajaduse kuna peab enne kliendiga arutama mis alles jääb mis kaob jne.
    * **Lahendus**: Võimalik et TEDIs on tarvis luua alammenüü jaoks sarnaselt eesti.ee-ga lahendus kus alampunktid võivad olla laused ja neid saab struktureerida paremini. Praegune külgmenüü võib paljudele vajadustele kitsaks jääda. 

## Otsused
* luua valge infonupp, vaadata üle kaardikomponentidest kas seal juba ei ole loodud
* arvestada sooviga et arenduses saaks horisontaalset nav-i panna stickyma scrollimise peale
* lisada separator horisontaalsse menüüsse
* mõelda mis hetkest või loogika alusel horisontaalne menüü läheb mobiilseks - kas võimalik hallata arenduses et jääb kauemaks mittemobiilseks kui linke on vähem menüüs
  
Eelmistest koosolekutest veel üleval:
* Otsing headerisse
* Vertical stepperi alamsammude kuvamine mobiilis
* Välisveebi komponentide vajaduste ja näidete kogumine
* Filtrite Figma disaini prioritiseerida
