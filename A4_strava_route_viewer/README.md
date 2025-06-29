# A4 — Modules, functions & imports
## Strava Geographic Route Viewer
## Overview
A4.py is module designed for decoding Strava polylines from an already extracted strava dataset, mapping GPS routes interactively and visualizing topographic profile. It combines geospatial libraries with Plotly Dash to generate an interactive dashboard for route analysis.

## Features
- Decode Strava-encoded polyline strings into latitude/longitude coordinates.
- Plot interactive route maps using Folium or Plotly’s Mapbox.
- Generate elevation profiles from Open Elevation API data.
- Interactive dashboard with linked map and elevation views:
    - Hover on route points to highlight corresponding elevation profile points.
    - Synchronized highlighting between map and profile.

## Functions Overview
### decode_polyline(polyline_str)
Decodes a Strava-encoded polyline string into geographic coordinates.

Input: polyline_str (str): Encoded polyline string from Strava
Output: List of coordinates (latitude, longitude)

### plot_route_map(coords)
Creates an interactive Folium map displaying the full route with start and end markers.

Input: coords (list): List of (lat, lon) coordinate tuples
Output: folium.Map: Interactive route map with colored path and markers

### plot_elevation_profile(coords)
Plots an elevation profile along the route using the Open-Elevation API and Matplotlib.

Input: coords (list): List of (lat, lon) coordinate tuples
Output: Displays a plot inline

### interactive_dashboard(coords)
Launches a Dash app with synchronized interactive map and elevation profile.

Input: coords (list): List of (lat, lon) coordinate tuples
Output: Interactive dashboard with hover linking between map and chart

## File Structure
```
A4
├── A4.py      # Main python module containing the functions
├── A4.ipynb   # Jupyter notebook where the functions are utilized
└── README.md  # This file
```

---
## Dependencies:

- polyline
- folium
- matplotlib
- pandas
- geopy
- requests
- plotly
- dash

---
### Author
Nicole Salazar-Cuellar
MSc Candidate in Geoinformatics – Practice: Software Development (Python)
@nicolevasos
Date: June 2025

