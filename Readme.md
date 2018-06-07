# OSM to s57 chart

In this repository small changes are made to be able to convert regions of osm maps to s57 charts.

# Build

The actual code needed sits in the subdirectory 'seachart/josmtos57'

```
cd seachart/josmtos57
ant
touch meta
# osmconvert with the -b=?? statement to clean up the file. 
# Corrupted charts would be the result otherwise
osmconvert ~/data/world.osm -b=8.8588,47.4736,9.7617,47.8316 -o=~/data/bodensee.osm  
java -jar josmtos57.jar ~/data/bodensee.osm meta ~/data/ bodensee.000
