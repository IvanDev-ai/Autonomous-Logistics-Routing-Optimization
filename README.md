# PharmaDrone Madrid: Pathfinding Optimization and Intelligent Logistics Simulation

### Data Structures & Algorithms Project — PHE Applied Computing & Artificial Intelligence
**Author:** Iván Lumbreras Martín  
**Academic Year:** 2024-2025

---

## 1. Overview
PharmaDrone Madrid is a technical simulation designed to optimize the autonomous delivery of pharmaceutical supplies in urban environments. This project focuses on solving complex routing problems by implementing advanced pathfinding algorithms over a custom-built graph representing the city of Madrid.

The system manages a fleet of drones, accounting for real-world constraints such as payload capacity, battery consumption, and dynamic obstacles (no-fly zones, weather conditions, and military airspace).

---

## 2. Core Technical Challenges
* **Routing & Pathfinding:** Implementation and comparison of **Dijkstra’s Algorithm** and **A*** to determine the most efficient paths in a weighted graph.
* **Dynamic Constraint Management:** Integration of "adversity factors" including restricted airspace (Zonas Militares), green zones, and battery-to-distance ratios.
* **Data Structures:** Utilization of Abstract Data Types (ADTs), FIFO Queues for order management, and complex Graphs for urban navigation.

---

## 3. System Architecture

### Graph Theory Implementation
The urban map is modeled as a weighted graph where:
* **Nodes:** Represent key locations in Madrid (Moncloa, Chamberí, Atocha, etc.).
* **Edges:** Represent navigable flight paths with associated "costs" (distance and risk factors).
* **Library:** Built using `NetworkX` for graph manipulation and visualization.

### Algorithm Benchmarking
1.  **Dijkstra:** Used for finding the absolute shortest path in a static environment.
2.  **A* Search:** Enhanced with heuristics to optimize search time and computational efficiency for real-time delivery requests.

### Drone Logic
* **Payload Management:** Capacity limited to 5kg per drone.
* **Energy Optimization:** Real-time battery tracking based on flight distance and payload weight.

---

## 4. Features & UI
* **Web-Based Interface:** A functional dashboard (implemented via `pyngrok` and Flask/Colab) that allows users to place orders, select destinations, and specify pharmaceutical weights.
* **Real-Time Simulation:** Visual tracking of the drone's route, showing the sequence of nodes visited until successful delivery.

---

## 5. Results and Key Learnings
* Achieved a 100% success rate in route calculation across 10+ simulated urban nodes.
* Demonstrated significant computational efficiency gains by utilizing A* heuristics compared to standard breadth-first approaches.
* Validated the importance of robust data structures (FIFO Queues) in managing concurrent delivery requests in high-demand scenarios.

---

## 6. Technology Stack
* **Language:** Python
* **Libraries:** NetworkX, Geopy, Matplotlib
* **Algorithms:** A* (A-Star), Dijkstra, Graph Traversal
* **Concepts:** Data Structures (Queues, Graphs, ADTs), Logistics Optimization

---

## 7. Repository Structure
* `src/` — Core implementation of the routing engine and simulation logic.
* `docs/` — Comprehensive technical report and architectural presentation.
* `assets/` — Visual representations of the city graph and algorithm performance.

---

## 8. Academic Output
* Technical assignment submitted for the **Unit 19: Data Structures & Algorithms** module.
* Full documentation on routing complexity and algorithmic efficiency.

---

## Author
**Iván Lumbreras Martín** Computer Science Graduate | Aspiring Data Scientist / ML Engineer  
**Specialized in:** Algorithm Optimization & Intelligent Systems.

---
*Last updated: April 2026*
