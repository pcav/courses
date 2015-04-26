Basic QGIS course
===========================

* Duration: 2 days
* Introduction to the QGIS software

  * interface, customization
  * legend, browser, overview, other components
  * resources: website, mailing lists
  * the custom installer: how and why

* Plugins management
* Vector data

  * properties
  * import/export
  * conversion between formats (here esp. add Comma Delimited Text
  * turn a table into a geographic layer
  * PostGIS layers [#Connections to PostGIS databases available and #data from ``R:\GeoSpatialData``)
* How to use GPS units in QGIS

  * convert data (”waypoints”, ”tracks”, ”routes”) from GPS to GPX
  * add GPX
  * project GPS data (WGS84) to UTM (EPSG:25833)
  * convert data (”points”, ”lines”) from GIS to GPS (GPX)
  * save data on GPS unit
  * add background maps (from AR5, N50… + naturbase…) to GPS unit
  * #single users + schema available for database access

* Projections handling and conversion between CRS; local CRSs [#25833, see wiki page]
* Vector theming, symbology and labels

  * manually (classified, gradual, random)
  * using templates (SLD, QML, QLR)
 
* Tables of attributes

  * basic SQL (for feature selection)

* Actions
* Usage of template projects

* Vector digitizing

  * snapping, topology, reshaping
  * new CAD digitizing?
  
* Editing attributes using «Custom Forms»
* Data from the web

  * discover data (*MetaSearch*: **GeoNorge**)
  * add layers from map servers: WMS, WFS, WFS-T, CSW, WPS, Google Maps [#list available through the custom installer]

* Raster data

  * properties and theming
  * coordinate reference systems management and mosaics
  * conversion between rasters and vectors?
  * georeferencing (just mention the possibility)

* Some useful plugins

  * Mirror map
  * 

Printing
----------

* Simple and Advanced layouts/printing [#see templates]

  * Atlas
  * how to export (best formats)

Analysis
----------------

Learn how to do raster and vector GIS analysis in QGIS. Just briefly mention the QGIS interface with additional tools such as GRASS. Show only the “preferred” solution, not all possible alternatives as it would most likely confuse participants.  Main focus on generic tools which are most frequently used. These tools should be examples for how things can be done (as there is not enough time to go through all kinds of tools).

* Basic vector analyses

  * in QGIS: point sampling (Point Sampling Tool), dissolve, buffer, overlay, attribute management, etc.
  * in PostGIS: running modified #template queries

* Raster data analysis

  * using the GRASS plugin [#DB hopefully available; support uncertain]
  * geomorphology analyses: digital terrain modules, contour, slope, aspect, shaded maps

Advanced Course
=========================================================

* Duration: 2 days

Advanced analysis
------------------

* Various backends available
* Raster

  * using the GRASS plugin [#DB hopefully available; support uncertain]
  * Geomorphology analyses: digital terrain modules, contour, slope, aspect, shaded maps
  * Distance analyses?
  * reclassification of rasters, map algebra
  * zonal statistics
  
* Use R within Processing [#please provide sample scripts and data]
* Modelling through graphical interface and command line
* Automatic land use classification (quick, if we have time; #sample images needed)

PostGIS
--------

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
* Topology support (just mention)

Web
----

* Data publishing

  * QGIS web server interface (OWS) [#QGIS Server available]
  * simple interactive maps on the web (*qgis2leaf* plugin?)
  * mention LizMap

Python
-------

* Interacting with PostGIS using a #simple Python-plugin

  * Run plugin builder
  * Modify UI in QTDesigner
  * Define a connection and run a simple query (possibly with one (hard coded) variable from UI): https://pypi.python.org/pypi/psycopg2, https://pypi.python.org/pypi/py-postgresql

Note
=====

#data required from the locals
