*Tegu on AI kokkuvõttega*

# Peamised punktid

## Sheet ja sisukord
- Mitme-Sheet'i variant toetab paralleelselt avatud tööriistu — kasutaja vahetab Sheet'ide vahel, Sheet jääb avatuks kuni sulgemiseni (sulgemine käib ühe Sheet'i, mitte kogu komplekti kohta); Design Reviews'i lahendus tuleb pärast tavapärast Sheet'i.
- Sisukorra komponent saab nupuga avatava, kompaktse variandi pikkadele lehtedele; TEDI sisukord kuvab aktiivset elementi kerimiskoha järgi. Praegune näidis kasutab veel linke ja pealkirju, mitte täielikku komponenti.
- Mitut komponenti hõlmavad näited viiakse eraldi lehele, et põhikomponendi leht jääks puhtamaks (näited jäävad komponentidega lingituks).

## Figma struktuur ja dokumentatsioon
- Figma raamid korrastatakse komponendipõhiseks (checkbox ja checkbox card säilitavad nime); näidised, kaardid ja checkboxid tõstetakse eraldi, vana raam eemaldatakse (kahele komponendile juba rakendatud).
- Iga komponendi juurde lisatakse vaikimisi näidis (lingid, raamistikud, tehnoloogiad) ja anatoomiasektsioon (alamkomponendid, omadused, värvid, väärtused).
- Omadused esitatakse tabelipõhiselt (värvivariatsioonid, ikoon, kirjeldus, paigutus, mobiili/töölaua erinevused); lisatakse suuremad realistlikud kombinatsiooninäited.
- Valitud olekute interaktsioonid (hover, active, focus) dokumenteeritakse täielikumalt — kaetakse varem puudunud checkbox'i ja checkbox card'i olekud.

## Ligipääsetavus ja menüüd
- Lisandub Skip-to-content komponent: tab-klahviga ilmub lehe ülaossa ujuv element, mis Enteriga hüppab navigatsioonist põhisisu juurde (ka ekraanilugejatele); sulgub pärast edasiliikumist.
- Dropdown lihtsustatakse menüüelementide põhiseks (action ikoonidega, multi-select checkboxidega, raadiovalikud, kirjeldusega elemendid; avav nupp/trigger, sisu, vajadusel filtriväli).
- Lahtine: kas komponendi nimi jääb "dropdown" või muutub "menu"; samuti kollaps-nupu noole käitumine. Nimi pole veel avaldatud, oodatakse tagasisidet.

## Komponentide parandused
- Attachment: üleslaadimata failidel pole kustutamisnuppu; vigased failid kuvatakse esimesena ja neid saab eemaldada (muudatus jäi piiratud ulatusega, arenduse poolelt Riina).
- Teksti ja ikooni värv viidi sama muutuja alla, et vältida olukorda, kus üks muutub ja teine mitte (visuaalselt väike muudatus, kuid vähendab sünkroonimisvigu).

## Chat-komponent
- Chat on disainis enam-vähem valmis, liigub veel teise disaineri vaatesse; põhineb varasemate projektide vajadustel; oodatakse projektide tagasisidet enne arendusse liikumist.
- Toetab heledat ja halli tausta, avatari/initsiaale ning teksti-, attachment'i-, pildi- ja slot-sisu; eri osapoolte sõnumid peavad jääma eristatavaks.
- Sisaldab metaandmeid ja olekuid (kuupäev/kellaaeg, saadetud/loetud, divider'id nt tänaste/lugemata sõnumite jaoks); kaetud on error-olukorrad, clickable card, mitme chati vaade ja mobiilinäide.

## Graafikud
- Projektidelt kogutakse graafikuvajadusi (Disaini kanal + discussion); eesmärk on täpsustada, millised graafikavaated on tegelikult vaja.
- Lahtine, kas graafikud ehitada TEDI-sse või kasutada välist teeki (Figma komponent võib olla TEDI-s ka siis, kui arendus kasutab välist tehnoloogiat); ajastus veel ebaselge.
- Seni eelistatud tehniline kandidaat on Vissix (vektoripõhine, kerge, kohandatav, toetaks TEDI värve/komponente/tooltip'e); Chart.js hinnati vananenuks. Lõplik otsus arendusega üle kontrollida.

# Otsused
- Figma komponendiraamid korrastatakse komponendipõhiseks; vana raam eemaldatakse pärast sisu üleviimist.
- Igale komponendile lisatakse vaikimisi näidis ja anatoomiasektsioon; omadused esitatakse tabelipõhiselt.
- Ligipääsetavuse jaoks lisatakse Skip-to-content komponent.
- Dropdown lihtsustatakse menüüelementide põhiseks (nimi "dropdown" vs "menu" veel lahtine).

## Eelmine koosolek
**Projektide disainerid**
- Anda tagasisidet chat-komponendi katvuse kohta ja viidata olemasolevatele Figma lahendustele.
- Koguda ja jagada graafikuvajadused (Disaini kanal / discussion).
- Testida sisukorra komponendi scrollimis- ja sticky-lahendusi ning jagada tagasisidet. (eelmisest)
- Stiilida väliste tekstiredaktorite teegid TEDI disainikeele järgi. (eelmisest)
- TTJA NBA ja Rahvastikuregistri menetluskeskkond: eristada külastatud ja külastamata olekuid. (eelmisest)
- AKS: Card header ja card vertical konflikt; brand-värvi peal pole searchi hint näha. (eelmisest)

**Arendusmeeskond ja TEDI tiim**
- Lisada multi-Sheet'i variatsioon ja sisukorra kompaktne/nupuga avatav variant.
- Korrastada Figma komponendiraamid, lisada vaikimisi näidised ja anatoomiasektsioon, viia suuremad näited eraldi lehtedele ning eemaldada vana raam.
- Ühtlustada komponentide esitlus (tabelipõhine omaduste/värvide kuvamine) ja täiendada valitud olekuid (hover/active/focus, sh checkbox ja checkbox card).
- Lisada Skip-to-content komponent.
- Lihtsustada dropdown/menüü lahendust; otsustada nimetus (dropdown vs menu) ja kollaps-nupu noole käitumine.
- Hinnata graafikute lisamist TEDI-sse (TEDI sisse vs väline teek, seni eelistus Vissix) ja arutada arendusega.
- Lisada pop-overi taustale tumedama kihi/varju võimalus ja avada GitHubi diskussioon. (eelmisest)
