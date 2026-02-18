# 2026-02-02 Regulaarne disainikoosolek

## Osalejad
- Liis Ots
- Einar Arro
- Kaisa Reimal
- Daisy Pukkonen
- Saskia Sonnberg
- Maris Jool
- Karis Karindi
- Kristel Ojamaa
- Piret Tabor
- Lauri Tõnisson
- Marju Sild
- Helis Lembe
- Siret Tuula
- Helis Sepp

https://bitwebou-my.sharepoint.com/personal/karolin_kivisikk_bitweb_ee/_layouts/15/stream.aspx?id=%2Fpersonal%2Fkarolin%5Fkivisikk%5Fbitweb%5Fee%2FDocuments%2FRecordings%2FDisaineritele%20TEDI%20komponendid%2D20260202%5F160059%2DMeeting%20Recording%2Emp4&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E1c899324%2D72db%2D4edb%2Da86a%2D4ae22a814744&isDarkMode=false

## Päevakord
* Demo: release notes, resizeri demo

# TEDI poolt info
* Release demo:
  * Checkboxi ja RadioButtoni komponendid uuendati – eemaldati vanad variandid (sh ilma ikoonita versioonid) ning kaotati võimalus checkboxi välja lülitada. Lisati uus filterikomponent, mis asendab varasemaid lahendusi ning toetab nii ühe- kui mitmevalikulist kasutust (veel mitte avalik). Samal ajal tagati tagurpidi ühilduvus olemasolevate projektidega.
  * Focus state kujundati ümber (valge rõngas), et see sobiks paremini sinise tausta ja inverteeritud nuppudega. Vormiväljade error- ja hint-tekstide käsitlus ühtlustati. Accordioni lahendus viidi kokku collapse-komponendiga, et vältida dubleerimist.
  * Top headeri komponent sai mitmeid täiustusi: lisandus keelevaliku dropdown ning mobiilis fullscreen-otsing. Otsingu suurust saab nüüd Figma-s muuta ilma kogu headerit eemaldamata. Komponendid koondati ja korrastati, et vältida erandeid ning hoida süsteem ühtsem.
  * Migratsioon toimub järk-järgult. Vanad komponendid märgitakse ja kustutatakse TEDI communityst plaanipäraselt, et uued projektid kasutaksid ainult uuendatud elemente. Migratsioonitabel aitab jälgida asendusi ja kustutamisi ning vältida projektide katkemist.
* Alustatakse TEDI kasutatavuse tagasiside kogumisega intervjuude kaudu, kaasates nii hiljuti liitunud kui ka varasema kogemusega disainereid. Intervjuud viiakse läbi koostöös Melioradiga ning nende eesmärk on koguda sisendit edasisteks arendusteks.

# Küsimused disaineritelt
**Küsimus: Vanglasüsteem vajab chati/sünumite vahetamise funktsionaalsus, kas ja kuidas TEDI komponentidega seda ehitada?**
Vastus: Vaadatakse üle, kas olemasolevad TEDI komponendid katavad vajalikud funktsionaalsused. Luua Discussioni postitus, kogume teistest prototüüpidest kokku vajadused.

**Küsimus: Millal ja kas lisandub Vue raamistik TEDI-sse?**
Vastus: Vue raamistiku lisamine on arutelus arenduses.

**Küsimus: Kas külgmenüü mobiilivaates saab käituda overlay-tüüpi lahendusena, et see ei lükkaks sisu kõrvale?**
Vastus: TEDi mobiili külgmenüü on juba overlay'na. 

**Küsimus: AKS projekt ootab Reacti headerit, millal tuleb? Märtsis neil on live.**
Vastus: Algatada discussion, sõltub selle komponendi huvist. 

**Küsimus: AKS soovib editori enda projekti**
Vastus: Algatada discussion.

## Otsused
* Koguda projektidest chati/sõnumi disainid kokku üle projektide.

Eelmistest koosolekutest veel üleval:
* Arenduse Headeri arenduses arvestada vajadust logo sisse-välja lülitada (mobiilis teemaks ruumipuuduse tõttu) - sama ka figmas
* Figma make ja TEDI kooslus vajab veel testimist, testitud varasemas etapis võimalik et Make on arenenud. 
* Sidenavile lisada jalus ja päis
* Map componentsis külgpaneeli parem sulgemise/avamise lahendus
* Vertical stepperi alamsammude kuvamine mobiilis
* Välisveebi komponentide vajaduste ja näidete kogumine
* TTJA NBA, Rahvastikuregustri menetluskeskkond: vajadus tabelis/lingil eristada mida on külastatud mida mitte.
* Aadresside ja Kohanimede Süsteem (AKS): Card header ja card vertical tekitavad disainis mingi konflikti kui headeris kõik väärtused sisselülitada, brand värvi peal pole searchi hinti näha
