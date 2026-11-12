# CO2-emissions-USA
CO2 emissions analysis of the United States using R
# Assessing Historical Trends in United States CO2 Emissions (1990–2024)

## Research Question
How have annual fossil fuel CO2 emissions and per-capita emissions changed in the United States from 1990 to 2024?

## Data Source and Definitions
* **Data Source:** Our World in Data (OWID) CO2 and Greenhouse Gas Emissions dataset.
* **Key Metrics:** 
  * `year`: The calendar year of observation.
  * `co2`: Total annual fossil fuel and industrial CO2 emissions measured in million tonnes.
  * `co2_per_capita`: Annual CO2 emissions per person measured in tonnes.

## How to Reproduce the Analysis
1. Open this repository as an RStudio Project.
2. Ensure you have an active internet connection.
3. Run the analysis script in the RStudio console:
   ```r
   source("scripts/analyze_co2.R")
   Key Findings & Visualizations
Total Emissions: Peak emissions occurred in the mid-2000s, followed by a steady downward trend driven by transitions in energy infrastructure.

Per-Capita Trends: Per-capita emissions show a consistent decline, reflecting decoupling of economic growth from carbon intensity.
