# KultVis — Visualizing Cultural Values in Urban Planning

> An interactive web-based map visualization tool built with Leaflet for exploring cultural activities, historical sites, and visitor movement patterns in the Lindholmen district of Gothenburg, Sweden.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Leaflet](https://img.shields.io/badge/Leaflet-1.9.4-green.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow.svg)

---

## Features

- **Interactive Leaflet Map:** Custom basemap integration (CartoDB Light) centered on Lindholmen and Gothenburg.
- **Cultural Sites Mapping:** Dynamic rendering of cultural locations from shapefile data (`.zip`) mapped to custom color-coded categories (Museum, Library, Studio, Cinema, Cultural House).
- **Relationscape Lindholmen:** Pre-configured markers and interactive layers for 30+ historic and urban points of interest (e.g., Karlatornet, Backa teater, Kuggen, Lindholmen Manor).
- **Animated Migration & Visitor Arcs:** Custom canvas-based animated arc layers (`MigrationLayer`) visualizing visitor flows for events like Capoeira workshops, large concerts, and fairs.
- **Dual Perspective Control:** Dedicated quick-zoom buttons for switching between local views (Lindholmen close-up) and global views (visitor migration flows).
- **Interactive UI Controls:** Collapsible activity analytics panel displaying activity distribution and interactive legend filters for individual data layers.

---

## Technology Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript (ES6)
- **Mapping Framework:** [Leaflet.js v1.9.4](https://leafletjs.com/)
- **Geospatial Processing:** [shpjs (Shapefile to GeoJSON)](https://github.com/mbostock/shapefile)
- **Tiles:** [CartoDB Positron / Light](https://carto.com/attributions)

---

## Project Structure

```text
.
├── index.html                       # Main entry point and map container
├── kulturverksamheter_utdrag_GBG_251212.zip  # Shapefile dataset containing cultural sites
└── activities_bar_graph.png          # Analytics image for the activities widget
