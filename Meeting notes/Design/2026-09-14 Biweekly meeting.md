# Peamised punktid

## Sheet-komponent
- Sheet toimib modaalaknana ja sobib nii mobiili- kui veebivaatesse; päise saab avatuks jätta, lisada staatuseid ja tekste slotina ning kasutada nuppudega või ilma.
- Mobiilis toetab vorme (nt filtreerimine, sorteerimine); desktopiversioon on arenduses (suuremad vormid, infopaneelid, ekraaniserva lukustatav lai paneel).
- Lisandub täpsem dokumentatsioon ja komponendi kõrguse reguleerimine; MVP v1.3 sisaldab teemakaardi valikut ja dropdown'i.

## Reitingukomponent
- Lisati Hover, Disabled ja Focus olekud ning read-only režiim (hinnangu kuvamiseks ilma muutmiseta).
- Sobib avaliku sektori vajadustega, kus hinnang on sageli sisend, mitte avalik näit; toetab tärne ja emotsioone.

## Külgmenüü
- Toetab 2- ja 3-tasandilist navigeerimist; 3. tase lisati, kuid vajab visuaalset selgust — kaks varianti: laiendatud külgmenüü lisapaneeliga või kitsam dropdown-laadne lahendus.
- Päise ja jaluse saab slotidega konfigureerida või ruumi säästmiseks peita; mobiilis eraldab klikitav pärand navigeerimise ja alamlinkide avamise.
- Pärandite klikitavus tuleks projektiüleselt ühtlustada.

## Teemarežiimid
- Kolm režiimi (hele, tume, süsteemi vaikimisi); vahetuskomponendil on nii dropdown kui väiksed nupud, label nähtav või peidetud.
- Soovituslik on dropdown; oodatakse tagasisidet, et lahendusi projektiüleselt ühtlustada.

## Pop-over ja overlay
- Pop-overi taust on liiga läbipaistev — soovitatakse tugevamat varju/tumedamat overlay'd, vältides samas liigseid kohandusi.
- Tooltip'id ei sulgu teise klõpsuga (bug) — edastada TEDI arendusele ekraanisalvestusega.
- Topeltborder aktiivsetel elementidel segab; soovitatakse üht esiletõstetud äärist ja hall taust.

## Arenduse seis ja koostöö
- Table Card on valmis ja ootab koodiülevaatust; eeldatavasti järgmisel nädalal arendusse.
- Vajadused ja tagasiside disainikanalisse ning GitHubi diskussioonidesse, et töid õigesti prioriseerida.

# Otsused
- Kolmanda taseme navigeerimine lisatakse külgmenüüsse — refaktooring võimaldab seda nüüd hõlpsamalt.
- Teemavahetuseks soovitatakse dropdown-lahendust.
- Pop-overi tausta ja tooltip'i probleemid edastatakse arendusele (GitHubi diskussioon + ekraanisalvestus).

## Eelmine koosolek
- Jagada metsaregistri info ja vajadused disainikanalisse. (Kärolin)
- Koguda projektide tagasisidet ja vajadusi GitHubi diskussioonidesse (kaardirakenduse komponendid). (Kärolin)
- Lisada pop-overi taustale tumedama kihi/varju võimalus ja avada GitHubi diskussioon. (Kärolin)
- Visualiseerida ja korraldada 3. taseme navigeerimise erisused ning jagada meeskonnaga. (Kärolin)
- Teha Table Card arendusjäägid selgeks ja anda märku valmimisest. (Kärolin)
- Korraldada disainisüsteemi korrastamine: eristada baaskomponendid ja projektispetsiifilised näidised. (Kärolin)
- Jälgida ja vastata GitHubi diskussioonidele regulaarselt. (Kärolin)

**Projektide disainerid**
- Saata Kärolinile TEDI komponente kasutavate projektide lingid. (eelmisest)
- Stiilida väliste tekstiredaktorite teegid TEDI disainikeele järgi. (eelmisest)
- TTJA NBA ja Rahvastikuregistri menetluskeskkond: eristada külastatud ja külastamata olekuid. (eelmisest)
- AKS: Card header ja card vertical konflikt; brand-värvi peal pole searchi hint näha. (eelmisest)

**Arendusmeeskond**
- Rakendada ja testida uusi komponente (inline edit, tekstigrupi slot, sisukorra komponendi uued elemendid). (eelmisest)
- Teha radionuppude ja checkboxide muudatused ning eemaldada Choice Group. (eelmisest)
