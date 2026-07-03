# Workshop Energy Data Samples

This folder contains small CSV files for classroom exercises in the KSU undergraduate energy workshop. The files are deterministic, readable, and safe to use offline; they are reduced teaching samples, not authoritative historical records.

## Files

- `electricity-demand-sample.csv` uses the Korea Power Exchange supply/demand framing: current demand, maximum forecast demand, operating reserve, reserve rate, and temperature.
- `solar-weather-sample.csv` uses the Korea East-West Power Jeju solar forecast framing listed on Korea's public data portal: timestamp, location, weather variables, irradiance, installed capacity, and solar generation.
- `energy-use-sample.csv` uses the Korea Energy Agency/Korea Energy Statistical Information System energy-use statistics framing: sector, annual electricity, gas, heat, total energy, and an intensity index.

## Public-Source Framing

- Korea Power Exchange real-time power supply and demand: https://www.kpx.or.kr/eng/
- Korea East-West Power Jeju solar forecast file data on Korea's public data portal: https://www.data.go.kr/en/data/15143884/fileData.do
- Korea Energy Agency public energy-efficiency and demand-side-management role: https://www.energy.or.kr/en/main/main.do
- Korea Energy Statistical Information System consumption and survey statistics: https://kesis.keei.re.kr/eng

## Reduction and Sampling

- Rows were hand-reduced into workshop-sized examples so students can inspect them in a spreadsheet or with basic Python.
- Values are rounded to classroom-friendly units and ordered by time or year.
- No live download, API key, account, or network access is required.
- The samples preserve public-source column concepts and units while avoiding large official datasets that would slow the workshop.

## Units

- `timestamp`: ISO 8601 local Korea time.
- `current_demand_mw`, `max_forecast_mw`, `reserve_mw`, `solar_capacity_mw`: megawatts.
- `reserve_rate_pct`, `humidity_pct`: percent.
- `temperature_c`: degrees Celsius.
- `precipitation_mm`: millimeters per hour.
- `irradiance_mj_m2`: megajoules per square meter.
- `solar_generation_mwh`: megawatt-hours for the hour.
- `electricity_gwh`: gigawatt-hours per year.
- `city_gas_tj`, `heat_tj`, `total_energy_tj`: terajoules per year.
- `energy_intensity_index`: index with 2020 set to 100 for each sector.

## Privacy and Safety

The files contain only public energy-system teaching variables. They do not include student records, personal information, customer-level meter data, addresses, facility identifiers, or administrative university data.
