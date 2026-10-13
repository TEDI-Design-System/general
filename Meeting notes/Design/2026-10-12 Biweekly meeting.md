*Tegu on AI kokkuvõttega*

# Peamised punktid

## Komponentide uuendused ja ühtlustamine
- Sheet-komponent: ühtne mobiili- ja desktopilahendus eri päiste/jalustega ja breakpoint-käitumisega; Reacti versioon peagi valmis, Angular varsti järel. Projekt valib ise sheet'i või popover'i vahel.
- Disabled-staatus ühtlustati nuppudel ja vormiväljadel (ühtsed värvid ja läbipaistvus); projektid võivad erandeid teha, kuid TEDI soovitab hoida ühtsust ja sellest teada anda.
- Checkbox-komponendile lisandusid uued olekud (selected hover, active, focus, disabled) — toetab arendust ja prototüüpimist; muutujate arv kasvas, nii et projektid peavad kohandused üle vaatama.

## Projektipõhised kohandused ja muutujad
- TEDI muutujad on avalikud: projektid saavad Figmas muuta baasfonti, värve, mõõtmeid ja paddingut (nt kompaktsem tabel) — alati WCAG nõuete piires.
- Tabeliteksti suuruseks on eraldi muutuja (muudetav üle projekti); eraldi saab muuta ka komponendispetsiifilisi värve (nt ikoonivärvid).
- Muutujate muudatused kanduvad disainist arendusse ja on jälgitavad; muudatustest tuleb TEDI tiimi teavitada.

## Figma protsessid ja dokumentatsioon
- Kuvamisvead lahenevad prototüübis "regenerate all instances" nupuga; vigadest teatada TEDI tiimile.
- Plaanis on Figma struktuuri ümberkorraldus: põhiversioon ja suurused ettepoole, light/dark kõrvuti, suuremad flow'd eraldi lehtedele.
- Komponentidele lisatakse dokumentatsiooni- ja arenduslingid (töö käib, kõik pole veel kaetud).

## Sisukord ja mobiilivaade
- Pikematel lehtedel vajab sisukorra scrollimis-/sticky-käitumine veel selgitamist; oodatakse projektide tagasisidet.

## Koostöö ja suhtlus
- Projektidel on vabadus valida komponente ja käitumist, kuid muudatustest ja erivajadustest tuleks TEDI tiimiga suhelda (nt millal sheet, millal popover).
- Sheet ja seda avav nupp on eraldi komponendid — nende sidumine on projekti vastutus.
- Küsimused ja probleemid Designi kanalisse.

# Otsused
- Disabled-staatus ühtlustatakse nuppudel, vormiväljadel ja checkbox-komponendil; soovituslik on hoida ühtsust.
- Projektipõhised kohandused (värvid, padding, tekstisuurus) on lubatud, kui järgitakse ligipääsetavuse (WCAG) nõudeid.
- Figma struktuur korraldatakse ümber parema leitavuse nimel.

## Eelmine koosolek
**Projektide disainerid**
- Figma komponentide nihkumisel kasutada "regenerate all instances" ja teatada TEDI tiimile.
- Anda tagasisidet Figma komponendi struktuuri muutmise kohta.
- TTJA NBA ja Rahvastikuregistri menetluskeskkond: eristada külastatud ja külastamata olekuid. (eelmisest)
- AKS: Card header ja card vertical konflikt; brand-värvi peal pole searchi hint näha. (eelmisest)

**Arendusmeeskond ja TEDI tiim**
- Kontrollida ja uuendada komponentide dokumentatsioon ning arenduslingid Figma failides.
- Lisada pop-overi taustale tumedama kihi/varju võimalus ja avada GitHubi diskussioon. (eelmisest)
