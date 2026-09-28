# AI Asszisztens – Architektúra

**Utolsó frissítés:** 2026-09-24

## Cél
Minden előre tervezés és emberek felé történő adat-/tervkiadás kötelező szabályrendszeren + pre-release ellenőrzésen + tanulság dokumentumon megy keresztül.

## Magas szintű felépítés

```
CURSOR_UTASITAS.md + .cursorrules     ← belépési pont, kötelező olvasás
        │
        ▼
06_Altalanos_szabalyrendszer/         ← MASTER 10 szabály (minden modulra)
        │
        ├── 01_PM_Tervezes_Muszereszek     (ÉLES)
        ├── 02_PM_Tervezes_OP_MNT_PM       (PILOT)
        ├── 03_Validacio_es_Review         (minőségkapu)
        ├── 04_Kommunikacio
        ├── 05_Tudastar
        └── 07_Egyeb_modulok               (jövőbeli + sablon)
```

## Adatáramlás (kiadás előtt)

1. Kérés érkezik
2. Cursor beolvassa CURSOR_UTASITAS + MASTER + modul-szabályok
3. Pre_release_checklist fut
4. PASS → generálás
5. Felelős review (ha kötelező, pl. Balogh János)
6. Éles kiadás + Kiadasi_log
7. 1–2 hét múlva Tanulasi_loop → esetleg szabályfrissítés

## Felelősségi mátrix

| Modul                        | Státusz     | Review felelős     |
|-----------------------------|-------------|--------------------|
| 01_PM_Tervezes_Muszereszek  | ÉLES        | Balogh János       |
| 02_PM_Tervezes_OP_MNT_PM    | PILOT       | Rimóci Attila      |
| MASTER szabályok            | ÉLES        | Projektgazdák      |
| Kommunikáció                | ÉLES        | Projektgazdák      |

## Új modul hozzáadása
Használd a `07_Egyeb_modulok/Sablon_uj_modul/` másolatát.
Mindig írd be a felelőst a Stakeholder_terkep-be és a Dontesi_naplo-ba.
