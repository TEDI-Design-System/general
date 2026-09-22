# Peamised punktid

## Komponentide uuendused
- Sisukorra komponendile lisandusid slot, ikoonitugi, separaator ja border bottom — parem loetavus ja kohandatavus.
- Inline edit (endine hidden field) aktiveerub hoveriga ja ikoon näitab muudetavust; koodireview on lõppfaasis, peagi arendusse.
- Tekstigrupi komponendile lisati lõppu slot (nupud/ikoonid); ikoonivärvid viidi WCAG nõuetega vastavusse ning label ja description on nüüd fill'i peal, et vältida teksti ülekatet.
- Uus Timeline komponent töötab nii Reactis kui Angularis (kasutuses nt terviseportaalis) — sobib sündmuste ja tegevuste logi kuvamiseks.

## Tekstiredaktor ja juhendid
- Tekstiredaktorit TEDI alla ei arendata — projektid võtavad välise teegi ja stiilivad selle TEDI järgi; kaasneb juhend.
- Cloud Designile valmis juhend TEDI põhjal oma disainisüsteemi loomiseks (Cloud Design kasutab eraldi varianti, mitte TEDI-t otse); tiimi tagasiside on oodatud.

## Peakasutajate roll
- Peakasutaja on asutuses kontaktisik ja teemaekspert — ei pea kõike teadma, vaid suunab küsimusi ja on põhiteemadega kursis.
- Suurtes asutustes on peakasutajad enamasti olemas, kuid ametlik kinnitamine puudub.
- Peakasutajad aitavad levitada TEDI release-uudiseid ja muudatusi oma asutuses.

## Kommunikatsioon ja kanalid
- Disainiküsimused suunatakse disainikanalisse, arendusküsimused arenduskanalisse — selgem vastutus ja kiirem lahendamine.
- Küsimusi ja tagasisidet oodatakse Slackis; avatud suhtlus toetab süsteemi pidevat parendamist.

# Otsused
- Tekstiredaktori komponenti TEDI alla ei lisata — kasutatakse väliseid teeke koos TEDI stiilijuhistega (projektipõhine).
- Disaini- ja arendusküsimused suunatakse vastavatesse kanalitesse; peakasutajad suunavad küsimusi, ei vastuta kõigi detailide eest.

## Eelmine koosolek
- Jagada Cloud Designi juhendi link Slackis huvilistele. (Kärolin)
- Korraldada peakasutajate määramist ja teavitada TEDI-teemalistest uuendustest. (Kärolin)
- Vastata TEDI disainisüsteemi küsimustele või suunata need edasi. (Kärolin)

**Projektide disainerid**
- Testida Cloud Designi juhendit ja anda tagasisidet.
- Stiilida väliste tekstiredaktorite teegid TEDI disainikeele järgi.
- Kasutada uut Timeline komponenti vastavalt vajadusele.
- Saata Kärolinile TEDI komponente kasutavate projektide lingid. (eelmisest)
- Map komponendis külgpaneeli parem sulgemise/avamise lahendus. (eelmisest)
- TTJA NBA ja Rahvastikuregistri menetluskeskkond: eristada külastatud ja külastamata olekuid. (eelmisest)
- AKS: Card header ja card vertical konflikt; brand-värvi peal pole searchi hint näha. (eelmisest)

**Arendusmeeskond**
- Rakendada ja testida uusi komponente (inline edit, tekstigrupi slot, sisukorra komponendi uued elemendid).
- Viia lõpuni külgmenüü refaktooring ja 3. taseme lihtsustamine. (eelmisest)
- Jätkata rating komponendi arendamist. (eelmisest)
- Teha radionuppude ja checkboxide muudatused ning eemaldada Choice Group. (eelmisest)
