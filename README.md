# COVID19_Project

## Data Sources

We sources 3 versions of COVID-19 from the following sources: 

1. New York Times COVID-19 Github repository: https://github.com/nytimes/covid-19-data 

  **We recommend not using this source, as the sources below seemed to have a more ideal format**
  
  * Advantages: 
    * Already in long format, at the state and county level
  * Disadvantages:
    * Mix of county versus city level data, so many FIPS codes are missing 
    * The way data are updated makes it unclear why there are discrepancies in cases/deaths for each date for a given location, and thus which count should be used

2. USA Facts: https://usafacts.org/visualizations/coronavirus-covid-19-spread-map/

  **We recommend using this source for county-level COVID analyses**

  * Advantages:
    * County-level COVID cases, deaths, and overall population data are well documented with clean FIPS codes. These can be merged together and on other data sources.
  * Disadvantages: 
    * In wide format with columns for every date, which means that it must be transformed to long format for most analyses

3. COVID Tracking Project: https://covidtracking.com/data

  **We recommend using this source for state-level COVID analyses**

  * Advantages:
    * Very detailed COVID data, including information about what treatments people are getting (e.g., how many people are in ICU) 
    * Clean FIPS codes can be merged on other data.
  * Disadvantages:
    * Only at the state level 
