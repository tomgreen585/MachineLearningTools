# REQUIREMENT AND TASK FOR PART_ONE CODING

The part of assignment is to explore several classifiers in scikit-learn and investigate the hy-
perparameter for complexity control for each of these classifiers on three datasets by setting
the hyperparameter to a range of plausible values and seeing how well it does on ”held out”
data. To do this you will need train test split from scikit-learn. To get better estimates, sim-
ply repeat 50 times with different random splits (set the seed to get reproducible results). For
simplicity, use a 50:50 train:test split in all cases. For each setting of the hyperparameter, you
then have a distribution over 50 different classification accuracies on the test set. A nice way
to visualise these scores is to produce a box plot where the x-axis gives options for a parameter
of the model, while the y-axis indicates the spread for classification accuracies of the classifier.
Titles and Axis Labels are needed for clarity.

## TASK

1. Build a 7-by-3 (7 classifiers and 3 datasets) table to present the boxplots on the classifier
accuracy versus parameter values ( as the example table below). It probably won’t fit into
one summary figure. You should structure it as separate main plots, one per classifier,
each consisting of several subplots for different datasets.
2. Present two summary tables, with rows being classifiers, and columns being datasets.
Table (1) is to contain the lowest mean value of the test errors obtained from each classi-
fier with various hyperparameter settings.
Table (2) is to contain the corresponding hyperparameter values for obtaining the best
test errors.
3. Paragraph to compare and analyse in "".pdf

## part_one.pynb - Observations and How to Run

### HOW TO RUN

- Open vscode
- Make sure you have the necessary libraries and extensions to run the program
- Press Run All at the top of the .ipynb file

### WHAT THE CODE CONSISTS of

- First section -> accessing datasets and extracting labels(classes) and data from them as well as scaling the data. also sets up necessary
hyperparameters and arrays for algorithms and outputting data to box-plot
- Second section -> KNeighbors Classifier; runs both of the extracted datasets gotten from the second section and performs knn algorithm on them.
appends the score of each dataset to an array. Uses knn hyperparameter N_NEIGHBORS.
- Third section -> Gaussian Naive Bayes; runs both of the extracted datasets gotten from the second section and performs gnb algorithm on them.
appends the score of each dataset to an array. Uses gnb hyperparameter VAR_SMOOTHING.
- Fourth section -> Logistic Regression; runs both of the extracted datasets gotten from the second section and performs lr algorithm on them.
appends the score of each dataset to an array. Uses lr hyperparameter C.
- Fifth section -> Decision TreeC lassifier; runs both of the extracted datasets gotten from the second section and performs dtc algorithm on them.
appends the score of each dataset to an array. Uses dtc hyperparameter MAX_DEPTH.
- Sixth section -> Gradient Boosting Classifier; runs both of the extracted datasets gotten from the second section and performs gbc algorithm on them.
appends the score of each dataset to an array. Uses gbc hyperparameter MAX_DEPTH.
- Seventh section -> Random Forest Classifier; runs both of the extracted datasets gotten from the second section and performs rfc algorithm on them.
appends the score of each dataset to an array. Uses rfc hyperparameter MAX_DEPTH.
- Eighth section -> MLP Classifier; runs both of the extracted datasets gotten from the second section and performs mlpc algorithm on them.
appends the score of each dataset to an array. Uses mlpc hyperparameter ALPHA.
- Ninth section -> Prints out lowest mean error and best hyperparameter for each of the three datasets per each algorithm. Also outputs each of the datasets
to a boxplot for each of the algorithms passed through it based on accuracy and hyperparameter
