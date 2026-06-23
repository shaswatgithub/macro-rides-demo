# 🗺️ Macro Rides - Hyperlocal EV Mobility Engine

### 🚀 Zone Boundary & Dynamic Route Corridor Visualization Tool

A high-performance, interactive geospatial visualization tool built for **Macro Rides** to optimize hyperlocal EV fleet dispatching. The application dynamically computes a smooth **350-meter routing corridor** around a live driver, transforms the physical bounding geometry into an optimized discrete **Uber H3 hexagonal grid**, and performs instant constant-time ($O(1)$) screening of active passenger pickup hotspots.

---

## 🔗 Project Links

* **🖥️ Live Interactive Demo:**https://macro-rides-demo.netlify.app/
* **📁 Source Code Repository:** https://github.com/shaswatgithub/macro-rides-demo

---

## 🛠️ Core Engineering Stack

The system utilizes a lightweight, frontend-only single-file architecture deployed entirely via CDN endpoints to guarantee rapid processing speeds without server-side lag:

* **⬢ Uber H3 (`h3-js`):** Hexagonal hierarchical spatial indexing system used to discretize irregular continuous coordinate shapes into 64-bit address hashes for ultra-fast spatial querying.
* **📐 Turf.js:** Advanced client-side geospatial mathematical library used to calculate precise physical spherical buffers and interpolate smooth vehicle route vectors.
* **🗺️ Leaflet.js:** Lightweight open-source mapping canvas used to render spatial layers, dynamic SVG vectors, map tiles, and asset markers smoothly.
* **🌍 OpenStreetMap Nominatim:** Public geocoding interface enabling on-the-fly keyword address resolution and engine teleportation worldwide.

---

## ✨ Interactive Operational Features

* **🔍 Typeable Location Engine:** Type any global landmark or city (e.g., `IIT Kanpur`, `San Francisco`, `Paris`) to instantly shift operational contexts.
* **🎛️ Dynamic Corridor Radius Slider:** Scale the vehicle catchment buffer in real time from `100m` to `1000m` and watch the grid scale dynamically.
* **💎 Variable H3 Resolution Selector:** Toggle between Resolution 8 (~700m), Resolution 9 (~100m), and Resolution 10 (~40m) to evaluate mathematical grid granularity vs performance overhead.
* **📊 Dynamic Pickup Density Adjuster:** Inject between 5 and 150 independent passenger terminal nodes using an automated randomized spatial distribution pattern around your center point.

---

## 🏎️ Data Processing Pipeline
