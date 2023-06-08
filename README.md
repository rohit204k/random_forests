# Random Forests - From Scratch
## Simple implementation of Random Forests Algorithm

Random Forests is a state-of-the-art ensemble algorithm which combines the output of multiple decision trees to produce combined results. Each tree is trained on a slightly different bootstrap dataset.
This is a very simple implementation of Random Forests algorithm designed for learning purpose.

## Features
- The dataset file to run the code is present in the repo. Alternatively, any other .csv file can also be provided.
- Ensure the the target class columnd is named as 'target'.
- This algorithm is capable of handling both categorical and numerical attributes.
- The numerical attributes need not be normalised.
- The stopping criterion can be changed for each tree individually. 
- I have used the following criterion
      1. Minimum gain - Minimum information gain to continue training process.
      2. Maximum depth - Maximum depth of a tree.
      3. Minimum size - Minimum dataset split size beyond which training process has to be stopped.
  A combimation of these can be used by providing None for the heuristic which need not be used. 
- The algorithm also implement K-fold cross validation and each forest is trained/tested against different datasets and the results are averaged.
- I have plotted accuracy, precision, recall and f1-score of model over training and testing data by varying the number of tree in the forest.
- The effect of increasing the number of trees on the model's performance can be studied through the graphs.

## Steps to run the code

1. The .ipynb file can be run through jupyter notebook
2. The .py file needs to be run through the following commands. ( The .py file can be generated using the .ipynb file)
    * Ensure that all requirements have been installed using
        ```sh
            pip install -r requirements.txt
        ```
    * Run the file using
        ```sh
            python random_forests_voting_dataset.py
        ```
