
# 🚑 Shortest Path and Ambulance Management System

This project simulates an ambulance dispatch system that determines the **shortest route** from the **nearest ambulance** to the emergency location using graph-based pathfinding algorithms like Dijkstra's.

> ✅ **To run the project**, execute:
```bash
python Main.py
```

---

## 🧠 Objective

The aim of this project is to **reduce emergency response time** by automatically assigning the nearest ambulance to an emergency and calculating the optimal path using weighted graphs.

---

## ✅ Features

- 🚨 Automatically finds the **nearest ambulance**
- 📍 Computes **shortest path** using Dijkstra's algorithm
- 🗺️ Simulates a simple city as a graph with distances
- 📊 Visualizes the route and graph using `matplotlib`
- 💡 Easy to customize with your own map or ambulance positions

---

## 🏁 Getting Started

### 🔧 Requirements

Make sure you have the following Python libraries installed:

- Python 3.x  
- `networkx`  
- `matplotlib`

Install using pip if needed:

```bash
pip install networkx matplotlib
```

---

### ▶️ Running the Project

1. Clone or download this repository.
2. Navigate to the project directory.
3. Run the main file:

```bash
python Main.py
```

This will launch the console output and a plot window showing the graph and the path.

---

## 🧱 Project Structure

```
📁 AmbulanceShortestPath/
├── Main.py                 # Main execution and visualization
├── GraphBuilder.py         # Builds the city graph (nodes & edges)
├── AmbulanceManager.py     # Finds the nearest ambulance
├── ShortestPath.py         # Calculates the shortest path
└── README.md               # Documentation
```

---

## 🧪 How It Works

1. A city is represented as a **graph** with nodes (locations) and edges (roads with weights).
2. Ambulances are placed at fixed nodes.
3. The user defines an **emergency location**.
4. The system calculates:
   - Which ambulance is **closest** (least total edge weight)
   - The **shortest path** from that ambulance to the emergency
5. The result is displayed in the terminal and plotted on a graph.

---

## 🖼️ Screenshots

### 🖥️ Console Output

![Console Output](images/output_console.png)

### 🗺️ Graph Visualization

![Graph View](images/graph_view.png)

---

## 📚 Sample Output

```text
Nearest Ambulance is at: A, Distance: 14
Shortest Path: ['A', 'C', 'B', 'D', 'E']
Total Distance: 14
```

Legend in the Graph:
- 🟦 Blue = locations
- 🟩 Green = selected ambulance
- 🟧 Orange = emergency location
- 🔴 Red = computed path

---

## 💡 Future Enhancements

- Integration with **real-world maps** (OpenStreetMap, Google Maps API)
- Use of **live GPS data** for ambulances
- Web interface or mobile app
- Traffic-aware routing
- Priority queue optimization with A* algorithm

---

## 🙌 Acknowledgments

This is an academic/simulation project aimed at demonstrating how algorithms can assist in emergency services and logistics using pathfinding and graph theory.

---

## 📜 License

This project is open-source under the [MIT License](LICENSE).
