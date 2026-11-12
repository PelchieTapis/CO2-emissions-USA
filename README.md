# United States CO2 Emissions Analysis (1990–2024)
Student: Tapis, Maria Pelchie D. Country / ISO-3: United States / CHE Study period: 1990 to 2024 Declared to instructor on: [November 12, 2026]
# Assessing Historical Trends in United States CO2 Emissions (1990–2024)

## Research Question
How have total annual fossil fuel CO2 emissions and per-capita CO2 emissions trended in the United States between 1990 and 2024, and what structural or economic factors account for these temporal shifts?

## Data Source and Definitions
* **Data Source:** Our World in Data (OWID) CO2 and Greenhouse Gas Emissions dataset. https://raw.githubusercontent.com/owid/co2-data/master/owid-co2-data.csv
* **Key Metrics:** 
  * year: The calendar year of observation (filtered for 1990–2024).
  * co2: Annual emissions of fossil fuel and industrial carbon dioxide CO2, measured in million tonnes (Mt).
  * co2_per_capita: Annual fossil fuel CO2 emissions per person, measured in tonnes per person.
  * co2_growth_prct: The percentage change in total annual CO2 emissions compared to the preceding year.

# How to Reproduce the Analysis
* Clone or Download the Repository:
Ensure the project folder structure remains intact:
CO2-emissions-USA/
├── data/
├── figures/
├── results/
├── scripts/
│   └── analyze_co2.R
├── .gitignore
└── README.md
* Open the Project in RStudio:
Launch RStudio and set your working directory to the project root folder.
* Execute the Script:
Run the analysis script in the RStudio Console:
source("scripts/analyze_co2.R")
The script automatically downloads the latest dataset from OWID, filters the records for the United States (USA), outputs cleaned datasets to data/ and results/, and saves high-resolution plots into figures/.

# Results
Summary Table Overview
| Metric | Value | Year / Details |
| :--- | :--- | :--- |
| **Target Country** | United States | ISO3 Code: USA |
| **Analysis Period** | 1990 – 2024 | 35-year historical timeframe |
| **Peak Total Emissions** | ~6,130 million tonnes | Mid-2000s |
| **Recent Total Emissions (2024)** | ~4,700 million tonnes | Continuous decline from peak |
| **Peak Per-Capita Emissions** | ~20.5 tonnes / person | Early 1990s to late 1990s |
| **Recent Per-Capita Emissions (2024)** | ~13.8 tonnes / person | Significant overall reduction |
| **Major Disruption Events** | 2008 & 2020 | Global Financial Crisis & COVID-19 pandemic |
| **Primary Energy Driver** | Coal to Gas & Renewables | Structural grid decarbonization |

# Annual Total CO2 Emissions
<img width="1440" height="840" alt="image" src="https://github.com/user-attachments/assets/fb5512ff-580b-49e2-a759-9f0fcf44c40d" />

# Per-Capita CO2 Emissions
<img width="1440" height="840" alt="image" src="https://github.com/user-attachments/assets/08860cfa-8ce7-463b-b678-e2cea7026839" />

# Annual Percentage Change in Emissions
<img width="1440" height="840" alt="image" src="https://github.com/user-attachments/assets/646d4aff-690d-47c0-85d7-ede0255a782a" />

# Interpretation
Between 1990 and 2024, United States CO2 emissions demonstrated distinct structural shifts reflecting economic transitions, policy changes, and technological advances in energy production. Total annual CO2 emissions expanded steadily throughout the 1990s, reaching a peak in the mid-2000s near 6,000 million tonnes. Following this peak, total emissions entered a downward trajectory driven largely by the sharp transition from coal-fired electricity generation toward natural gas and renewable energy sources such as wind and solar.

Per-capita emissions reached their peak earlier and declined significantly faster than total emissions, decreasing from over 20 tonnes per person in 1990 to under 14 tonnes per person by 2024. This divergence indicates a structural decoupling of economic and population growth from direct carbon intensity. Sharp downward spikes in total emissions and annual growth rates correspond directly to major external disruptions, including the 2008 global financial crisis and the 2020 COVID-19 pandemic, both of which caused temporary contractions in industrial production and transportation demand. Despite post-crisis economic recoveries, emissions failed to return to their former peaks, confirming a long-term transition toward a less carbon-intensive energy grid.

# Limitations
* Scope of Emissions: The dataset focuses primarily on fossil fuel combustion and industrial land-use emissions; it does not fully encompass short-lived non-CO2 greenhouse gases like methane ($CH_4$) or nitrous oxide ($N_2O$).
* Consumption vs. Production: Data reflects territory-based production emissions rather than consumption-based emissions, meaning carbon embedded in imported goods is excluded.
* Data Aggregation: National totals mask significant regional, state-level, and sector-specific variability across energy grids.

# References
* Our World in Data (OWID): CO2 and Greenhouse Gas Emissions Dataset. https://raw.githubusercontent.com/owid/co2-data/master/owid-co2-data.csv
* R Core Team (2024): R: A Language and Environment for Statistical Computing. R Foundation for Statistical Computing, Vienna, Austria. https://www.R-project.org/
