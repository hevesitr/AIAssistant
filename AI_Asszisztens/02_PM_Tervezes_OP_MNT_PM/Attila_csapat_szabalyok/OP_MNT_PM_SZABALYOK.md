# OP MNT PM (Rimóci Attila csapat) – Modul-specifikus szabályok

**Státusz:** CSAK LEHETŐSÉG / PILOT – NEM ÉLES  
**Felelős:** Rimóci Attila + későbbi egyeztetés  
**Fontos:** Jelenleg TILOS éles tervet kiadni ebből a modulból.

---

## Extra szabályok

| # | Szabály | Leírás |
|---|---------|--------|
| A1 | Pilot only | Semmilyen terv nem mehet ki éles kommunikációban. Csak belső teszt / lehetőség. |
| A2 | Vendor vs Production | Vendor szabadidő SOHA nem lehet elsődleges. Először production / OPC kényszerek. |
| A3 | Összevonás kötelező | Féléves + éves + egyéb nagyobb MNT-k max. 1-2 sormegállítás/év elv. |
| A4 | OneSAP / kritikus időszak | Automatikus blokkolás ha OneSAP, Blackweek, major átállás vagy backlog-recovery van. Részletek: `Konfliktus_detektor/KRITIKUS_IDOSZAKOK.md` |
| A5 | Heti egyeztetés | Minden nagyobb tervnek meg kell jelennie a heti MNT meetingen mielőtt kiküldésre kerül. |

---

## Cursor utasítás
Ha valaki OP MNT PM tervet kér:
1. Figyelmeztesd: „Ez a modul jelenleg csak PILOT. Éles kiadás tilos.”
2. Futtasd a MASTER + ezeket a szabályokat.
3. Generálj csak belső, nem kiküldhető draftot.
4. Javasold a tolást / összevonást ha konfliktus van.
