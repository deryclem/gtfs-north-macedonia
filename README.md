# gtfs-north-macedonia

[GTFS](https://gtfs.org) feed for **MŽT** (Македонски Железници Транспорт АД Скопје), North Macedonia's national railway operator.

Timetable: **1 Sep 2026 – 12 Dec 2026** (Updated with Gradski Voz & restored train 642) · 5 routes · 34 trains · 103 stops · Geographic Shapes (OSM) · Fares · 13 GTFS files

## Download

[gtfs-north-macedonia.zip](./gtfs-north-macedonia.zip)

## Trains

| # | Route | Days |
|---|-------|------|
| 2020, 2021, 2022, 2023 | Скопје ↔ Куманово | Mon–Sat |
| 600, 601, 2080, 2083 | Скопје ↔ Велес | 600/2083 daily; rest Mon–Sat |
| 611, 630, 631, 632 | Скопје ↔ Гевгелија | Daily |
| 640, 641, 642, 643, 644, 645 | Скопје ↔ Битола / Жабени | Daily |
| 3080, 3081, 3082, 3083, 3084, 3085, 3086, 3087, 3088, 3089, 3180, 3181, 3182, 3183, 3184, 3185 | Скопје ↔ Зелениково (Градски воз) | Daily (8 round trips) |

- **Градски воз (Gradski Voz)**: New suburban rail service inaugurated on 01.09.2026 between Skopje and Zelenikovo (16 trains/day).
- **Train 642**: Restored to full route from Жабени / Битола all the way to Скопје (arriving 16:15).
- **Trains 2081/2082**: Suspended since 07.08.2026 (replaced by the Gradski Voz schedules).
- Скопје–Кичево (660/661) and Велес–Кочани (651) remain suspended and not included.

## GTFS Structure & Best Practices (13 Files)

- **Fares (`fare_attributes.txt`, `fare_rules.txt`)**: Confirmed flat fares for the Gradski Voz suburban service (40 MKD one-way, 70 MKD return).
- **Geographic Shapes (`shapes.txt`)**: 12 route traces (16,804 coordinate points) routed along actual physical tracks from OpenStreetMap, with cumulative distance (`shape_dist_traveled`).
- **Station Transfers (`transfers.txt`)**: Timed transfers defined at key interchange stations (Skopje Central, Veles, Zelenikovo).
- **Operator Details (`agency.txt`)**: Enriched with official ticketing URL (`https://mzt.mk/prevozni-ceni-dodatoci-i-nadomestoci/`) and customer email (`kontakt@mzt.mk`).
- **Station UIC Codes (`stops.txt`)**: 39 official 7-digit UIC codes sourced from UIC DIUM 65 and confirmed international passenger registry (`6500001` for Skopje Central).
- **Translations (`translations.txt`)**: Full English translations for all 103 stations, routes, and operator name, conforming strictly to the official GTFS specification.
- **Track-snapped Coordinates**: Interpolated stations (Мартолци, Загорани, Сулари) snapped to the physical railway track adjacent to each village.
- **Validated**: Validated with [MobilityData GTFS Validator v4.2.0](https://github.com/MobilityData/gtfs-validator) — 0 errors.

## Sources

- [MŽI timetable documents](https://mzi.mk/%d0%b2%d0%be%d0%b7%d0%b5%d0%bd-%d1%80%d0%b5%d0%b4/) — Gradski Voz timetable, updated timetable excerpt 01.09.2026–12.12.2026, draft project 2026–2027
- [MŽI Railway Network Statement 2026](https://mzi.mk/en/access-to-infrastructure/) — station codes
- [MŽT operator website](https://mzt.mk) — timetable verification & fares
- [UIC DIUM 65](https://uic.org) — official UIC railway station codes (65)
- [OpenStreetMap](https://www.openstreetmap.org) — station coordinates and railway track alignments (ODbL)
- [EGTRE North Macedonia](https://www.egtre.info/wiki/North_Macedonia_-_General_Information) — independent timetable verification

## License

Feed: [CC0](https://creativecommons.org/publicdomain/zero/1.0/) · Coordinates & Rail Geometry: © OpenStreetMap contributors, [ODbL](https://opendatacommons.org/licenses/odbl/)
