# STA 250 Winter 2025 COVID-19 Dataset

COVID-19 dataset with daily confirmed cases, deaths, and other covariates. The Dataset was created in collaboration with Zichun Hu.

## Usage

The dataset is the `STA_250_COVID19_Dataset.csv` found in the repository. To use it, you can clone or download the repository and use a programming language or spreadsheet editor to manipulate the data.

### County FIPS Codes

County FIPS codes can be used to identify a county uniquely in a way that is independent of the state. This resolves name conflicts where two counties in different regions have the same name (e.g. "Fremont County"). The FIPS code is constructed with a two digit state number followed by a three digit county number. For example, Autauga County in Alabama has the county code 001. Alabama's state code is 01, so the FIPS code is "01001." For more information, please refer to [this site](https://transition.fcc.gov/oet/info/maps/census/fips/fips.txt).

### Column Descriptions

The dataset can be split into three categories. The community data and population data represent the covariate data that can be used for a more detailed analysis. 

The COVID-19 and community follows the same convention as the USAFacts COVID-19 dataset, where each column represents a particular day. There is no daily population data, only yearly. This data 

#### COVID-19 Data

- `mm/dd/yyyy` - The number of confirmed cases of COVID-19 in a county on the specified day 
- `mm-dd-yyyy_deaths` - The number of COVID-19 related deaths in a county on the specified day

#### Community Data 

 - `mm-dd-yyyy_retail_and_recreation_percent_change_from_baseline`
 - `mm-dd-yyyy_residential_percent_change_from_baseline`
 - `mm-dd-yyyy_workplaces_percent_change_from_baseline`
 - `mm-dd-yyyy_transit_stations_percent_change_from_baseline`
 - `mm-dd-yyyy_parks_percent_change_from_baseline`
 - `mm-dd-yyyy_grocery_and_pharmacy_percent_change_from_baseline`

The percent change from baseline in the specified categories on the specified day. For more information, there is a detailed data overview on the [source website](https://support.google.com/covid19-mobility/answer/9824897?hl=en&ref_topic=9822927&sjid=8831651663638123175-NC).

#### Population Data

- `yyyy-POPESTIMATE` – Estimated total population.
- `yyyy-POPEST_MALE` – Estimated male population.
- `yyyy-POPEST_FEM` – Estimated female population.
- `yyyy-UNDER5_TOT` – Total population under 5 years old.
- `yyyy-UNDER5_MALE` – Male population under 5 years old.
- `yyyy-UNDER5_FEM` – Female population under 5 years old.
- `yyyy-AGE513_TOT` – Total population aged 5–13.
- `yyyy-AGE513_MALE` – Male population aged 5–13.
- `yyyy-AGE513_FEM` – Female population aged 5–13.
- `yyyy-AGE1417_TOT` – Total population aged 14–17.
- `yyyy-AGE1417_MALE` – Male population aged 14–17.
- `yyyy-AGE1417_FEM` – Female population aged 14–17.
- `yyyy-AGE1824_TOT` – Total population aged 18–24.
- `yyyy-AGE1824_MALE` – Male population aged 18–24.
- `yyyy-AGE1824_FEM` – Female population aged 18–24.
- `yyyy-AGE16PLUS_TOT` – Total population aged 16 and older.
- `yyyy-AGE16PLUS_MALE` – Male population aged 16 and older.
- `yyyy-AGE16PLUS_FEM` – Female population aged 16 and older.
- `yyyy-AGE18PLUS_TOT` – Total population aged 18 and older.
- `yyyy-AGE18PLUS_MALE` – Male population aged 18 and older.
- `yyyy-AGE18PLUS_FEM` – Female population aged 18 and older.
- `yyyy-AGE1544_TOT` – Total population aged 15–44.
- `yyyy-AGE1544_MALE` – Male population aged 15–44.
- `yyyy-AGE1544_FEM` – Female population aged 15–44.
- `yyyy-AGE2544_TOT` – Total population aged 25–44.
- `yyyy-AGE2544_MALE` – Male population aged 25–44.
- `yyyy-AGE2544_FEM` – Female population aged 25–44.
- `yyyy-AGE4564_TOT` – Total population aged 45–64.
- `yyyy-AGE4564_MALE` – Male population aged 45–64.
- `yyyy-AGE4564_FEM` – Female population aged 45–64.
- `yyyy-AGE65PLUS_TOT` – Total population aged 65 and older.
- `yyyy-AGE65PLUS_MALE` – Male population aged 65 and older.
- `yyyy-AGE65PLUS_FEM` – Female population aged 65 and older.
- `yyyy-AGE04_TOT` – Total population aged 0–4.
- `yyyy-AGE04_MALE` – Male population aged 0–4.
- `yyyy-AGE04_FEM` – Female population aged 0–4.
- `yyyy-AGE59_TOT` – Total population aged 5–9.
- `yyyy-AGE59_MALE` – Male population aged 5–9.
- `yyyy-AGE59_FEM` – Female population aged 5–9.
- `yyyy-AGE1014_TOT` – Total population aged 10–14.
- `yyyy-AGE1014_MALE` – Male population aged 10–14.
- `yyyy-AGE1014_FEM` – Female population aged 10–14.
- `yyyy-AGE1519_TOT` – Total population aged 15–19.
- `yyyy-AGE1519_MALE` – Male population aged 15–19.
- `yyyy-AGE1519_FEM` – Female population aged 15–19.
- `yyyy-AGE2024_TOT` – Total population aged 20–24.
- `yyyy-AGE2024_MALE` – Male population aged 20–24.
- `yyyy-AGE2024_FEM` – Female population aged 20–24.
- `yyyy-AGE2529_TOT` – Total population aged 25–29.
- `yyyy-AGE2529_MALE` – Male population aged 25–29.
- `yyyy-AGE2529_FEM` – Female population aged 25–29.
- `yyyy-AGE3034_TOT` – Total population aged 30–34.
- `yyyy-AGE3034_MALE` – Male population aged 30–34.
- `yyyy-AGE3034_FEM` – Female population aged 30–34.
- `yyyy-AGE3539_TOT` – Total population aged 35–39.
- `yyyy-AGE3539_MALE` – Male population aged 35–39.
- `yyyy-AGE3539_FEM` – Female population aged 35–39.
- `yyyy-AGE4044_TOT` – Total population aged 40–44.
- `yyyy-AGE4044_MALE` – Male population aged 40–44.
- `yyyy-AGE4044_FEM` – Female population aged 40–44.
- `yyyy-AGE4549_TOT` – Total population aged 45–49.
- `yyyy-AGE4549_MALE` – Male population aged 45–49.
- `yyyy-AGE4549_FEM` – Female population aged 45–49.
- `yyyy-AGE5054_TOT` – Total population aged 50–54.
- `yyyy-AGE5054_MALE` – Male population aged 50–54.
- `yyyy-AGE5054_FEM` – Female population aged 50–54.
- `yyyy-AGE5559_TOT` – Total population aged 55–59.
- `yyyy-AGE5559_MALE` – Male population aged 55–59.
- `yyyy-AGE5559_FEM` – Female population aged 55–59.
- `yyyy-AGE6064_TOT` – Total population aged 60–64.
- `yyyy-AGE6064_MALE` – Male population aged 60–64.
- `yyyy-AGE6064_FEM` – Female population aged 60–64.
- `yyyy-AGE6569_TOT` – Total population aged 65–69.
- `yyyy-AGE6569_MALE` – Male population aged 65–69.
- `yyyy-AGE6569_FEM` – Female population aged 65–69.
- `yyyy-AGE7074_TOT` – Total population aged 70–74.
- `yyyy-AGE7074_MALE` – Male population aged 70–74.
- `yyyy-AGE7074_FEM` – Female population aged 70–74.
- `yyyy-AGE7579_TOT` – Total population aged 75–79.
- `yyyy-AGE7579_MALE` – Male population aged 75–79.
- `yyyy-AGE7579_FEM` – Female population aged 75–79.
- `yyyy-AGE8084_TOT` – Total population aged 80–84.
- `yyyy-AGE8084_MALE` – Male population aged 80–84.
- `yyyy-AGE8084_FEM` – Female population aged 80–84.
- `yyyy-AGE85PLUS_TOT` – Total population aged 85 and older.
- `yyyy-AGE85PLUS_MALE` – Male population aged 85 and older.
- `yyyy-AGE85PLUS_FEM` – Female population aged 85 and older.
- `yyyy-MEDIAN_AGE_TOT` – Median age of the total population.
- `yyyy-MEDIAN_AGE_MALE` – Median age of the male population.
- `yyyy-MEDIAN_AGE_FEM` – Median age of the female population.


## Sources

- [COVID-19 Community Mobility Reports](https://www.google.com/covid19/mobility/)
- [US COVID-19 cases and deaths by state | USAFacts](https://usafacts.org/visualizations/coronavirus-covid-19-spread-map/)
- [County Population by Characteristics: 2020-2023](https://www.census.gov/data/tables/time-series/demo/popest/2020s-counties-detail.html?utm_source=chatgpt.com)
