# Pre-release Checklist – Kötelező minden kiadás előtt

**Használat:** A Cursor / AI minden generálás előtt végigmegy ezen a listán.  
**Eredmény:** PASS / FAIL listát ad vissza. FAIL esetén nem generál végső kimenetet.

---

## Checklist

### Általános (MASTER)
- [ ] 1. Előrejelzési idő megfelelő? (≥8 hét nagyobb, ≥4 hét kisebb)
- [ ] 2. Összevonás megvizsgálva?
- [ ] 3. Konfliktus (OneSAP, Blackweek, full-load, backlog…) detektálva?
- [ ] 4. Stakeholder sorrend helyes?
- [ ] 5. Dátum / adat konzisztens?
- [ ] 6. Kapacitás / fedezet rendben?
- [ ] 7. Belső egyeztetés (heti meeting) megtörtént?
- [ ] 8. Történeti adatok figyelembe véve?
- [ ] 9. Felelős review (Balogh János vagy modul-felelős) megtörtént / kérve?
- [ ] 10. Tanulási loop előkészítve?

### Modul-specifikus
- [ ] Műszerészek esetén: Balogh János review kérve
- [ ] OP MNT PM esetén: FIGYELMEZTETÉS – csak pilot, éles kiadás tilos
- [ ] Kommunikáció esetén: sablon + escalation path ellenőrizve

### Eredmény
- Ha minden [x] → PASS → generálható
- Ha bármelyik [ ] → FAIL → sorold fel a hiányzókat és állj meg
