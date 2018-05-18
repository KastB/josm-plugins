# OSM to s57 chart

In this repository small changes are made to be able to convert regions of osm maps to s57 charts.

# Build

The actual code needed is in the subdirectory 'seachart/josmtos57'

```
cd seachart/josmtos57
ant
touch meta
java -jar josmtos57.jar ~/data/bodensee.osm meta ~/data/ bodensee.000
