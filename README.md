# QAOA Partitioning

## Partitioned QAOA vs. Unpartitioned Classical Solver
The [notebook](https://github.com/Amana-L/qaoa-partitioning/blob/main/part_QAOA_v_s_GW.ipynb) provides the code used to solve MaxCut with;

i. using the partitioning to split up the problem and then applying QAOA using the PennyLane Simulator

ii. the Goemans-Williamson algorithm without partitioning the principal problem

The metric used to compare solution quality is the cut size. The data used in the plot given in the paper can also be found in the notebook.

## Comparison of Classical Solvers with & without Partitioning
The [notebook](https://github.com/Amana-L/qaoa-partitioning/blob/main/Part_v_s_Unpart_GW.ipynb) explores the impact of graph partitioning on the MaxCut problem and demonstrates an end-to-end solution for MaxCut, both with and without an initial partitioning step.

To quantitatively assess the effect of partitioning, we compare the cut size obtained in both scenarios. The ratio of these cut sizes serves as a key metric for solution quality. Furthermore, recognizing that graph structure influences MaxCut solutions, we also present the results in relation to the characteristics of the input graphs.
