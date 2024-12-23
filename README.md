Steam Dataset Analysis and Collaborative Filtering Recommender System

Overview

This project uses the Steam dataset to develop a collaborative filtering recommender system using Spark MLlib. The dataset provides user purchase and play behaviors, enabling the analysis of implicit feedback to train the recommendation model. All tasks are executed within Databricks.

Dataset Description

The dataset, steam-200k.csv, includes the following columns:

User ID: Unique identifier for each user.

Game Name: The name of the purchased or played game.

Behavior: Indicates whether the action is purchase or play.

Value: For purchase rows, this is 1. For play rows, this is the number of hours played.

Key Notes:

A game must be purchased before it can be played, resulting in two rows for some user-game combinations.

An additional games.csv file contains a mapping of game names to unique IDs but implementing the mapping directly in Databricks adds more value.

Objectives

Load the dataset into a Spark DataFrame and conduct initial exploratory analysis.

Preprocess the data, including generating unique integer IDs for users and games.

Use Spark MLlib to train a collaborative filtering recommender system with the Alternating Least Squares (ALS) algorithm.

Experiment with different feedback types (purchase vs. play) and evaluate the model's performance.

Explore the generated recommendations for users.

Steps

1. Data Loading and Exploration

Load the steam-200k.csv dataset into a Spark DataFrame.

Perform exploratory analysis using DataFrames, Spark SQL, and visualizations.

2. Data Preprocessing

Generate unique integer IDs for games and users.

Prepare the data for the ALS algorithm.

Split the dataset into training and testing subsets.

3. Model Implementation

Train a collaborative filtering recommender system using Spark MLlib’s ALS.

Tune hyperparameters (rank, regularization parameter, iterations) for optimal performance.

Test the model on the testing subset and evaluate its performance using metrics such as Root Mean Squared Error (RMSE).

4. Recommendations

Generate personalized game recommendations for users.

Analyze and interpret the results.

Tools and Libraries

Apache Spark: Data processing and model training.

Databricks: Cloud-based platform for collaborative data analysis.

Spark MLlib: Library for machine learning tasks.

Results

Comparative analysis of recommendations using purchase and play behaviors.

Insights into the effectiveness of ALS for implicit feedback data.

Conclusion

This project demonstrates the use of Spark MLlib to build a recommender system from implicit feedback. By analyzing user behaviors, it highlights the potential for personalized gaming recommendations on platforms like Steam.

Files

steam-200k.csv: Dataset used for analysis.

Notebooks: Databricks notebooks containing the implementation steps.

Author

Uchendu Okechukwu MSc Data Science School of Engineering and Environment

