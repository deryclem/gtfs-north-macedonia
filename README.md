# gtfs-north-macedonia

[![GTFS Validator](https://img.shields.io/badge/MobilityData%20Validator-0%20errors-brightgreen)](https://github.com/MobilityData/gtfs-validator)
[![Timetable Validity](https://img.shields.io/badge/Timetable-01.09.2026%20--%2012.12.2026-blue)](https://mzi.mk)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

Official [GTFS](https://gtfs.org) schedule feed for **MŽT** (Македонски Железници Транспорт АД Скопје), North Macedonia's national railway operator.

This feed also feeds into [Panto](https://getpanto.app), a real-time train tracking app currently in beta.

📦 **[Download latest GTFS package (`gtfs-north-macedonia.zip`)](./gtfs-north-macedonia.zip)**

---

## 🚆 Network & Active Services

**Validity**: 1 September 2026 - 12 December 2026 · **5 routes** · **34 trains/day** · **103 stops**

| Route | Cyrillic | Train Numbers | Frequency |
|---|---|---|---|
| **Skopje ↔ Kumanovo** | Скопје ↔ Куманово | 2020, 2021, 2022, 2023 | Mon-Sat (2 round trips) |
| **Skopje ↔ Veles** | Скопје ↔ Велес | 600, 601, 2080, 2083 | Daily (600/2083), Mon-Sat (others) |
| **Skopje ↔ Gevgelija** | Скопје ↔ Гевгелија | 611, 630, 631, 632 | Daily (2 round trips) |
| **Skopje ↔ Bitola / Žabeni** | Скопје ↔ Битола / Жабени | 640, 641, 642, 643, 644, 645 | Daily (3 round trips, train 642 fully restored) |
| **Skopje ↔ Zelenikovo (Gradski Voz)** | Скопје ↔ Зелениково (Градски воз) | 3080-3089, 3180-3185 | Daily (8 round trips / 16 trains) |

> **Suspended services (not included in feed):**
> - Skopje ↔ Kičevo (trains 660, 661): suspended by operator.
> - Veles ↔ Kočani (train 651): suspended by operator.
> - Trains 2081/2082: replaced by the *Gradski Voz* commuter rail schedules.

---

## 📦 GTFS Features & Specifications

This feed includes 13 GTFS files built according to MobilityData best practices:

- **Geographic Shapes (`shapes.txt`)**: 12 high-precision railway alignments (16,804 GPS points) mapped along physical tracks via OpenStreetMap, with cumulative distance (`shape_dist_traveled`).
- **Station Coordinates (`stops.txt`)**: All 103 passenger stops aligned to physical railway track geometries.
- **UIC Station Codes**: 39 official 7-digit UIC station codes populated from UIC DIUM 65 (e.g. `6500001` for Skopje Central).
- **Fares (`fare_attributes.txt`, `fare_rules.txt`)**: Official flat fares configured for *Gradski Voz* suburban lines (40 MKD one-way / 70 MKD round-trip).
- **Transfers (`transfers.txt`)**: Minimum interchange connection times defined at Skopje Central, Veles, and Zelenikovo.
- **Multilingual (`translations.txt`)**: Full Macedonian (Cyrillic) and English translations for stops, routes, and agency metadata.
- **Quality Assurance**: Validated with [MobilityData GTFS Validator v8.0.1](https://github.com/MobilityData/gtfs-validator) (0 errors).

---

## 📚 Sources & Attribution

- **Timetables & Operations**: [MŽI (Makedonski Železnici Infrastruktura)](https://mzi.mk) & [MŽT (Železnici na RM Transport)](https://mzt.mk)
- **Station Codes**: UIC DIUM 65 & MŽI Railway Network Statement
- **Track Alignments & Coordinates**: [OpenStreetMap](https://www.openstreetmap.org) contributors (ODbL)
- **Cross-verification**: [EGTRE (European Golden Temple of Rail Enthusiasts)](https://www.egtre.info/wiki/North_Macedonia_-_General_Information)

---

## 📄 License

- GTFS Feed Data: [Creative Commons Zero (CC0 1.0 Universal)](https://creativecommons.org/publicdomain/zero/1.0/)
- Rail Geometry & Base Map Data: [OpenStreetMap contributors](https://www.openstreetmap.org/copyright), licensed under [ODbL](https://opendatacommons.org/licenses/odbl/)
