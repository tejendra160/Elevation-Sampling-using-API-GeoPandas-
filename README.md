# Elevation-Sampling-using-API-GeoPandas-
This project demonstrates a simple yet powerful geospatial data pipeline that integrates a public elevation API with Python-based spatial analysis tools.


The goal is to extract elevation values for sample locations within a watershed boundary and generate geospatial outputs for further analysis.

Using the Watershed 22 (W22) shapefile, the workflow generates random points within the watershed, queries elevation data from the Open-Elevation API, and stores the results in both tabular and spatial formats.

This project is designed as a learning example for:

API usage in geospatial workflows
GeoPandas-based spatial processing
Data integration for environmental and hydrologic analysis


Workflow Overview

The project follows a step-by-step geospatial pipeline:

Load Watershed Boundary

Read shapefile using GeoPandas

Ensure valid geometry

Convert coordinate system to WGS84 (required for API)


Generate Sample Points

Create random points inside watershed boundary

Ensure all points fall within the polygon


API Integration

Send latitude/longitude requests to elevation API

Retrieve elevation (meters) for each point


Data Storage

Save results as:

CSV (tabular data)

GeoPackage (spatial data)


Visualization

Plot watershed boundary

Overlay sampled points colored by elevation

 boundary
Overlay sampled points colored by elevation
