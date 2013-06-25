# DC Maps

## Maps of Washington DC area public geodata 

## Source

http://data.dc.gov/Main_DataCatalog.aspx

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

## Fine print

> The data made available here has been modified for use from its original source, which is the Government of the District of Columbia. Neither the District of Columbia Government nor the Office of the Chief Technology Officer (OCTO) makes any claims as to the completeness, accuracy or content of any data contained in this application; makes any representation of any kind, including, but not limited to, warranty of the accuracy or fitness for a particular use; nor are any such warranties to be implied or inferred with respect to the information or data furnished herein. The data is subject to change as modifications and updates are complete. It is understood that the information contained in the web feed is being used at one's own risk.