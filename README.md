# Gun Violence Analysis in America

> A statistical analysis of gun violence patterns in the United States (2013-2018). Done together with Cyril Odiwuor (https://github.com/COdiwuor)

## Project Overview
This analysis examines gun violence trends across the United States, focusing on casualties per 100,000 residents at state levels. The project was conducted as part of STA 518, utilizing R for data analysis, visualization, and statistical modeling.

## Table of Contents
- [Installation](#installation)
- [Data Sources](#data-sources)
- [Methods](#methods)
- [Results](#results)
- [Dependencies](#dependencies)
- [Usage](#usage)

## Installation
```r
# Install required R packages
install.packages(c(
  "tidyverse",
  "data.table",
  "skimr",
  "gt",
  "rmdformats",
  "gtExtras",
  "lubridate",
  "sf",
  "naniar",
  "stringr",
  "geofacet",
  "remotes",
  "leaflet",
  "scales",
  "patchwork",
  "htmltools"
))
```

## Data Sources
The analysis utilizes two primary data sources:
1. **Gun Violence Archive (GVA)**
   - Source: [Gun Violence Archive](https://www.gunviolencearchive.org/)
   - Time period: 2013-2018
   - Contains incident-level data on gun violence across the US

2. **US Census Data**
   - Source: County-level census data (2009-2021)
   - URL: [Census Dataset](https://raw.githubusercontent.com/dilernia/STA418-518/main/Data/census_data_county_2009-2021.csv)
   - Used for population normalization and demographic analysis

## Methods
### Data Cleaning
- Utilized `stringr` for string manipulation and standardization
- Employed `lubridate` for date formatting and temporal analysis
- Handled missing data using visualization tools from `naniar`

### Analysis
- Performed population-adjusted analysis (casualties per 100,000 residents)
- Implemented bootstrapping for statistical inference
- Conducted temporal and spatial analysis of gun violence patterns

### Visualization
1. State-level casualty analysis
2. Time series visualization of casualties
3. Choropleth map of gun violence incidents
   - Created using `leaflet` and `sf` packages
   - Incorporated geographic visualization using `geofacet`

![image](https://github.com/user-attachments/assets/21ddceb1-7ecd-4db4-a429-c1636867c574)

![image](https://github.com/user-attachments/assets/a3783bf3-c41e-413e-a595-81eb7e97bfb1)

![image](https://github.com/user-attachments/assets/ef0fd641-cc98-40e7-90ad-559655c2bb9b)


## Dependencies
- R (version 4.3.0 or later)
- RStudio (2023.12.0 or later)

### Required Packages
```r
library(tidyverse)    # Data manipulation
library(data.table)   # Reading data tables
library(skimr)        # Missing data analysis
library(gt)           # Table creation
library(rmdformats)   # HTML document formatting
library(gtExtras)     # GT table theming
library(lubridate)    # Date manipulation
library(sf)           # Spatial visualization
library(naniar)       # Missing data visualization
library(stringr)      # String manipulation
library(geofacet)     # US-shaped plot layouts
library(remotes)      # GitHub package installation
library(leaflet)      # Interactive mapping
library(scales)       # Plot axis scaling
library(patchwork)    # Plot combination
library(htmltools)    # HTML manipulation
```

## Project Structure
```
├── README.md
└── docs/
    └── analysis_report.Rmd
```

## Usage
1. Clone the repository
2. Install required packages using the installation code provided
3. Run scripts in the Rmd File
   ```

## License
MIT License

## Acknowledgments
- Data provided by Gun Violence Archive
- US Census Bureau
- Cyril Odiwuor (https://github.com/COdiwuor)
- Course instructor: Andrew DiLernia (https://github.com/dilernia)
```

 

