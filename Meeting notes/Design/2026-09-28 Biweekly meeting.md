*Tegu on AI kokkuvõttega*

# Peamised punktid

## Komponentide uuendused
- Timeline koondati Figmas terviklikuks komponendiks — elemente saab lisada ja järjestada slotina, ilma eraldi tükke kokku panemata. Kärolin tegi ettepaneku rakendada sama lähenemist ka stepperi puhul (pole veel tehtud).
- Checkbox-grupile tehti slot-põhine muudatus (label ja tagasiside koos kaartidega üheks tervikuks), kuid seda pole veel avalikustatud.
- Dropdown lihtsustatakse ühetasandiliseks slot-toega variandiks, et vähendada keerukust ja kiirendada prototüüpimist.
- Uued Reacti komponendid jõudsid eelmisel nädalal tarnesse: CardStepper, TableCard ja VerticalStepper. TableCard on responsive (mobiilis kaart, desktopis tabel), VerticalStepper toetab linke, nuppe ja eri olekuid.

## Angulari komponendid (TEDI-Ready)
Uued TEDI-Ready (Angular) komponendid:
- **FloatingButton** — lehe serva kinnitatud nupp, nt tagasiside andmiseks.
- **HeadingWithIcon** — pealkiri koos ikooniga, nt sektsioonide pealkirjades.
- **Skeleton** — sisu kohatäide, mida näidatakse andmete laadimise ajal.
- **TableOfContents** — pika lehe sisukord, mis näitab, millises osas kasutaja parasjagu on.
- **Truncate** — lühendab pika teksti ja laseb kasutajal seda vajadusel täismahus avada.

## TJT projekti küsimused
- **Kuhu kadusid kolm värvi?** Värvid ei ole kadunud — TEDI eelkäijaga võrreldes on neil uued nimed. Oranž muudeti tumedamaks (WCAG kontrastinõuete tõttu), ülejäänud kaks on uue nimega, kuid samade värvikoodidega.
- **Miks kadus textarea juurest sulgemisnupp (closing button)?** Textareal ei ole remove-nuppu ette nähtud.
- **Miks tooltip ei jää pärast klikkimist avatuks?** Popover jääb avatuks — probleemi ei tuvastatud.
- Soovitus: arendajad kommunikeerigu muresid otse dev-react kanalis, et vältida "telefonimängu".
- TJT kasutab praegu Reacti versiooni 17, kuid on liikumas versioonile 19.

## MAKI projekti küsimused
- **Kas tabi taustavärvi tohib muuta?** TEDI: projekt võib vajadusel ise värvimuudatuse teha, kuid TEDI soovitab värvi samaks jätta.
- Kui hall ja valge omavahel ära vahetada, ei ole visuaalne erisus TEDI-ga enam nii suur.
- Aktiivset tabi tähistab rasvane (bold) tekst ja border, seega taustavärv hetkel staatust ei kanna.

## STAR projekti vajadused
- STAR soovib labelile lisasuurusi: label on Figmas fikseeritud laiusega, kuid neil on vaja veel laiemat varianti.
- TEDI: projekt võib seda oma vajaduste järgi muuta, kuid soovitab teha GitHubi discussion'i. Kui tegu on pisimuudatusega, võib selle lisada ka TEDI Figmasse, et projektidel oleks lihtsam kasutada — sama vajadust on väljendanud ka teine projekt.
- Tegu on üksnes disaini ja Figma teemaga, mitte arendusega.

## Aatomdisaini põhimõtted
- TEDI uuris disaineritelt, kas aatomdisaini põhimõtete kommunikeerimine ja visualiseerimine (nt märgis iga komponendi juures) lisaks väärtust.
- Disainerid: iga komponendi juures eraldi märgist pole vaja — põhimõtted on neile selged ja teada. Vajaduse korral on see info pigem kasulik tooteomanikele ja projektijuhtidele.

# Otsused
- Vajadus on tervikkomponentide järgi, mille sees on slot: vertikaalne stepper, horisontaalne stepper, dropdown ja tabel. Disainerid näevad selles väärtust ja see lihtsustab tööd.
- Praegune frame'ide ülesehitus Figmas ei ole disainereid segadusse ajanud; küll aga vaatavad nad Figmas kindlasti näiteid, kasutusnäiteid ja variante.

## Eelmine koosolek
- Jagada kokkuvõtete linke ja otsustada meeskonnaga, kas TEDI koosolekute videod jäävad salvestatuna jagamisele või piisab videokokkuvõtetest. (Kärolin)
- Jagada TEDI tiimiga MAKI tabide praegune visuaal, et saaks hinnata. (Kärolin)
- Lisada Reacti tiimile hidden text field -komponent (inline edit) ja jagada dokumentatsiooni lingid.
- Koostada uute komponentide (TableCard, stepperid) kasutusjuhendid.

**Projektide disainerid**
- Saata Kärolinile TEDI komponente kasutavate projektide lingid. (eelmisest)
- Stiilida väliste tekstiredaktorite teegid TEDI disainikeele järgi. (eelmisest)
- TTJA NBA ja Rahvastikuregistri menetluskeskkond: eristada külastatud ja külastamata olekuid. (eelmisest)
- AKS: Card header ja card vertical konflikt; brand-värvi peal pole searchi hint näha. (eelmisest)

**Arendusmeeskond**
- Rakendada ja testida uusi komponente (inline edit, tekstigrupi slot, sisukorra komponendi uued elemendid). (eelmisest)
- Teha radionuppude ja checkboxide muudatused ning eemaldada Choice Group. (eelmisest)
