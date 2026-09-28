# AI Asszisztens – Státusz

**Utolsó frissítés:** 2026-09-28

## Röviden
A szabálymotor és a Cursor-utasítás megvan; a teljes `AI_Asszisztens/` fa a GitHub AIAssistant repóban van.

## Státuszok

| Modul                        | Státusz     | Review felelős   |
|-----------------------------|-------------|------------------|
| 01_PM_Tervezes_Muszereszek  | **ÉLES**    | Balogh János     |
| 02_PM_Tervezes_OP_MNT_PM    | **PILOT**   | Rimóci Attila    |
| MASTER + Validáció          | **ÉLES**    | Projektgazdák    |

## Nem kód — emberi teendők

1. **Roland-válasz kiküldése**
2. **Balogh Jánossal** a műszerész-szabályok véglegesítése
3. **Pilot finomhangolás** (Rimóci / Roland)

## Cursor működése
Minden generálás előtt: `.cursorrules` + CURSOR_UTASITAS → MASTER → modul-szabályok → Pre-release checklist → PASS/FAIL.
