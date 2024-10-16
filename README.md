# Singapore Bus and Train Heat Map

This project aims to create a **graphical representation of bus stops and train stations** over Singapore, coupled with a **heat map showing real-time and historical arrival times**. The project will be developed from scratch, minimizing reliance on external dependencies, frameworks, or libraries.

*Note: This README has been graciously summarized by AI since I'm too lazy to write one myself.* 😄

## Objectives
1. **Graphical Representation**: Visualize the geographical locations of bus stops and train stations in Singapore.
2. **Heat Map**: Show real-time and historical data of bus and train arrival frequencies. Heat intensity will increase based on the frequency or waiting times of buses and trains.
3. **Minimal Dependencies**: Create core functionalities (polling, data storage, graphical rendering) from scratch with as few pre-built libraries or frameworks as possible.
4. **Custom Data Handling**: Manually handle data parsing, storage, and manipulation, including creating a custom format for storing bus stops and train stations.
5. **Manual Rendering**: Implement a basic rendering engine to display the map and heat map without using pre-made graphics libraries.

## Self-Imposed Limitations
1. **No High-Level Frameworks**: Avoid using high-level frameworks such as Mapbox, Google Maps API, or even common web frameworks. Everything will be built from scratch.
2. **Custom Rendering**: The graphical map and heat map visualization will be created manually, avoiding pre-made rendering engines like Leaflet or D3.js.
3. **Low-Level Programming**: Prefer low-level programming techniques, such as writing custom JSON parsers, HTTP clients, and basic I/O handling without relying on existing libraries (beyond system libraries).
4. **Minimal Use of External Libraries**: Apart from basic system libraries or APIs (like HTTP request handling or X11 for graphics), avoid external dependencies as much as possible.
5. **Flat-File Data Storage**: Avoid using relational databases (like SQLite or PostgreSQL) unless absolutely necessary. Use flat-file systems (e.g., CSV, custom formats) for data storage.

## To-Do List
### Phase 1: Data Collection and Storage
- [ ] Poll bus and train arrival data from public APIs (e.g., *MyTransport.sg*).
- [ ] Write custom code to fetch and parse JSON responses from APIs.
- [ ] Store bus stop and train station coordinates in flat files (CSV, or custom format).
- [ ] Design a simple flat-file time-series storage system for arrival times.

### Phase 2: Map Rendering
- [ ] Write a custom 2D map rendering engine using basic system libraries.
- [ ] Plot bus stop and train station locations on the map.
- [ ] Implement zooming and panning on the map.

### Phase 3: Heat Map Implementation
- [ ] Develop a custom heat map algorithm based on bus/train arrival frequencies.
- [ ] Create a manual color gradient for visualizing heat intensities.
- [ ] Overlay the heat map on top of the graphical representation of Singapore’s transport network.

### Phase 4: User Interface
- [ ] Implement user interaction for zooming, panning, and querying data at specific stops.
- [ ] Display real-time updates of bus/train arrival data on the map.
- [ ] Add functionality to toggle between bus and train networks.

### Phase 5: Optimization and Enhancements
- [ ] Optimize memory usage and performance for real-time data visualization.
- [ ] Implement caching for precomputed heat maps.
- [ ] Refine graphical rendering for better performance with larger data sets.

## Future Plans
- Implement a **mobile-friendly version** with minimal resource usage.
- Add support for **historical data analysis**, allowing users to view trends over time.
- Introduce **route planning** integration, building on top of pathfinding algorithms for public transport systems.
