### PROBLEM STATEMENT:

We were given the task of building a model to help the company increase its ability to predict those who would be most at risk of defaulting on a car loan. After balancing our drastically balanced classes, 50% became our baseline accuracy. 

The company has the goal of giving back by identifying those on the line of qualiying for, or at risk of defaulting on a car loan. From there the company will assist them by enrolling them in a personal finance program designed to increase likelihood of approval and reduce likelihood of default. 

### Questions We Seek To Answer:

1. Can we accurately predict who is mostly likely to default on a car loan?


### Table of Contents:

1. Data: includes csv files of datasets used as well as a data dictionary
2. Notebooks: includes Cleaning, EDA, Feature Selection and Modeling notebooks
3. Visuals: visuals from the EDA process and results from model performance

### Process:

Our data was extracted from a kaggle challened and initially contained heavy class inbalance. SMOTENC was used to balance the classes. Next feature selection which included seperating continuous features from categorical features then binarizing as necessary. EDA was performed on binary features and most were found to not be worth including in the model. 

Continuous values were relatively normal in distributuon with the exception of a few outliers (approximately 3,244 out of 233,154 values). Those outliers were managed by imputing mean values for outliers  exactly three or more deviations from the mean (less than 1.5% of data and on just one feature). From there the goal was to identifify as many unique and non-correlated features as possible and include them in the model. 

There were three versions of feature selection and each member of the team ran individual models to test performance. 

### Software Requirements

Pandas, Numpy, Scikit-learn, Imblearn, MatPLotLib, & Seaborn 