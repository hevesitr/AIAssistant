# Kritikus időszakok – Konfliktus detektor

**Frissítve:** 2026-09-24  
**Forrás:** Vincze Emese email + Ribesam eset

## Aktív / ismert kritikus időszakok

| Időszak | Típus | Hatás | Forrás |
|---------|-------|-------|--------|
| **2026. szept. vége – okt. eleje (Blackweek + megelőző napok)** | SAP P03 nélküli időszak / OneSAP átállás | Alkatrészellátás manuális, „vakon” időszak, 18:00 után csak indokolt kiadás | Vincze Emese 2026-09-23 |
| OneSAP / major SAP átállás hetek | Rendszerátállás | Termelés feszült, backlog-recovery, extra megállás kerülendő | Sebestyén Attila / Roland Pater (Ribesam) |
| Full-load + backlog-recovery | Production prioritás | Decommit fedezet hiány, extra MNT kerülendő | OPC visszajelzések |

## Szabály (A4 + MASTER 3)
Ha egy tervezett MNT vagy nagyobb tevékenység a fenti időszakokba esik:
→ **Figyelmeztetés / blokkolás** + alternatív slot javaslat kötelező.
→ Vendor-szabadidő nem írhatja felül.

## iShare / helyi másolat (Blackweek alkatrészek)
- iShare: https://ishare.infineon.com/sites/hianyzo-PIO-SpareParts/SitePages/Home.aspx
- Helyi: `X:\Németh - Hevesi\Blackweek - MNT- CEG`
- Fájlok: Folyamatban_anyagszámok, PIO_anyagszámok, Alkatrész igénylés MNT.xlsx
