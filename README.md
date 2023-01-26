# Knapsack problem 
The objective of this project is to implement some algorithms for solving the Knapsack Problem and to provide an experimental study of their running time and quality.
The algorithm implemented in this project are the followings: 

1. The brute-force algorithm that explore all the possible solutions in a systematic way,
2. Dynamic programming approach,
   1. A Dynamic programing version,
   2. And a Top Down version that optimizes the number of calls
3. The Fully polynomial time approximation scheme
4. A version based on a randomized approach (MCMC - Markov chain Monte Carlo).
5. Four Greedy version : 
   1. Greedy weight
   2. Greedy Value
   3. Greedy Ratio
   4. Greedy Fractional
6. Two Branch and bound version :
   1.  Branch and Bound BFS (Best First Search)
   2.  Branch and Bound DFS (Depth first search)
7. Two genetic algorithm
   1. One that take the optimal solution (Genetic optima)
   2. And the second that search the best capacity (Genetic No Optima)
8. A version based on Ant colony approach.  

# Table of Contents
- [Knapsack problem](#knapsack-problem)
- [Table of Contents](#table-of-contents)
- [Installation](#installation)
  - [Jupiter Lab](#jupiter-lab)
  - [Python](#python)
- [Data \& Analyze](#data--analyze)
  - [Architecture of the result folder](#architecture-of-the-result-folder)
  - [File generated](#file-generated)


# Installation

## Jupiter Lab
To launch this you need Jupiter lab, we advice you to use it in VSCode.

Get started with VSCode:\
https://code.visualstudio.com/docs/datascience/jupyter-notebooks

## Python
You will need to have python on your machine and have or install the package listed in the main section in the source code.

# Data & Analyze

For each algorithm we provide curves and tables inside pdf files, we give the The curves and the graphs are in the folder ```results data/analysis/all```

The Excels source files are also provided inside the ```results data/analysis/``` folders.


## Architecture of the result folder

The ``results-data`` folder contain two folder the ``raw-data`` folder which contain the data generated from the algorithm and the analysis folder which contain the analysis made with the raw data.

Below an example of the architecture generated inside the ``raw-data`` folder when you generate data from the source code. 

```
result-data
│   
│   
└─── raw
│   │   
│   │
│   └─── RANDOM
│   │   │   
│   │   └─── BRUTE FORCE   
│   │   │   │ 
│   │   │   └─── small 
│   │   │   │ res-10-10
│   │   │   │ res-10-100
│   │   │   │ res-10-1000
│   │   │   │
│   │   │   └─── medium
│   │   │   │ res-100-10
│   │   │   │ res-100-100
│   │   │   │ res-100-1000
│   │   │   │
│   │   │   └─── large
│   │   │   │ res-1000-10
│   │   │   │ res-1000-100
│   │   │   │ res-1000-1000
│   │   │
|   │   └───DYNAMIQUE
│   │   │    │ 
│   │   │    └─── small 
│   │   │    │ res-10-10
│   │   │    │ res-10-100
│   │   │    │ res-10-1000
│   │   │    │
│   │   │    └─── medium
│   │   │    │ res-100-10
│   │   │    │ res-100-100
│   │   │    │ res-100-1000
│   │   │    │
│   │   │    └─── large
│   │   │    │ res-1000-10
│   │   │    │ res-1000-100
│   │   │    │ res-1000-1000
│   │   │
│   │   └─── ...
│   │  
│   └─── NORMAL
│   │   │   
│   │   └─── BRUTE FORCE   
│   │   │   │ 
│   │   │   └─── small 
│   │   │   │ res-10-10
│   │   │   │ res-10-100
│   │   │   │ res-10-1000
│   │   │   │
│   │   │   └─── medium
│   │   │   │ res-100-10
│   │   │   │ res-100-100
│   │   │   │ res-100-1000
│   │   │   │
│   │   │   └─── large
│   │   │   │ res-1000-10
│   │   │   │ res-1000-100
│   │   │   │ res-1000-1000
│   │   │
│   │   └─── ...
│   └─── ...
```

## File generated

A file generated is named with the prefix `res` and followed by two numbers, the first number is the number of item and the second the capacity.
For example `res-10-100` mean that the test was launched with 10 items and a capacity of 100.

Then regarding the content of a generated file, the last 4 lines of the file correspond to the minimum, maximum and average time of execution and usage of memory of the algorithm, the last line is the solution finded by the algorithm.
