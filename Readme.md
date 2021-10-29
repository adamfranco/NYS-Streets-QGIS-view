# About
This directory contains a QGIS view that can be applied to the [NYS Streets](http://gis.ny.gov/gisdata/inventories/details.cfm?DSID=932) data set to assist with highway classification in OSM.

The color-coding of roads in this view corresponds to the colors used in the JOSM OpenStreetMap editor to allow comparison views.

As described in [Proposal:New York/Highway Classification](https://wiki.openstreetmap.org/wiki/Proposal:_New_York/Highway_Classification), New York State's Arterial Classification Codes (ACC) are useful for identifying the proper OSM highway classification for major highways. In particular ACC=1 maps well to `highway=motorway`, ACC=2 maps well to `highway=trunk`, and ACC=3 maps well to `highway=primary`. Lower ACC levels are less deterministic for classifying lower OSM `highway=*` levels.

## Author
This QGIS view was prepared by [Adam Franco](https://www.openstreetmap.org/user/Adam%20Franco) for the [New York Highway Classification project](https://wiki.openstreetmap.org/wiki/Proposal:_New_York/Highway_Classification).

# Usage
1. Download and install [QGIS](https://qgis.org/) if you do not already have it on your computer.
2. Clone this repository or simply download the `NYS Streets QGIS view.qgs` file.
3. Download the `NYS Streets.shp.zip` file from http://gis.ny.gov/gisdata/inventories/details.cfm?DSID=932
4. Unzip the `NYS Streets.shp.zip` file into the same directory the `NYS Streets QGIS view.qgs` file from this project.

   This should give you the following directory structure:
   ```
   NYS Streets QGIS view.qgs
   NYS Streets.shp/
   Readme.md
   ```
5. Open the `NYS Streets QGIS view.qgs` file using QGIS. After a bit of loading you should you should see a rendered view of the top road levels organized by ACC.

   ![Screen Shot](./Screen Shot.png)

After loading the file you can pan and zoom as well as filter different ACC levels.
