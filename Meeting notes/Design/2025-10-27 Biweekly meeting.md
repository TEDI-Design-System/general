# 2025-10-27 Regulaarne disainikoosolek

Osalejad: 
* Kärolin Kivisikk
* Henry Semmel
* Marju Sild
* Kristel Ojamaa
* Gerli Liiv
* Karis Karindi - RIK
* Johhanna Loomets
* Norman Järve
* Joanna Joa
* Siret Tuula
* Maris Jool
* Ingrid Aasoja-Zverev

Video: https://bitwebou-my.sharepoint.com/:v:/r/personal/karolin_kivisikk_bitweb_ee/Documents/Recordings/Disaineritele%20TEDI%20komponendid-20251027_160124-Meeting%20Recording.mp4?csf=1&web=1&e=wz6vkw&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

## Demo
* Text group kohandatava pikkusega label
* Github Wishlist discussionite loogika

## Vajadused ja muu tagasiside
* Kristel Ojamaa, MaRu projekt, Aadresside ja Kohanimede Süsteem (AKS): 
  * Community komponentidest nad kasutavad tertiary nuppu, sama nagu TEDI-Readys ka olemas kuid Communitys oli selles x-padding olemas + hover/active taust. TEDI-Ready komponent tugineb Veerale, vasak/parem padding on eemaldatud et nuppu paremini tekstidega joondada kuna tihti kasutatakse 'Tagasi' nupuna ning et nuppude vahed oleksid visuaalselt ühtlasemad kuna läbipaistva nupu vasak/parem padding tekitab visuaalselt ebaühtlase vahe nuppude vahel kus osad omavad bordereid/taustavärvi.
  * AKS-il on mure kuna varasema nupu klikatavuse/hover paistis paremini silma kuna nupp muutis ka enda tausta. TEDI nupp muudab vaid teksti värvi + kursor muudab kuju.
  * Mure on hetkel ennatlik ning pole teada kas põhjustab kasutajate seas segadust. 
  * **Lahendus**: Hetkel TEDI komponenti ei muuda sest teistes projektides ei ole probleemiks osutunud, lisaks tugineb TEDI nupp Veeral. AKS-il on võimalus ise lisada hover olek enda projekti-põhiselt, mida nad koosolekul otsustasid et siiski ei tee hetkel. Küll aga jääb Community nupp alles kuna sellel puudub TEDI-Readys vaste siis seniks pole ohtu et see kustutatakse, seega seda Community nuppu võivad ka hetkel edasi kasutada. TEDI soovitus oli sellest github wishlist discussion luua ja kui ka teistel projektidel huvi sellise nupu järgi siis saab selle töösse vajadusel võtta.
    * Sireti vastus kinnitas et juhul kui peaksime selle nupu eemaldama siis anname pikemalt ette teada, hetkel jääb nupp communitysse alles.
* Joanna Joa, STAR projekt, File upload + progressbar:
  * Hetkel TEDI-Ready Figmas puudub lahendus kuidas progressbari attachmenti sees kasutada. STAR-is peab see progressbar aga konkreetse failiga seotud olema. Progressbar hetkel puudub TEDI-ready arendusest, STAR on ise arendanud selle
    * **Lahendus**: Las projekt disainib selle progressbari sinna sisse ise hetkel, TEDI disainiga hiljem põrgatada kuna hetkel ei ole ressurssi nii kiiresti seda Figmasse luua, siis koostöös saame vajaliku stiili/visuaali paika panna ning hiljem saab TEDI figmasse selle ümber tuua. 
  * File upload komponent puudus ka Angularis, TEDI-Readys ehk et praegu arendavad ise communityna. Küsimus kas failid hakkavad kohe üles laadima kui nad dropzone-i lisatakse või peab mingit nuppu vajutama
    * **Lahendus**: Failid peaks automaatselt üles laadima kui nad on dropzone-i lisatud.
  * Kristel Ojamaa, MaRu projekt, Aadresside ja Kohanimede Süsteem (AKS):
    *  Otsingu sisend on nii pikk et üherealisel otsingul ei näe teksti lõppu, aadressi nimed on nii pikad.
    *  TEDI ei toeta mitmerealist otsinguvälja
    * **Lahendus**: AKS võib ise teha vajadusel kas kaherealise, TEDI ise seda ei toeta, või kuvada otsitav nimi otsinguvälja all kuna tegu võib olla pika nimetusega, või teha lainev otsinguväli ehk peale klikates väli laieneb (ka ei sobi kuna väikestel ekraanidel jääb ikka kitsaks)
    * 

## Otsused
* STARis Joanna loob ise progressbariga vajaliku komponendi disainis
* Hetkel uusi nuppe TEDI-sse juurde ei too kuna vajadus vaid ühes projektis
  
Eelmistest koosolekutest veel üleval:
* Otsing headerisse
* Horisontaalne header luua
* Vertical stepperi alamsammude kuvamine mobiilis
* Välisveebi komponentide vajaduste ja näidete kogumine
* Filtrite Figma disaini prioritiseerida
