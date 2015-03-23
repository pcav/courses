Basic QGIS course content
===========================

* Introduction to the QGIS software
* Plugins management
* Vector data

  * Properties
  * import/export
  * conversion between formats (here esp. add Comma Delimited Text, PostGIS layers and data from R:\GeoSpatialData)
  * Basic SQL (for feature selection)

* Projections handling and conversion between CRS; local CRSs
* Vector theming (Symbology?) and labels

  * manually (classified, gradual, random)
  * using templates (SLD, QML, QLR)
 
* Tables of attributes. Turn a table into a geographic layer
* Actions
* Usage of template projects
* How to use GPS units in QGIS

  * Convert data (”waypoints”, ”tracks”, ”routes”) from GPS to GPX
  * Add GPX
  * Project GPS data (WGS84) to UTM (EPSG:25833)
  * Convert data (”points”, ”lines”) from GIS to GPS (GPX)
  * Save data on GPS unit
  * Add background maps (from AR5, N50… + naturbase…) to GPS unit

* Vector digitizing and editing attributes using «Custom Forms»
* Data from the web

  * Discover data (MetaSearch)
  * Add layers from map servers: WMS, WFS, WFS-T, CSW, WPS, Google Maps

* Raster data

  * Properties and theming
  * Coordinate reference systems management and mosaics
  * Georeferencing (please provide local data?)

* Analysis

Learn how to do raster and vector GIS analysis in QGIS. Just briefly mention the QGIS interface with additional tools such as GRASS. Show only the “preferred” solution, not all possible alternatives as it would most likely confuse participants.  Main focus on generic tools which are most frequently used. These tools should be examples for how things can be done (as there is not enough time to go through all kinds of tools). 

  * Basic vector analyses
  
    * In QGIS: point sampling (Point Sampling Tool), dissolve, buffer, overlay, attribute management, etc.
    * In PostGIS: running modified template queries

* Raster data analysis

  * using the GRASS plugin
  * Geomorphology analyses: digital terrain modules, contour, slope, aspect, shaded maps
  * Raster and vector buffers, distance analyses, least cost paths
  * Reclassification of rasters, map algebra
  * Zonal statistics

* Simple and Advanced layouts/printing
* Data publishing

  * QGIS web server interface (OWS)
  * qgis2leaf-plugin (Simple interactive maps on the web) 

Advanced Course on Geodatabases (PostgreSQL and PostGIS)
=========================================================
