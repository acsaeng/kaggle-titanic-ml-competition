# Background
This project includes the following directories and files:
- `data/` - Training and testing Titanic datasets provided by Kaggle
- `results/` - Screenshots of the submission results
- `submission/` - .csv files containing the predictions from each developed machine learning model
- `project.ipynb` - Main project file containing all analyses and results
- `ProjectProposal.md` - Project proposal submitted at the beginning of this project
- `ProjectReadme.md` - Project directives and conclusions (this file)
- `README.md` - Project instructions

# Instructions
The code can all be run from the Jupyter notebook in the order that they are presented. No additional installation packages are required for this project.

# Results

Results are tabulated and visualized in the accompanying Jupyter notebook (*project.ipynb*). This document contains the entire process of handling the data and applying the machine learning models. Its contents are divided into the following sections:

1. Overview
2. Importing the Data
3. Analyzing the Data
    - 3.1 Feature and Target Variables
    - 3.2 Significance of the Data
    - 3.3 Data Visualization
4. Transforming the Data
    - 4.1 Splitting the Data
    - 4.2 Dropping Features
    - 4.3 Applying the Column Transformer
5. Applying Machine Learning Models
    - 5.1 Logistic Regression
    - 5.2 Support Vector Machine
    - 5.3 Random Forest
    - 5.4 Gradient Boosting
6. Conclusion
    - 6.1 Results Summary
    - 6.2 Interpretation of Results
    - 6.3 Reflection

# Interpretation

*A copy of this is also found in Sections 6.2 of the notebook*

In this investigation, machine learning techniques were applied to Kaggle's Titanic dataset to determine if a given passenger survived or did not survive the disaster. The provided data was first imported, analyzed, and visualized to gain some insight on the problem and determine an effective plan of action. The dataset was then modified to be more workable by encoding features, addressing empty values, and removing irrelevant information. Four different supervised machine learning classifiers were used in this analysis - linear regression, support vector machine, random forest, and gradient boosting.

Each machine learning model was put to the test using a column transformer to arrange the features and a grid search to find the optimal hyperparameters. After training the models, each made a set of predictions on the provided testing dataset and were submitted on Kaggle's competition page to obtain its respective accuracy score. The results achieved by each model did not vary by much and were all typically found to underfit the data, as the test score were a bit less than the training score, but not exceeding high overall. The random forest classifier slightly outperformed the other three models, achieve a score of 77.751%. This was then followed by the support vector machine, linear regression, and gradient boosting models. Overall, I would say that these model score decently well in predicting the survival rate of passengers aboard the Titanic.

Although this is a good start, there is also certainly much to be improved with these models in order to achieve better results. With more time, there are a couple of modification that could be made for this project, both in feature extraction and model tuning. One aspect of the features that was completely removed from the beginning was the `Name` column. Many of the names listed here contained certain titles (Miss, Mr., Mrs., etc.). This is one feature that could potentially remain if handled and implemented in a methodical manner. Another addition that could potentially assist in handling the data and in optimizing some of the models is the usage of a scaler, which depending on the model, could have been implemented and possibly improved some of the results.

# Reflection

*A copy of this is also found in Sections 6.3 of the notebook*

This competition was a was a good way to showcase what I have learned over the past semester and in testing my knowledge. It was interesting to walk through the entire process of using real-world data to build supervised machine learning models on my own. After completing this project, I better understand the importance of properly analyzing and manipulating datasets for machine learning model. Another aspect that I have come to realize is that the choices you make on how you present the input data to the model can ultimately determine the true effectiveness of it. In addition, I also learned how to implement useful tools provided by sci-kit learn, such as the column transformer and grid search to improve my workflow and build more robust machine learning models.

Unfortunately, time did not permit me to implement everything that I would have liked to. One task that I was not able to complete was attempting to ensemble some models together. This would have involved combining a set of models together in order to maximize the potential of each and attain a better score. Along with the improvements listed in the previous section, this is a feature that I hope to implement when I revisit this competition again, with the hopes of really improving upon what I accomplished so far.

Overall, I really enjoyed this project, as I've always been fascinated with machine learning in predicting real-world data. I hope to a lot more about learn machine learning in the future and potentially attempt more advanced projects and competitions on my own. Thank you for providing the means and opportunity for us to undertake a project like this!