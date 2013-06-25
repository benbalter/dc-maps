# DC Maps

## Maps of Washington DC area public data 

Source: http://data.dc.gov/Main_DataCatalog.aspx

## Process

1. Navigate to http://data.dc.gov
2. Locate a dataset in the "ESRI Shapefile" format
3. Download the zip file
4. Use ogr2ogr to convert to `.geojson` with the `crs:84` SRS

## Bulk processing

1. Follow the steps above to download one or more zipped shapefiles
2. Run [this shell script](https://gist.github.com/benbalter/5858851)

## Requirements to convert

To convert shapefiles to geojson and reproject, you'll need [ogr2ogr](http://www.gdal.org/ogr2ogr.html). On OS X, the easiest way to do this is with [Homebrew](http://mxcl.github.io/homebrew/), by running the command `brew install gdal`.

## Contributing

1. Fork the project
2. Add a `.geojson` file
3. Submit a pull request