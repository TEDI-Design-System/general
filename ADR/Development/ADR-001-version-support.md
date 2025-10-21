# ADR-001: Reacti ja Angulari versioonitoe poliitika

- **Staatus:** Accepted  
- **Kuupäev:** 2025-04-23  
- **ADR ID:** ADR-001  
- **Otsuse tegijad:** Tõnis Tobre, Oliver Vaga  

---

## 1. Kontekst

TEDI (TEHIKu disainisüsteem) tugineb uusimatele Reacti ja Angulari versioonidele.  
Kõik tarbijarakendused (infosüsteemid, portaalid, teenused), mis TEDI teeke kasutavad, ei saa aga minna koheselt üle kõige uuemale versioonile.  
Põhjused võivad olla:
- Tehnoloogiline võlg  
- Teiste raamistike või komponentide sõltuvused  
- Ressursi- või ajapiirangud

---

## 2. Otsus

TEDI hakkab toetama **kuni ühte major-versiooni vanemaid Reacti ja Angulari versioone** paralleelselt uusimatega.

Vanema versiooni puhul:
- Tehakse ainult hädavajalikke parandusi (bugfixid, hotfixid, ligipääsetavuse parandused)  
- Ei lisata uusi funktsioone ega komponente  
- Dokumentatsioonis eristatakse selgelt, millised muudatused kehtivad ainult uusima versiooni kohta

---

## 3. Tagajärjed

**Positiivsed:**
- Vanemate versioonide kasutajad saavad vajalikud parandused ilma kohustusliku uuendamiseta  
- Selge signaal, et süsteemid peaksid planeerima ressursse sõltuvuste regulaarselt uuendamiseks  
- Leevendab migratsiooniriski riiklikel infosüsteemidel

**Negatiivsed:**
- TEDI arendustiimi töökoormus kasvab versioonide paralleelse hoolduse tõttu  
- Vaja on automatiseeritud CI/CD protsessi, et parandused jõuaks ka vanemasse versiooni  
- Changelogi ja semver’i haldus muutub kriitiliselt oluliseks

---

## 4. Alternatiivid


---

## 5. Järeldus



---

## 6. Seotud dokumendid / Tulevikutöö

