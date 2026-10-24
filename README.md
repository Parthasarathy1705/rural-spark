# Rural Spark

A community-owned solar mini-grid for a Chenchu (PVTG) hamlet in Amrabad, Nagarkurnool, Telangana.
Schneider Electric Go Green 2026, Phase 2 business case.

Team: Parthasarathy P, Tanush Pavan Vakalaggada (Amrita Vishwa Vidyapeetham).

**Results and evidence:** https://parthasarathy1705.github.io/rural-spark/

- `index.html` with the `.gif` and `.png` files: the results website (animated outputs, tables, sources).
- `.csv` files: the data behind every chart in the deck.
- `Rural_Spark_models.zip`: all model code, inputs and results
  - `model/simulation_b1/`: 5/15-minute controller simulation (Python) with the MATLAB battery pack model and Simulink file (`matlab/RuralSpark_BatteryPack.slx`; run `matlab/RUN_ME.m`)
  - `model/dispatch_16yr/`: 16-year hourly dispatch model (JavaScript) on PVGIS-ERA5 weather
  - `model/finance/`: 15-year cash-flow and renewal-reserve model (Python)

Design: 18.36 kWp PV (34 × 540 Wp), 15 kW three-phase grid-forming inverter, 40.96 kWh LFP battery, 30 metered connections.

All performance figures are simulated on satellite-derived weather (PVGIS, EC JRC). Loads are assumed schedules until a metered baseline is collected. No funding is sanctioned and no tariff is agreed; both are modelled as assumptions.
