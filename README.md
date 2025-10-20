# Region Clustering Project
My project research where I use Gurobi solver on Python environment to optimize the best place to set the warehouse.

## Concept
Based on the given location information in excel file to find the optimal warehouse.

## Define the region clustering based on latitude and longtitude
Using Elbow method to optimization number of clusters then apply KMeans clustering with 3 clusters and Display the map

## Defining warehouse location
Using **gurobipy library** to minimize the sum of Euclidean distance

This can be formulated as a Second-Order Cone constraint:
(s_i)^2 >= (optimal_lat_gm - lat_i)^2 + (optimal_long_gm - long_i)^2

## Design milk-run path starting from the defined warehouse location to all cities in "Miền Tây" Viet Nam
I need Distance Matrix and Subtour elimination constraints (Miller-Tucker-Zemlin) knowledge to set up TSP model then using the **gurobipy library** to minimize the run path.

