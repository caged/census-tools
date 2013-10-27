### NHGIS Census Importer

Currently there is one command [`nhgis2pgsql`](bin/nhgis2pgsql) that can import extracts from the [The National Historical Geographic Information System](https://nhgis.org).

### Example

``` bash
$ ./bin/nhgis2pgsql -d nhgis -s ~/Desktop/nhgis0010_shape.zip -c ~/Desktop/nhgis0010_csv.zip
```

The command above imports all shapefiles and data files located in the
specified directories into a PostGIS-enabled Postgres database.  The shapefiles are
reprojected to [EPSG:4326](http://en.wikipedia.org/wiki/World_Geodetic_System) (WGS 84).
