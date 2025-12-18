# Munich Airport Delay Intelligence Dashboard ✈️

Dieses Projekt analysiert Verspätungen am Flughafen München (EDDM), indem **Flugplan-, Airline- und Wetterdaten** zusammengeführt werden. Ziel ist es, **Pünktlichkeitsmuster, saisonale Cluster und wetterbedingte Effekte** sichtbar zu machen und über ein Tableau-Dashboard interaktiv auszuwerten.

## Projektziele

- Mit **Python, Pandas und SQL** Flugplan-, Airline- und Wetterdaten zusammenführen, bereinigen und modellieren, um Verspätungen und saisonale Muster zu analysieren.
- Mit **statistischen Methoden** und **KPI-Definitionen** (z. B. Pünktlichkeitsquote, durchschnittliche Verspätung, Ausfallrate) zentrale Leistungskennzahlen identifizieren und aufbereiten.
- In **Tableau** ein interaktives Dashboard mit Heatmaps, Trendlinien und Filtern erstellen, um Airline-Abweichungen und saisonale Verspätungscluster sichtbar darzustellen.

## Datenquellen

- `data/raw/flights_bavaria_2025.csv`  
  Fluglevel-Daten für Bayern (inkl. EDDM), Basis für Verspätungsanalyse.

- `data/raw/airport_traffic_2024.csv`, `data/raw/airport_traffic_2025.csv`  
  Tägliche An- und Abflüge pro Flughafen (Eurocontrol Airport Traffic).

- `data/raw/10866_2024.csv`, `data/raw/10866_2025.csv`  
  Stündliche Wetterdaten (Temperatur, Wind, Niederschlag etc.) für Station 10866 (Raum München).

- `data/raw/Stakeholder_Punctuality.xlsx`  
  Offizielle Pünktlichkeits-KPIs pro Flughafen (Ankunft/Abflug, YTD).

- `data/raw/runways.csv`  
  Runway-Charakteristika (Länge, Oberfläche, Beleuchtung) inkl. EDDM.

- `data/raw/airports.csv`  
  Stammdaten zu Flughäfen (Name, ICAO-Code, Land etc.).

munich-airport-delay-intelligence/
├─ README.md
├─ .gitignore
├─ requirements.txt              # optional, later for packages
├─ notebooks/
│  └─ 01_muc_delay_analysis.ipynb
├─ src/
│  ├─ __init__.py
│  ├─ data_prep.py              # functions for loading/cleaning data
│  ├─ kpi_calculation.py        # functions for KPIs
│  └─ utils.py                  # helpers if needed
├─ data/
│  ├─ raw/
│  │  ├─ flights_bavaria_2025.csv
│  │  ├─ airports.csv
│  │  ├─ airport_traffic_2024.csv
│  │  ├─ airport_traffic_2025.csv
│  │  ├─ 10866_2024.csv
│  │  ├─ 10866_2025.csv
│  │  ├─ runways.csv
│  │  └─ Stakeholder_Punctuality.xlsx
│  └─ processed/
│     ├─ flights_muc_weather.csv        # (we will create later)
│     ├─ daily_kpi_muc.csv              # (we will create later)
│     ├─ seasonal_matrix_muc.csv        # (for heatmaps)
│     └─ airline_kpi_muc.csv
├─ sql/
│  └─ kpi_queries.sql            # SQL snippets we’ll write later
├─ tableau/
│  └─ muc_delay_dashboard.twbx   # your Tableau workbook
└─ reports/
   └─ findings_muc_delay.md      # optional summary / notes
