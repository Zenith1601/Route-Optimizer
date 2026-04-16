# Route-Optimizer
Shortest path finder using Dijkstra and A* on real Nagpur map data.

# Route Optimizer — Nagpur City 

Shortest path finder using **Dijkstra** and **A\*** algorithms 
on real Nagpur road network data from OpenStreetMap.

# Route
- **Start** — Nagpur Railway Station
- **End** — Deekshabhoomi, Nagpur

# Tech Stack
- Python
- OSMnx — Real map data from OpenStreetMap
- Folium — Interactive map visualization
- NetworkX — Graph operations

# How it Works

### Dijkstra
Explores all roads from source outward, always picking 
the cheapest unvisited node using a min-heap priority queue.
Guaranteed to find the optimal path.

### A\*
Smarter than Dijkstra — uses Haversine heuristic to guide 
search toward the destination. Visits significantly fewer 
nodes while still finding the optimal path.

### Key Difference
| | Dijkstra | A* |
|---|---|---|
| Strategy | Explores blindly | Guided toward goal |
| Nodes Visited | More | Less (~78% fewer) |
| Speed | Slower | Faster |
| Optimal Path | ✅ 

##  Output
- Terminal — travel time, distance, nodes visited comparison
- route_map.html — Interactive map showing:
  - 🔵 Blue line — Dijkstra route
  - 🟢 Green dashed line — A* route
  - 🔴 Red marker — Start (Railway Station)
  - 🟢 Green marker — End (Deekshabhoomi)

##  Concepts Used
- Graph Theory — Nodes (intersections) and Edges (roads)
- Min-Heap Priority Queue — For efficient node selection
- Haversine Formula — Great circle distance as A* heuristic
- OpenStreetMap — Real world road network data
