# eds223-extreme-weather

# EDS 223: Winter Storm Impacts in Houston, TX 

## Purpose
This repository contains data and code to identify and visualize the impacts of the February 2021 Texas power crisis caused by a series three of extreme winter storms, based on NASA remotely-sensed night lights data and OpenStreetMap data. 

## Repository Structure 
This repository is structured as follows:

```
eds223-extreme-weather
├── README.md
├── extreme_weather.pdf
└── extreme_weather.qmd
|   .gitignore
    └───data
        └─── gis_osm_buildings_a_free_1.gpkg.zip
        └─── gis_osm_roads_free_1.gpkg.zip
        └─── VNP46A1
            ├── VNP46A1.A2021038.h08v05.001.2021039064328.tif
            ├── VNP46A1.A2021038.h08v06.001.2021039064329.tif
            ├── VNP46A1.A2021047.h08v05.001.2021048091106.tif
            └── VNP46A1.A2021047.h08v06.001.2021048091105.tif
```

## Data Access  
The specific files used in this exercise can be downloaded using [this link](https://drive.google.com/file/d/1bTk62xwOzBqWmmT791SbYbHxnCdjmBtw/view?usp=drive_link). The data used in this project originated from the following sources:

1. Visible Infrared Imaging Radiometer Suite ([VIIRS](https://en.wikipedia.org/wiki/Visible_Infrared_Imaging_Radiometer_Suite)) data from the Suomi satellite, distributed through NASA’s Level-1 and Atmospheric Archive & Distribution System Distributed Active Archive Center ([LAADS DAAC](https://ladsweb.modaps.eosdis.nasa.gov/)).

Data files:
* `VNP46A1.A2021038.h08v05.001.2021039064328.tif`: tile h08v05, collected on 2021-02-07
* `VNP46A1.A2021038.h08v06.001.2021039064329.tif`: tile h08v06, collected on 2021-02-07
* `VNP46A1.A2021047.h08v05.001.2021048091106.tif`: tile h08v05, collected on 2021-02-16
* `VNP46A1.A2021047.h08v06.001.2021048091105.tif`: tile h08v06, collected on 2021-02-16

2. Texas road data from [OpenStreetMap](https://planet.openstreetmap.org/). The EDS 223 teaching team used [Geofabrick](https://download.geofabrik.de/) to retrieve a shapefile of all highways in Texas and prepared a Geopackage containing just the subset of roads that intersect the Houston metropolitan area. 

Data files:
* `gis_osm_roads_free_1.gpkg`

3. Texas building data from [OpenStreetMap](https://planet.openstreetmap.org/), downloaded from [Geofabrick](https://download.geofabrik.de/). The EDS 223 teaching team prepared a GeoPackage containing only houses in the Houston metropolitan area.

Data files:
* `gis_osm_buildings_a_free_1.gpkg`

## Authors
[Courtney Lorey](https://github.com/cllorey/cll214final), Bren School of Environmental Science & Management, University of California, Santa Barbara

## References

Data prepared by the EDS 223 teaching team. 

NASA Black Marble VIIRS/NPP Daily Gridded Day Night Band 15 arc-second Linear Lat Lon Grid Night (VNP46A1), Version 1, tiles h08v05 and h08v06, February 7 and February 16, 2021. 2021. *NASA Level-1 and Atmospheric Archive & Distribution System Distributed Active Archive Center (LAADS DAAC)*. Retrieved: November 2026, from [https://ladsweb.modaps.eosdis.nasa.gov/](https://ladsweb.modaps.eosdis.nasa.gov/).

OpenStreetMap Texas Roads (gis_osm_roads_free_1), subset to the Houston metropolitan area. 2021. *Geofabrik GmbH; © OpenStreetMap contributors*. Retrieved: November 2026, from [https://download.geofabrik.de/north-america/us/texas.html](https://download.geofabrik.de/north-america/us/texas.html).

OpenStreetMap Texas Buildings (gis_osm_buildings_a_free_1), subset to houses in the Houston metropolitan area. 2021. *Geofabrik GmbH; © OpenStreetMap contributors*. Retrieved: November 2026, from [https://download.geofabrik.de/north-america/us/texas.html](https://download.geofabrik.de/north-america/us/texas.html).
