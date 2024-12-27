# Airline-Route-Analysis-Project
This project analyzes airline routes to explore hub connectivity and identify insights for airline AL35's expansion. Using graph-based analysis, it examines critical airports, connections, and optimal hubs. The study processes a dataset of 6,700 routes to derive actionable insights for improved decision-making.

Objectives

The main objectives of the project include:
Filtering and reducing the raw dataset to only include routes for the airline AL35.
Representing the airline's routes as an undirected graph, with airports as nodes and connections as edges.
Computing graph metrics such as node degree, density, diameter, and centrality to identify key hubs.
Determining the next potential hub for the airline based on data-driven metrics.

Key Steps:

Dataset Reduction:
From the raw dataset of 6,700 routes, only the routes for AL35 are extracted, resulting in 393 records.
A clean, reduced dataset is created for further analysis.

Graph Construction:
The reduced dataset is represented as an undirected graph.
Airports serve as nodes, and flight connections between them are edges.
Duplication of edges is avoided (i.e., bi-directional connections are treated as a single edge).

Graph Analysis:
Metrics such as the number of nodes (airports), edges (routes), graph density, and connected components are computed.

Observations:
86 nodes (airports) and 196 edges (routes) in the graph.
Graph density is low, indicating many airports are underutilized or lack direct connections.
The graph is a single connected component, ensuring all nodes are reachable.

Key Findings:
The top 5 airports based on connections are identified:
Chengdu Shuangliu International Airport (CTU)
Chongqing Jiangbei International Airport (CKG)
Kunming Changshui International Airport (KMG)
Xi'an Xianyang International Airport (XIY)
Harbin Taiping International Airport (HRB)
CTU is the busiest airport, with 54 connections, making it the central hub for AL35.

Next Hub Identification:
Using graph metrics like degree centrality, betweenness centrality, and closeness centrality, Xi'an Xianyang International Airport (XIY) is identified as the most suitable choice for the next hub.

Factors considered include:
High centrality metrics.
Accessibility to major cities.
Potential for future expansion.

Tools and Techniques
Programming Language: Python
Libraries Used: Pandas, NetworkX, Matplotlib

Graph Metrics:
Degree Centrality: Measures connections of an airport.
Betweenness Centrality: Identifies bottleneck nodes on shortest paths.
Closeness Centrality: Measures average distance to other nodes.
Key Files

routes_v3.txt: Contains raw airline route data.
FinalCode.ipynb: Main analysis code.
Graph generation and analysis are performed using the NetworkX library.
