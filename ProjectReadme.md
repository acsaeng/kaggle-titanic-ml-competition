Here is where you include:
  - Background on your code files
  - How to run your code, guide to install any additional packages
  - Results, interpretation and reflection

# Background
The main directory of this project includes the following directories and files:
- `data/` - Training and testing Titanic datasets provided by Kaggle
- `results/` - Screenshots of the submission results
- `submission/` - .csv files containing the predictions of each developed machine learning model
- `project.ipynb` - Main project file containing all analyses and results
- `ProjectProposal.md` - Project proposal submitted at the beginning of this project
- `ProjectReadme.md` - Project directives and conclusions (this file)
- `README.md` - Project instructions

# Instructions
The code can all be run from the Jupyter notebook in the order that they are presented. No additional packages are required to run this project.

# Results

Results are tabulated and visualized in the accompanying Jupyter notebook (*project.ipynb*). This document contains the entire process of handling the data and applying the machine learning models. Its contents are divided into the following sections:

- 1 Overview
- 2 Importing the Data
- 3 Analyzing the Data
    - 3.1 Feature and Target Variables
    - 3.2 Significance of the Data
    - 3.3 Data Visualization
- 4 Transforming the Data
    - 4.1 Splitting the Data
    - 4.2 Dropping Features
    - 4.3 Applying a Column Transformer
- 5 Applying Machine Learning Models
    - 5.1 Logistic Regression
    - 5.2 Support Vector Machine
    - 5.3 Random Forest
    - 5.4 Gradient Boosting
- 6 Conclusion
    - 6.1 Results Summary
    - 6.2 Interpretation of Results
    - 6.3 Reflection

# Interpretation

*A copy of this is also found in Sections 6.2 of the Jupyter notebook*

In this investigation, machine learning techniques were applied to Kaggle's Titanic dataset to determine if a given passenger survived or did not survive the disaster. The provided data was first imported, analyzed, and visualized to gain more insight on the problem and determine an effective plan of action. The dataset was then modified to be more workable by encoding features, addressing empty values, and removing irrelevant information. Four different supervised machine learning classifiers were used in this analysis - linear regression, support vector classifier, random forest, and gradient boosting.

Each machine learning model was put to the test using column transformer to arrange the features and grid search to find the optimal hyperparameters. After training each model, they were applied to the given testing data and submitted on Kaggle's competition page to obtain the accuracy score. The results achieved by each model did not vary by much and each were typically found to underfit the data, as the score were a bit less than the training score. The random forest classifier slightly outperformed the other three models, obtaining a score of 77.751%. This was then followed by the support vector machine, linear regression, and gradient boosting model. Overall, these model score decently well in predicting the survival of passengers aboard the Titanic.

Although this is a good start, there is also certainly much to be improved with these models in order to achieve better scores. With more time, there are a couple of modification that could be made for this project, both in feature extraction and model tuning. One aspect of the features that was completely removed from the beginning was the `Name` column. Many of the names listed here contain certain title (Miss, Mr., Mrs., etc.). This a one feature that could potentially remain if handled and implemented methodically. Another addition that could help when handling the data and in optimizing the model is using a scaler. Depending on the model, a scaler could have definitely been implemented and possibly improve the results, especially for a model like the support vector classifier.

  # Reflection

  *A copy of this is also found in Sections 6.3 of the Jupyter notebook*