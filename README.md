# genetic-algorithm-crew-scheduling
Parallel Genetic Algorithm for Airline Crew Scheduling

Genetic Algorithm for Airline Crew Scheduling
Prescriptive Analytics Project — Masters of Data Analytics

This project builds a Parallel Genetic Algorithm (GA)–based solver for optimizing airline crew schedules. Crew scheduling is one of the most complex and expensive operational challenges in aviation. Our solution combines meta-heuristics + multi-threading to generate near-optimal pairings faster than traditional solvers.

🔍 Project Overview

Airline crew costs are the second largest operational expense, and traditional solvers like CPLEX and Gurobi become slow as the number of flights increases.

We implemented a Parallel GA Framework inspired by Ouyang & Zhu (2023) to:

1. Improve runtime efficiency.

2. Increase crew–flight matching.

3. Enhance scalability in large datasets.

<img width="526" height="430" alt="image" src="https://github.com/user-attachments/assets/886754e9-6ef7-4ba0-a7d0-d59ea3cc849e" />

What is a Genetic Algorithm?

Genetic Algorithms simulate evolution using:

Selection

Crossover

Mutation

Repeated over generations to reach an optimized solution.
Our framework improves GA performance using parallelism and population drift for stability.

⚙️ Parallel GA Framework

Multi-threaded implementation (MPI)

Exchange of chromosomes between populations

Faster convergence

More stable results

Scales effectively for large flight datasets

| Dataset | Flights | Crew | Airports |
| ------- | ------- | ---- | -------- |
| A       | 206     | 21   | 7        |
| B       | 13,954  | 465  | 39       |

Key Results
Dataset A

✔ 96.6% flights matched

✔ 85% faster runtime compared to CPLEX

✔ Crew utilization: ~44 flights/month

✔ High stability for small problems

Dataset B

✔ 93.4%+ flights matched

✔ 45–60% faster than Gurobi

✔ Efficient scheduling for 13,954 flights

✔ Outperformed traditional GA & commercial solvers

| Solver                 | Flights Solved | Runtime | Efficiency |
| ---------------------- | -------------- | ------- | ---------- |
| **CPLEX**              | 198            | 147 min | Low        |
| **Gurobi**             | 13,225         | 524 min | Moderate   |
| **Parallel GA (ours)** | 13,496         | 284 min | High       |


Business Impact

Major savings for airlines annually

Handles crew shortages and disruptions

Boosts crew fairness and utilization

Reduces cancellations & delays

Applicable across logistics, manufacturing & healthcare

🙋 Team Members

Aena Parekh

Akash Kumar

Aundeep Yathepu

Supervised by: Prof. William Pourmajidi

📚 Reference

Ouyang, W., & Zhu, X. (2023). Meta-heuristic solver with parallel genetic algorithm framework in airline crew scheduling. Sustainability, 15(2), 1506.


