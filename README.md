# Heuristic competition for modified CVRP
* Written by: [Poon Athit S. ](https://www.linkedin.com/in/athit-srimachand/), Carol Fan
* Technologies: VBA, constructive heuristics, local search algorithms, meta-heuristics
## 1. Introduction
This project is initiated by a competition among MSc Business Analytics cohorts to build the best 3 heuristic models to solve modified Capacitated Vehicle Routing Problem (CVRP) in VBA. The case we are dealing with is designed from the real-life warehouse picking situation yet simplified. With a set of orders in different locations and a trolley with limited capacity, the time services of picking jobs should be minimized to decrease the costs incurred. In this context, three constraints are considered: capacity of trolley and incompatibility of orders while each order is picked only once; each route starts/ends at the depot; and the algorithm run-time must not exceed 5 minutes in VBA. 

**The competition problems are broken down into 3 parts as follows:**
  * Problem1: Build the best-performance constructive heuristic model
  * Problem2: Build the best-performance pure local search algorithm to improve the initial solution from naive method
  * Problem3: Build the best-performance meta-heuristic algorithm to improve the initial solution from naive method

**The algorithms we chose for each problem are:**
  * Algorithm1: Parametric Clarke-Wright (Parametric CW)
  * Algorithm2: The local search model that selects neighbourhoods from 6 basic local search algorithms (LSA)
  * Algorithm3: Tabu search (TSA)

## 2. Key findings
The three algorithms applied on six instances are parametric CW, LSA, and TSA. The results are analyzed mainly based on the comparison with benchmarks. The overall performance of three algorithm designs is acceptable given an execution time limit of five minutes, with the result of two instances outperforming that of the cohorts for each part. This makes us to be the group with the highest number of best known solutions in this competition. The performance of each algorithm is illustrated into the following tables.

### 2.1 Performance of Parametric CW
<img src="https://github.com/PoonAthitS/heuristic-competition/blob/main/Tables/Table1.png?raw=true" width="800">

### 2.2 Performance of LSA
<img src="https://github.com/PoonAthitS/heuristic-competition/blob/main/Tables/Table2.png?raw=true" width="600">

### 2.3 Performance of TSA
<img src="https://github.com/PoonAthitS/heuristic-competition/blob/main/Tables/Table3.png?raw=true" width="750">

## 3. About the model
Each model's algorithm can be demonstrated by the diagrams as follows

### 2.1 Parametric CW model
<img src="https://github.com/PoonAthitS/heuristic-competition/blob/main/Diagrams/Diagram1.PNG?raw=true" width="700">

### 2.2 LSA model
<img src="https://github.com/PoonAthitS/heuristic-competition/blob/main/Diagrams/Diagram2.1.PNG?raw=true" width="700">

Each sub local search algorithms can be displayed in this node diagram.
<img src="https://github.com/PoonAthitS/heuristic-competition/blob/main/Diagrams/Diagram2.2.PNG?raw=true" width="600">

### 2.3 TSA model
<img src="https://github.com/PoonAthitS/heuristic-competition/blob/main/Diagrams/Diagram3.PNG?raw=true" width="700">


## 4. About the programming

### 4.1 Files
The algorithms are built in an Excel with VBA codes embeded: [Heuristic_algorithm.xlsm](https://github.com/PoonAthitS/heuristic-competition/blob/main/Heuristic_algorithms.xlsm)

### 4.2 Data
We use the mock-up warehouse CVRP input data with their incompatibility constraints in the TXT input data folder

### To learn more about Poon Athit S., visit his [LinkedIn profile](https://www.linkedin.com/in/athit-srimachand/)

All rights reserved 2022. All codes are developed and owned by Poon Athit S. or the metioned team member(s). If you use this code, please visit his LinkedIn and give him a skill endorsement in Data analytics and the aforementioned coding technologies.
