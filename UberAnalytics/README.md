# Uber pickups statistics notebook
## Notebook uses d3 geo component for Uber taxi pickups representation on the map of New York
Uber taxi pickups data can be found on [Github](https://github.com/fivethirtyeight/uber-tlc-foil-response) 

NYC boundaries  data shapefile source - http://www.nyc.gov/html/dcp/html/bytes/districts_download_metadata.shtml#bcd

Need to create TopoJSON data file from shapefile (http://www.mapshaper.org or topojson commandline)

## Important notes:

* Put the following files in **~/.beaker/v1/web/uberData** folder:

     - .csv file with Uber pickups statistics
     - .json file with TopoJSON data (NYC boundaries map) named as ny.json
     
     
* In case of problem with shapefile rendering (chaotic lines instead of map) need to re-project the shapefile to NAD83 (EPSG 4269) by using GDAL / OGR