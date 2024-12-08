# Houston Blackout Analysis

## Overview
This project contains a geospatial analysis of the 2021 TX power crisis from an environmental justice perspective. Nighttime satellite imagery are cross-referenced with roads, house, district boundary, and median income data to ascertain the extent of the impact, but also how that impact disproportionately affected individuals and families along lines of income.

![](united-states-nightlight.jpg "Nightime in the United States.")

## Description

### File Information
* `blackout_analysis_code.qmd` contains all code for the analysis. In it, we process the data to produce 4 maps, each analyzing different aspects of the blackout and/or the severity of it.
* `blackout_analysis_code.html` documents the analysis in detail. It contains all code and outputs from the code, as well as explaining the steps taken throughout the analysis.
  + `blackout_analysis_code_files/` contains associated files for the rendering of the html.


### File Structure

```         
UCSB-EDS-220-Fisheries-Habitat-Suitability
│
├── README.md
│
├── blackout_analysis_code.qmd
|
├── blackout_analysis_code.html
├── blackout_analysis_code_files/
├── custom.css  # html style information
|
├── UCSB-EDS-223-Houston-Blackout-Analysis.Rproj
│
├── united-states-nightlight.jpg # photo for README
├── .gitignore 
```

## Data Access
The data needed for this analysis is not stored in the repository. The datasets can be loaded from their own respective sources.

* The `VNP46A1` GeoTIFFs are products of the [VIIRS/NPP Daily Gridded Day Night Band 500m Linear Lat Lon Grid Night](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/VNP46A1) from the Level-1 and Atmospheric Archive & Distribution System Distributed Active Archive Center (LAADS DAAC). 
* The roads layer `gis_osm_roads_free_1.gpkg` and houses layer `gis_osm_buildings_a_free_1.gpkg` can both be downloaded from the [OpenStreetMap hosting site Geofabrik](https://download.geofabrik.de/).
* The socioeconomic data `ACS_2019_5YR_TRACT_48.gdb` comes as a ArcGIS proprietary geodatabase format. It can be downloaded from the [U.S. Census Bureau’s American Community Survey](https://www.census.gov/data/developers/data-sets/acs-5year.2019.html#list-tab-1806015614).

## References

### Acknowledgements

#### This project is supported in part by:

-   [EDS 223 Geospatial Analysis at UCSB](https://eds-223-geospatial.github.io/)
-   [UCSB Bren School for Environmental Science and Management](https://bren.ucsb.edu/)
-   [The Master of Environmental Data Science degree at Bren](https://bren.ucsb.edu/masters-programs/master-environmental-data-science)
-   [National Center for Ecological Analysis and Synthesis (NCEAS)](https://www.nceas.ucsb.edu/)
-   [Sam Csik](https://samanthacsik.github.io/)

### Data Citations
| Data | Citation | Link |
|-------------------|----------------------------------|-------------------|
| NASA Worldview VNP46A1 - VIIRS/NPP Daily Gridded Day Night Band 500m Linear Lat Lon Grid Night | Román, M.O., Wang, Z., Sun, Q., Kalb, V., Miller, S.D., Molthan, A., Schultz, L., Bell, J., Stokes, E.C., Pandey, B. and Seto, K.C., et al. (2018). NASA's Black Marble nighttime lights product suite. *Remote Sensing of Environment* 210, 113-143 [Dataset]. doi:10.1016/j.rse.2018.03.017. | [Link to nightlight data.](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/VNP46A1) |
| OpenStreetMap from Geofabrik | OpenStreetMap contributors. (2024). OpenStreetMap [Database]. *Geofabrik*. https://www.geofabrik.de/ | [Link to roads and houses data.](https://download.geofabrik.de/) |
| U.S. Census Bureau American Community Survey 2019 | U.S. Census Bureau. (2022). American Community Survey 5-Year Data (2009-2022) [Database]. | [Link to socioeconomic data.](https://www.census.gov/data/developers/data-sets/acs-5year.2019.html#list-tab-1806015614) |

