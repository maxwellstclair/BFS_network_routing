# Network Analysis Problem
## Data Structure
The input file branch.csv describes a network topology using three columns
* i: source bus ID
* j: destination bus ID
* ckd_id: circuit ID connecting the buses
These connections are undirected and unweighted
For clarity, a second simple network topology is provided with a visualization – branch_simple_example.csv
## Functions
1. compute_hops(df, start_bus, end_bus) – finds the minimum number of hops between two buses in the network
2. buses_within_hops(df, start_bus, max_hops) – lists all buses within a given number of hops from a starting bus

Both functions rely on the Breadth-First Search (BFS) algorithm because:
* It guarantees the shortest path in unweighted graphs
* It systematically explores nodes level by level
* It's efficient and easy to implement using a queue
## Applications 
* Visualizing or analyzing network topology, such as eleectric transmission networks
*   Validating connectivity in simulation tools (e.g. PSS/E, PowerWorld)
* Educational examples for graph theory on real-world datasets
