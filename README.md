# gtfs-north-macedonia

[GTFS](https://gtfs.org) feed for **MŽT** (Македонски Железници Транспорт АД Скопје), North Macedonia's national railway operator.

Timetable: **14 Dec 2025 – 12 Dec 2026** · 4 routes · 20 trains · 103 stops

## Download

[gtfs-north-macedonia.zip](./gtfs-north-macedonia.zip)

## Trains

| # | Route | Days |
|---|-------|------|
| 2020, 2021, 2022, 2023 | Скопје ↔ Куманово | Mon–Sat |
| 600, 601, 2080, 2081, 2082, 2083 | Скопје ↔ Велес | 600/2083 daily; rest Mon–Sat |
| 611, 630, 631, 632 | Скопје ↔ Гевгелија | Daily |
| 640, 641, 642, 643, 644, 645 | Скопје ↔ Битола / Жабени | Daily |

Train 642 is suspended between Велес and Скопје from 02.01.2026.  
Скопје–Кичево (660/661) and Велес–Кочани (651) are not in the 2025/26 timetable and not included.

## Sources

- [MŽI timetable documents](https://mzi.mk/%d0%b2%d0%be%d0%b7%d0%b5%d0%bd-%d1%80%d0%b5%d0%b4/) — wall timetable, working booklet, amendment 02.01.2026
- [MŽI Railway Network Statement 2026](https://mzi.mk/en/access-to-infrastructure/) — station codes
- [MŽT operator website](https://mzt.mk) — timetable verification
- [OpenStreetMap](https://www.openstreetmap.org) — station coordinates (ODbL)
- [EGTRE North Macedonia](https://www.egtre.info/wiki/North_Macedonia_-_General_Information) — independent timetable verification

## Notes

- Only Скопје has a confirmed UIC passenger code (`6500001`).
- 3 station coordinates are linearly interpolated: Мартолци, Загорани, Сулари.
- Validated with [MobilityData GTFS Validator v4.2.0](https://github.com/MobilityData/gtfs-validator) — 0 errors.

## License

Feed: [CC0](https://creativecommons.org/publicdomain/zero/1.0/) · Coordinates: © OpenStreetMap contributors, [ODbL](https://opendatacommons.org/licenses/odbl/)
