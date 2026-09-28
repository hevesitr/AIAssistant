# MASTER SZABÁLYRENDSZER – Minden kiadás előtt kötelező

**Verzió:** 1.0  
**Dátum:** 2026-09-24  
**Státusz:** ÉLES – minden modulra érvényes  
**Cursor / AI utasítás:** Ezt a fájlt MINDIG olvasd be mielőtt bármilyen tervet, adatot, választ vagy dokumentumot generálsz / kiadsz. Ha bármelyik szabály FAIL → NE generáld a végső kimenetet, hanem jelezd a hibát.

---

## Alapelv
Bármikor, amikor:
- előre tervezünk (PM, karbantartás, ütemezés, stb.)
- adatot / tervet / információt adunk ki emberek felé (email, report, dashboard, üzenet)

… akkor **kötelező** a pre-release ellenőrzés.

---

## 10 kötelező szabály (minden modulra)

| # | Szabály | Ellenőrzés | FAIL esetén |
|---|---------|------------|-------------|
| 1 | **Minimum előrejelzési idő** | Nagyobb esemény (≥1 nap vagy external) ≥ 8 hét; kisebb ≥ 4 hét | Blokkolás + indoklás kérése |
| 2 | **Összevonás / optimalizálás** | Ugyanazon erőforrás / gépcsoport eseményei max. indokolt számú megállást okozzanak | Összevonási javaslat kötelező |
| 3 | **Konfliktus-detektálás** | Ismert kritikus időszakok (OneSAP, Blackweek, major ramp, backlog-recovery, full-load, stb.) | Figyelmeztetés + alternatív slot javaslat |
| 4 | **Stakeholder sorrend** | Az érintett területek (OPC, Production, stb.) előbb vagy párhuzamosan értesüljenek, mint a külső partner | Nem mehet ki csak vendor/external felé |
| 5 | **Dátum- és adat-konzisztencia** | Nincs elírás, átfedés, ellentmondás a dátumokban / adatokban | Blokkolás |
| 6 | **Kapacitás / fedezet** | Van-e erőforrás, decommit-terv vagy jóváhagyás | Érintett terület jóváhagyása kell |
| 7 | **Belső egyeztetés** | Nagyobb esemény szerepelt-e a releváns heti / rendszeres meetingen | Figyelmeztetés |
| 8 | **Történeti adat** | Előző 12 hónap hasonló eseményei figyelembe véve | Összevonási / tanulási javaslat |
| 9 | **Felelős review** | Az adott modul felelőse (pl. Balogh János) review-ja megtörtént | Kötelező checkpoint |
| 10 | **Tanulási loop** | Kiadás után retrospektív (feedback gyűjtés) | Szabály frissítés kötelező |

---

## Cursor / AI végrehajtási szabály

```
MIELŐTT BÁRMIT KIADSZ:
1. Olvasd be ezt a MASTER fájlt.
2. Olvasd be a modul-specifikus szabályfájlt.
3. Futtasd le mind a 10 szabályt + a modul-specifikusakat.
4. Ha BÁRMELYIK FAIL → ne generáld a végső kimenetet.
   Helyette: sorold fel a FAIL-eket és kérj javítást / döntést.
5. Csak ha minden PASS → generáld a kimenetet.
6. Minden kiadás után írd be a Kiadasi_log-ba és a Tanulasi_loop-ba.
```

---

## Frissítési szabály
- Bármely szabály változásakor egyeztetni kell az érintett stakeholderrel.
- Változás után a verziószámot növelni kell, és a Dontesi_naplo-ba beírni.
