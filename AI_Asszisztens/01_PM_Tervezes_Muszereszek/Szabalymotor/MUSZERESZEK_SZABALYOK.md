# Műszerészek PM-tervezés – Modul-specifikus szabályok

**Státusz:** ÉLES  
**Felelős review:** Balogh János (kötelező minden kiadás előtt)  
**Egyeztetve:** [ide írd be a dátumot amikor Balogh Jánossal véglegesítve]

Ez a fájl a MASTER_SZABALYRENDSZER kiegészítése. A 10 általános szabály + az alábbiak együtt futnak.

---

## Extra szabályok (műszerészek)

| # | Szabály | Leírás |
|---|---------|--------|
| M1 | Csak műszerész hatáskör | Csak a műszerészekre vonatkozó PM-tervek generálhatók és adhatók ki élesen. |
| M2 | Balogh János kötelező review | Nincs kivétel. Minden tervet ő néz át mielőtt élőbe megy. |
| M3 | Történeti MNT adatok | A rendszer mindig húzza be az előző 12 hónap műszerész-MNT-jeit. |
| M4 | Gép / eszköz prioritás | Kritikus eszközök prioritása magasabb, de soha nem írhatja felül a MASTER 1-3. szabályát. |

---

## Cursor utasítás
Mielőtt műszerész PM-tervet generálsz:
1. MASTER_SZABALYRENDSZER
2. Ez a fájl
3. Pre_release_checklist
4. Ha minden PASS → generálás + Balogh review kérés
