Basic QGIS course
===========================

* Introduction to the QGIS software

  * interface, customization
  * legend, browser, overview, other components
  * resources: website, mailing lists
  
* Plugins management
* Vector data

  * properties
  * import/export
  * conversion between formats (here esp. add Comma Delimited Text, PostGIS layers [Connections to PostGIS databases will be available ``Import_QGIS_Settings.bat``] and data from ``R:\GeoSpatialData``)

* Projections handling and conversion between CRS; local CRSs [info form locals]
* Vector theming (Symbology?) and labels

  * manually (classified, gradual, random)
  * using templates (SLD, QML, QLR)
 
* Tables of attributes

  * basic SQL (for feature selection)
  * turn a table into a geographic layer

* Actions
* Usage of template projects [check the available ``Import_QGIS_Settings.bat`` with refinements]
* How to use GPS units in QGIS

  * Convert data (”waypoints”, ”tracks”, ”routes”) from GPS to GPX
  * Add GPX
  * Project GPS data (WGS84) to UTM (EPSG:25833)
  * Convert data (”points”, ”lines”) from GIS to GPS (GPX)
  * Save data on GPS unit
  * Add background maps (from AR5, N50… + naturbase…) to GPS unit

* Vector digitizing

  * snapping, topology, reshaping
  * new CAD digitizing?
  
* Editing attributes using «Custom Forms»
* Data from the web

  * Discover data (*MetaSearch*: **GeoNorge**)
  * Add layers from map servers: WMS, WFS, WFS-T, CSW, WPS, Google Maps [list available through ``Import_QGIS_Settings.bat``]

* Raster data

  * Properties and theming
  * Coordinate reference systems management and mosaics
  * Georeferencing (please provide local data?)

Analysis
----------------

Learn how to do raster and vector GIS analysis in QGIS. Just briefly mention the QGIS interface with additional tools such as GRASS. Show only the “preferred” solution, not all possible alternatives as it would most likely confuse participants.  Main focus on generic tools which are most frequently used. These tools should be examples for how things can be done (as there is not enough time to go through all kinds of tools).

* Basic vector analyses

  * In QGIS: point sampling (Point Sampling Tool), dissolve, buffer, overlay, attribute management, etc.
  * In PostGIS: running modified template queries

* Raster data analysis

  * using the GRASS plugin [DB hopefully available; support uncertain]
  * Geomorphology analyses: digital terrain modules, contour, slope, aspect, shaded maps
  * (Distance analyses?)
  * Reclassification of rasters, map algebra
  * Zonal statistics
  * Modelling through graphical interface and command line (advanced?)

* Simple and Advanced layouts/printing [samples available?]
* Data publishing (advanced?)

  * QGIS web server interface (OWS) [QGIS Server available]
  * Simple interactive maps on the web (*qgis2leaf* plugin?) 

Advanced Course on Geodatabases (PostgreSQL and PostGIS)
=========================================================

Aimed at those who need to learn how to use a geodatabase of complex geographic data (do not focus on database setup and management). The course covers the use of PostGIS’ many database functions that allow for complex geoprocessing to be carried out within the database and displayed in real-time. It is suggested to have basic knowledge of the SQL language.

* Advantages of using a database for GIS
* Introduction to the Open Source RDBMS, PostgreSQL
* Schemas, Tables, Views, and Functions
* Introduction to PostGIS (and Open Geospatial Consortium standards)
* Geodatabases: structure and format of the data
* Creation of a geodatabase and the use of the GIS template
* Command line administration: psql
* Two graphical front-ends: QGIS and pgAdmin III
* PostGIS and QGIS: Importing shapefiles, digitizing, queries, plugins for advanced queries
* Advanced geoprocessing functions
* PostGIS rasters
* Topology support
* Interacting with PostGIS using a simple Python-plugin

  * Run plugin builder
  * Modify UI in QTDesigner
  * Define a connection and run a simple query (possibly with one (hard coded) variable from UI): https://pypi.python.org/pypi/psycopg2, https://pypi.python.org/pypi/py-postgresql
