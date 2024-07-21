# Utilizing Ant Colony Optimization for Efficient Navigation of Tokyo Metro Network

## Project Overview

This project explores the application of Ant Colony Optimization (ACO), an evolutionary algorithm, to find the shortest path between stations in the Tokyo Metro network. The aim is to enhance the efficiency of navigation in this complex subway system by reducing travel time and minimizing transfers.

## Motivation

As public transport networks grow, they become more complex, making it difficult for users to find the best route. This project leverages ACO to address this challenge, providing a robust solution for optimizing routes in the Tokyo Metro system, known for its complexity and high passenger volume.

## Dataset

The dataset, sourced from Kaggle, includes station names (both in English and Japanese), connections between stations, and distances measured in kilometers. The dataset represents 14 train lines and 291 unique stations.

## Methodology

### Data Preprocessing

- Organized data into a table with stations and corresponding lines.
- Created a graph of the metro network using Networkx.
- Verified data accuracy using the Dijkstra algorithm for initial validation.

### Ant Colony Optimization Implementation

- Parameters: number of ants, number of iterations, pheromone evaporation rate, influence of pheromones, and heuristic effect.
- Initialization: Equal pheromone levels across the network.
- Pheromone Update: Pheromones deposited based on distance traveled, with evaporation over iterations.
- Edge Selection: Ants select paths based on pheromone concentration and heuristic values.

### Graphical User Interface (GUI)

- Developed using Tkinter in Python.
- Allows users to select origin and destination stations interactively.
- Displays the shortest path and associated stations.

## Results

- The configuration with 50 ants provided the most efficient path.
- Comparative analysis showed Dijkstra’s algorithm performed better in terms of computational cost and path efficiency for specific scenarios.
- ACO demonstrated adaptability and the ability to find multiple valid solutions, making it suitable for complex networks.

## Discussion and Conclusions

The ACO algorithm effectively optimized routes in the Tokyo Metro network, demonstrating potential for broader applications in urban transit systems. Future work includes integrating real-time data and further tuning ACO parameters to improve performance.

## Repository Structure

- `TokyoMetro_AntColonyOptimazation_Algorithm_Final.ipynb`: Jupyter notebook containing the implementation of the ACO algorithm.
- `ACIT4620_Report.pdf`: PDF containing the project report.
- `Program demo.md`: .md file that contains an example of the program.
  

## References

- Wei, Y., et al. (2022). An Improved Ant Colony Algorithm for Urban Bus Network Optimization Based on Existing Bus Routes. ISPRS International Journal of Geo-Information, 11(5), 317. [Link](http://dx.doi.org/10.3390/ijgi11050317)
- Hsiao, Y.-T., et al. (2020). Ant colony optimization for best path planning. [Link](https://www.researchgate.net/publication/4135314_Ant_colony_optimization_for_best_path_planning)
- Tokyo Metro Co., Ltd. Characteristics of Tokyo Metro. [Link](https://www.metro-ad.co.jp/en/characteristic/)

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
