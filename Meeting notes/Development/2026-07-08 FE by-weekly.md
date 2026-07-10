# 2026-07-08 FE bi-weekly

## Osalejad: 
* Märt Sessman
* Tõnis Tobre
* Ly Tempel
* Kaia Jallai
* Ardo Kirsipuu
* Erki Dobek
* Pearu Sarv


## Teemad
* **Release**
  * Tuli rohkelt uusi komponente nii Reacti kui Angulari jaoks. Toimusid ka mitmed parandused ja täiendused. Kogu nimekiri nähtav: https://www.tedi.ee/1ee8444b7/p/0316fd-release-notes
  * Storybook uuendatud 10 versioonile. Sai tehtud ka visuaalne uuendus

* **Pooleli olevad komponendid**
  * ANGULARis: 
    * Slide komponent on olemas, hetkel design reviews
    * Bredcrumbs on Reactist üle toodud. Võimalik on collapsed puhul mitu kirjet kuvada enne ja pärast. Custom separator võimalus
    * Label sai tooltip supporti. Lihtsustatud nii InfoButtoni ja ToolTipi kasutust.
    * DateTimeField paneb kokku DateField ja TimeFieldi. Erinevad võimalused olemas selle jaoks. PreDefined slot näiteks visiidi aegaele. Saab määrata päeva kaupa. Multistep on veel arutamisel täpsemalt kuidas seda saaks teha.
    * Rating on hetkel veel pooleli. Olemas disaini laual, kuidas see käituma peaks. Näiteks kas on poolik täht võimalik või ei. Võimalus ka custom ikoonidele, saada numbrid ja rahulolu näod.
    * Searchiga tegelemine, sarnane Reacti omale
  * REACTis:
    * Vertical Stepper on suures osas valmis ja üles pandud
    * Timeline on nüüd olemas, Reactist üle toodud. Hetkel Design reviews
  * HeaderTop tulemas Angulari ja Reacti. Lisandub ka header language dropdown.
   
 * **Muud teemad**
    * Pärast releasi sai avastatud, et TopNavil on label stiil katki ning valed design tokenid olid kasutusel. See sai parandatud ja ootab code reviews.
    * TEDI muutujayte eksport plugin sai täiendust. Tekkis probleem, kus Figmas Extenditud TEDI muutujate kollektsioon kasutas enda sees Figma muutujaid, mis on täiesti eraldiseisvad private kollektsioonidest. Need ei tulnud ekpordiga kaasa CSS muutujatena. Varem exporditi ainult TEDI enda omi + kõik TEDI extended omad. See sai muudetud. Nüüd loob theme nimega klassi, kus asuvad kõik CSS muutujad ja failinimi. Kui on mingi kollektsioon, mida peaks saama kasutada ka custom komponentidel, mis pole TEDIga väga seotud ja on custom, siis neid saab ka nüüd eksportida
    * TextGroupi probleem, kus kitsal ekraanil ei mahu value ära ja label hakkab väiksemaks minema, mis muudab asja visuaalselt ebaühtlaseks. Peaks järgmisele reale breakima. Hetkel veel testitakse
    * FloatingWindow puhul tuli välja modal issue Reactis ühe projektiga. Võiks tekkdia aken, mida saab vähendada, muuta ja ei tohiks olla backdropiks. Hetkel suurt huvi selle vastu ei ole
    * Kas rick text editor peaks TEDIl olemas olema? PRaegu on deprecated simple text editor. Kuna raske implementeerida ja keeruline, siis TEDI tuumik arutab seda järgmisel koosolekul.
    * Tuli küsimus InfoTooltipi kohta: InfoTooltipi komponent on lableis toetatud. Kas on võimalik nii, et ei anna ainult stringi ette, vaid ka keerukamat sisu? Näiteks tekst boldis. HTML peaks seda võimaldama
    * 
 
