# REQUIREMENT AND TASK FOR PART_ONE CODING

The scikit-learn library provides a suite of different clustering algorithms to choose from, each
offering a different approach to discovering the natural groups in data.
In this part of assignment, you will explore the characteristics of different clustering al-
gorithms by testing them on three toy datasets. You will use the make blobs() function,
make classification (with ”n clusters per class=1”) and make circles (with ”noise=0.3”) to cre-
ate three toy clustering datasets. Each of them will have 1, 000 examples/instances, with two
input features (for ”make classification”, ”n infomative=2”). Keep Other hyperparameters as
default, and set the seed in the dataset generators to get reproducible results

## TASK

1. Fit the clustering models on the datasets and predict a cluster for each example in the
datasets. For clustering models that require specifying the number of clusters, use the
insights obtained from the three data-generating functions. Build a 7-by-3 (7 clustering
algorithms and 3 datasets) table to present the scatter plots showing the clusters gener-
ated by each algorithm.
1. Paragraph to compare and analyse in "".pdf

## part_two.pynb - Observations and How to Run

### HOW TO RUN

- Open vscode
- Make sure you have the necessary libraries and extensions to run the program
- Press Run All at the top of the .ipynb file

### WHAT CODE CONSISTS OF

- Section First: Specifies the seed used across the program. Creates datasets (1000 samples per),
made using make_blobs(), make_classification(), make_circles().
- Section Second: Performs initialization, fitting and prediction of each dataset using KMeans algorithm,
argument n_clusters of KMeans algorithm 3, 2, 2 respectively.
- Section Third: Performs initialization, fitting and prediction of each dataset using Affinity Propagation algorithm,
arguments are random_state as the seed specified in section 2.
- Section Fourth: Performs initialization, fitting and prediction of each dataset using DBSCAN algorithm, without any arguments.
- Section Fifth: Performs initialization, fitting and prediction of each dataset using Guassian Mixure algorithm,
arguments are random_state as the seed specified in section 2.
- Section Sixth: Performs initialization, fitting and prediction of each dataset using Birch algorithm,
argument n_clusters of Birch algorithm 3, 3, 3 respectively.
- Section Seventh: Performs initialization, fitting and prediction of each dataset using Agglomerative Clusetering algorithm,
argument n_clusters of Agglomerative Clusetering algorithm 2, 2, 2 respectively.
- Section Eighth: Performs initialization, fitting and prediction of each dataset using Mean Shift algorithm, without any arguments.
- Section Ninth: Outputs outcomes of each dataset being used in each algorithm to a scatter graph.
