# Tourism Regression Analysis

## Repository Contents
This repository contains the content for the code, data, and figures for an analysis and regression modeling of key tourism metrics. This project was created as part of the the Linear Models course (DS 6021) at the University of Virginia School of Data Science in the Summer of 2024.

## Source Code

### Installing/Building Code in this Repository

After cloning or forking this repository, its contents can be used to recreate different parts of this project. The required modules and packages used in Python and R for this project are listed below.

### Modules Used in this Project

#### Python Modules

This project makes use of the following Python modules:
- `numpy` - for numerical data manipulation
- `pandas` - for data manipulation
- `itertools` - for creating iterators for efficient looping
- `functools` - for creating higher-order functions

#### R Packages
This project makes use of the following R packages:
- `tidyverse` - for data manipulation and visualization
- `ggcorrplot` - for creating correlation plots
- `RColorBrewer` - for data visualization color schemes
- `gridExtra` - for data visualization allignment
- `caret` - for regression model builiding
- `broom` - for data manipulation
- `car` - for detecing multicollinarity

## Code

There are three code files in this repository which can be found in the `src` directory of this repository:
- `data_cleaning.ipynb` ([src](src/data_cleaning.ipynb)). This file contains the Python code used to read, transform, and aggregate the data from the different sources.
- `tourism_exploratory_data_analysis.Rmd` ([src](src/tourism_exploratory_data_analysis.Rmd)). This file contains the R code used for initial data exploration and visualization.
- `tourism_modeling_building.Rmd` ([src](src/tourism_modeling_building.Rmd)). This file contains the R code used for regression model building, training, evaluation, and assessment.
    
## Data

There is raw data collected from four organizations that is used as part of this project, all of which can be found in the `data/raw` section of this repository:
- **UN Tourism**: Datasets collected from the UN Tourism open database, containing key tourism metrics, such as tourism income, number of visitors, and infrastructure
    - `unwto-all-data-download_2022.xlsx`
- **UN Development Programme**: Dataset collected on the historical Human Development Index (HDI) for each country
    - `HDR23-24_Composite_indices_complete_time_series.csv`
- **U.S. Department of Agriculture**: Historical datasets collected on macroeconomic indicators from each country  
    - `RealGDPValues.xlsx`
    - `RealPerCapitaGDPValues.xlsx`
    - `RealExchangeRateValues.xlsx`
    - `CPIValues.xlsx`
- **World Bank**: Historical datasets collected on unemployments from each country  
    - `API_SL.UEM.TOTL.ZS_DS2_en_csv_v2_2431972.csv`

All of the individual data files were processed into a more analytics ready format. All of which can be found in the `data/processed` section of this repository:
- `full_tourism_dataset.csv`: primary dataset used for analysis; contains all the data from all sources
- `country_mapping.csv`: contains the mapping used between data sources for country names
- `tourism_metrics.csv`: contains all of the tourism metrics from the UN Tourism dataset
- `country_codes.csv`: contains the country code mapping used in the UN Tourism dataset
- `economic_metrics.csv`: contains all of the economic data collected from the U.S. Department of Agriculture
- `consumer_price_index.csv`: contains the consumer price index data collected from the U.S. Department of Agriculture
- `exchange_rates.csv`: contains the exchange rate data collected from the U.S. Department of Agriculture
- `gdp.csv`: contains the GDP rate data collected from the U.S. Department of Agriculture
- `gdp_per_capita.csv`: contains the GDP per capita data collected from the U.S. Department of Agriculture
- `hdi.csv`: contains the HDI data collected from the UN Development Programme
- `unemployment_rates.csv`: contains the unemployment rate data collected from the World Bank

## Figures

Figures and visuals for this project can be found in the `figures` directory of this repository.

## References

[1] https://www.unwto.org/tourism-statistics/key-tourism-statistics

[2] https://ers.usda.gov/data-products/international-macroeconomic-data-set.aspx

[3] https://data.worldbank.org/indicator/SL.UEM.TOTL.ZS​

[4] https://hdr.undp.org/data-center/documentation-and-downloads
