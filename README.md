Feature Selection using Boolean Artificial Bee Colony (BABC) Algorithm

This project implements the Boolean Artificial Bee Colony (BABC) algorithm in Python for feature selection on the Breast Cancer dataset from Scikit-learn.
The goal is to improve model efficiency by selecting the most relevant features while maintaining high classification accuracy.

Overview

Feature selection is a critical step in building efficient machine learning models.
By reducing the number of input features, we lower model complexity, speed up computation, and often improve generalization.
This implementation uses a metaheuristic optimization approach, inspired by the foraging behavior of honey bees, to search for the best subset of features.

Methodology

Data Preparation: Load and standardize the Breast Cancer dataset.

Baseline Model: Train a Random Forest classifier using all 30 features.

Fitness Function: Combine model accuracy and feature reduction to evaluate each subset.

BABC Algorithm: Explore and update candidate solutions (feature masks) using employed, onlooker, and scout bee phases.

Evaluation: Compare baseline accuracy with accuracy obtained using the selected features.

Results

Baseline accuracy (all features): ~95.6%

Optimized accuracy (selected features): ~94.9%

Feature reduction: ~53%

The algorithm successfully selected a smaller subset of features while keeping nearly the same predictive performance, demonstrating the power of metaheuristic optimization in feature selection tasks.
