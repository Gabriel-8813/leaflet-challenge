# leaflet-challenge
Module 15 challenge

# Overview

The Earthquake Visualization Project is a web application that fetches and displays recent earthquake data from the United States Geological Survey (USGS) using JavaScript and the D3.js library. The project visualizes earthquake locations on an interactive map, providing insights into the magnitude and depth of earthquakes that have occurred over the past week. 

# Features

1. Real-Time Data Fetching: Retrieves earthquake data in GeoJSON format from the USGS API and processes the data for visualization.
2. Interactive Map: Utilizes Leaflet.js to create and manage an interactive map that displays earthquake locations, using markers that represent the magnitude of each earthquake.
Color-Coded Magnitudes: Each earthquake marker is color-coded based on its depth, allowing users to quickly assess the severity of earthquakes at a glance.
3. Informative Popups: Clicking on an earthquake marker displays a popup with the location and timestamp of the earthquake, enhancing user engagement and information retrieval.
4. Map Layers: Users can switch between street and topographic views of the map for better context of earthquake locations.
5. Legend for Depth: A legend is provided at the bottom right of the map, indicating the depth ranges with corresponding colors for quick interpretation.


# Technologies Used

 - HTML/CSS: For structure and styling of the web application.
 - JavaScript: Main programming language used for implementing functionality.
 - D3.js: Library used for fetching and manipulating JSON data.
 - Leaflet.js: JavaScript library for interactive maps, enabling easy positioning and styling of map markers.
 - USGS API: Source of earthquake data available in GeoJSON format.


# Code Explanation

1. Data Fetching:
The application initiates a GET request to the USGS earthquake data endpoint using d3.json(queryUrl), retrieving weekly earthquake data.
2. Earthquake Feature Creation:
The createFeatures function processes the earthquake data, binding relevant properties (like location and time) to each earthquake marker.
The getColor function determines marker color based on the depth of the earthquake.
3. Map Initialization:
The createMap function sets up the Leaflet map, adding base maps (street and topographic) along with the earthquake markers.
A layer control is added to allow users to toggle between different map views.
4. Legend Creation:
A legend provides visual cues for interpreting the color-coded depth information associated with each earthquake.
Installation

To run the Earthquake Visualization Project, ensure you have the following:
 - An internet browser (Chrome, Firefox, etc.)
 - HTML and JavaScript environment (local server or directly open in a browser)

# Steps:

1. Download or clone the project repository.
2. Open index.html in your browser or run a local server to load the page.

# Usage

Upon loading, the map will display markers for recent earthquakes that occurred within the last week.
Click on the markers to see details about each earthquake.
Use the layer controls to switch between street and topographic maps.
Refer to the legend for an understanding of the depth ranges represented by marker colors.

