[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Farnoldmuiruri%2Fgun_violence_analysis&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Views&edge_flat=false)](https://hits.seeyoufarm.com)

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

![README-unnamed-chunk-5-1](https://github.com/user-attachments/assets/2b02dfb7-9e66-4c9d-8a49-8b37e7f37707)
![README-unnamed-chunk-4-1](https://github.com/user-attachments/assets/a617cff6-082c-41c9-894c-5cf4632dde61)
![README-unnamed-chunk-42-1](https://github.com/user-attachments/assets/1e2b0025-c02c-44d8-8304-8a9521cae8be)
![README-unnamed-chunk-41-1](https://github.com/user-attachments/assets/668c1d71-2506-41d3-b304-bc87f63e0159)
![README-unnamed-chunk-39-1](https://github.com/user-attachments/assets/44971927-c79f-4859-acc1-fc9a225131fc)
![README-unnamed-chunk-33-1](https://github.com/user-attachments/assets/737b5a12-94f0-4a80-87fa-ed74c0f2ab15)
![README-unnamed-chunk-31-1](https://github.com/user-attachments/assets/15f79fee-d8ee-44d9-810f-9923ae5d885e)
![README-unnamed-chunk-26-1](https://github.com/user-attachments/assets/008dea46-ca07-41cf-b1af-945e9676ad2a)
![README-unnamed-chunk-24-1](https://github.com/user-attachments/assets/b41b4b76-cf73-4cbe-8576-76a4c772aa62)
![README-unnamed-chunk-23-1](https://github.com/user-attachments/assets/7333ccac-f952-4d05-bd57-78e243461f6e)
![README-unnamed-chunk-21-1](https://github.com/user-attachments/assets/1f5857bc-c799-4adb-aa4d-f7ae41e83268)
![README-unnamed-chunk-11-1](https://github.com/user-attachments/assets/364022d2-41a5-4b35-8571-d57cc1068bc4)



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

 

