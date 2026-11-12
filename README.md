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
source("scripts/analyze_co2.R")
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
Between 1990 and 2024, carbon dioxide emissions in the United States underwent a marked shift from continuous growth to a sustained trajectory of decarbonization. From 1990 through the mid-2000s, total annual emissions expanded steadily, driven by robust macroeconomic growth, expansion of heavy industrial manufacturing, and widespread reliance on coal-fired electricity generation. Emissions peaked around 2005–2007 at over 6,100 million tonnes per year.

Following this peak, the United States entered a period of structural decline in overall carbon intensity. A primary driver was the domestic "shale gas revolution," which significantly reduced the price of natural gas relative to coal. Power utilities rapidly decommissioned coal-fired power plants in favor of cleaner natural gas and rapidly expanding renewable sources such as wind and solar photovoltaics. Consequently, emissions dropped precipitously over the following decade while real economic output continued to expand—a phenomenon known as absolute decoupling.

The historical timeline also highlights notable macro-economic shocks. The 2008 global financial crisis and the 2020 COVID-19 pandemic caused substantial temporary contractions in industrial production and transportation demand, resulting in sharp single-year drops in emissions. Although post-pandemic economic recovery caused a slight rebound in 2021, per-capita emissions continued their long-term downward trend, reaching approximately 14 tonnes per person by 2024—a reduction of over 30% from 1990 levels. Overall, the data illustrates that energy efficiency improvements, fuel switching in power generation, and structural economic shifts toward service industries have successfully curbed US carbon emissions over the past two decades.

# Limitations
* Scope of Emissions: The dataset focuses primarily on fossil fuel combustion and industrial land-use emissions; it does not fully encompass short-lived non-CO2 greenhouse gases like methane ($CH_4$) or nitrous oxide ($N_2O$).
* Consumption vs. Production: Data reflects territory-based production emissions rather than consumption-based emissions, meaning carbon embedded in imported goods is excluded.
* Data Aggregation: National totals mask significant regional, state-level, and sector-specific variability across energy grids.

# References
* Our World in Data (OWID): CO2 and Greenhouse Gas Emissions Dataset. https://raw.githubusercontent.com/owid/co2-data/master/owid-co2-data.csv
* R Core Team (2024): R: A Language and Environment for Statistical Computing. R Foundation for Statistical Computing, Vienna, Austria. https://www.R-project.org/
