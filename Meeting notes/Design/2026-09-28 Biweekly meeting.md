*Tegu on AI kokkuvõttega*

# Peamised punktid

## Komponentide uuendused
- Timeline ja stepper koondati Figmas tervikkomponentideks — itemeid saab slotiga lisada ja järjestada, ei pea tükke ise kokku panema; vertikaalne ja horisontaalne stepper on nüüd üks komponent.
- Checkbox grupile tehti slotipõhine muudatus (label ja tagasiside koos kaartidega üheks tervikuks) — veel avaldamata, oodatakse disainerite tagasisidet.
- Dropdown lihtsustatakse: üks tase ja slotid elementide jaoks, et vähendada keerukust ja kiirendada prototüüpimist.
- Uued Reacti komponendid TableCard ja vertikaalne stepper on tarnes — TableCard on responsive (mobiilis kaart, desktopis tabel), stepper toetab linke, nuppe ja eri olekuid.

## Disainisüsteemi struktuur ja dokumentatsioon
- Figma komponentide hierarhia muudetakse: tervikkomponendid ette, väiksemad tükid alla; päisesse plaanis WCAG-vastavuse staatus.
- Kaalutakse märget, kas komponent on aatom, organism või mall — pigem valikuline, et vältida infomüra.
- Disainisüsteemi lisatakse näidisvaated ja mallid (nt multistep-vormid) juhiste ja inspiratsioonina, mitte kohustuslikena.

## Värvid ja ligipääsetavus
- Oranž muudeti tumedamaks WCAG kontrastinõuete tõttu (timeline'il oli kontrast taustaga liiga väike); vana oranži saab soovi korral käsitsi projekti paletti lisada.
- Migratsiooni käigus uuendatakse värvinimed (vanad nimed kadunud) — juhend on migratsiooni dokumentatsioonis.

## Kasutajaliidese detailid
- Tooltip avaneb kas hoveriga või klikiga (jääb avatuks kuni väljaspool klõpsuni) — valik on projekti teha.
- Tabide taustavärv ja aktiivsus vajavad täiendavat analüüsi (valge vs hall taust); aktiivsel tabil on praegu sinine joon.
- Labelitel on kolm vaikelaiust (nt 32 ja 64 px), plaanis lisada 1–2 juurde; Figma Resizer võimaldab laiust muuta, kuid on keerukas ja vajab tagasisidet.

## Koostöö ja vastutused
- Arendus kasutab React 19; suhtlus käib Slacki arenduskanalis kiire tagasiside jaoks.
- Vastutused: aatomid (pisikomponendid) on disainisüsteemi oma, suuremad korduvad mustrid võivad olla projektipõhised või disainisüsteemi komponendid.

# Otsused
- Timeline, stepper ja (tulekul) dropdown pakutakse tervikkomponentidena slotipõhiselt.
- Oranž värv muudeti WCAG nõuete tõttu tumedamaks, projektil oli küsimus miks orange-600 muutunud on;
- Komponentide vastutus: aatomid disainisüsteemis, suuremad mustrid projektipõhiselt või disainisüsteemis.

## Eelmine koosolek
- Jagada kokkuvõtete linke ja otsustada meeskonnaga, kas koosolekute videod jäävad salvestatuna jagamisele või piisab videokokkuvõtetest. (Kärolin)

**Projektide disainerid**
- Anda tagasisidet checkbox grupi slotipõhise muudatuse ja kaardi-sloti kohta.
- Testida sisukorra komponendi scrollimis- ja sticky-lahendusi ning jagada tagasisidet. (eelmisest)
- Stiilida väliste tekstiredaktorite teegid TEDI disainikeele järgi. (eelmisest)
- TTJA NBA ja Rahvastikuregistri menetluskeskkond: eristada külastatud ja külastamata olekuid. (eelmisest)
- AKS: Card header ja card vertical konflikt; brand-värvi peal pole searchi hint näha. (eelmisest)

**Arendusmeeskond ja TEDI tiim**
- Luua lihtsustatud dropdown-komponent (üks tase, slotid).
- Lisada Reacti "inline edit" komponent (endine hidden text field) ja jagada dokumentatsiooni lingid.
- Täiendada TableCard ja stepper komponente vajadusel ning anda kasutusjuhendid.
- Viia läbi Figma komponentide ülesehituse ümberkorraldus ja oodata tagasisidet.
- Vaadata üle tooltipi kliki käitumine ja saata lingid arendustiimile.
- Kontrollida horisontaalsete tabide taustavärvi ja parandada kasutajakogemust (nt vaikimisi valge taust tabelites).
- Lisada pop-overi taustale tumedama kihi/varju võimalus ja avada GitHubi diskussioon. (eelmisest)
