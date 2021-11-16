### This repo has the following artifacts
- multiple_linear_regression.ipynb
- final_model_for_submission.ipynb
- production_deployment.ipynb
- models/DecisionTreeRegressor_GridSearchCV.sav
- models/DecisionTreeRegressor_RandomizedSearchCV.sav


### multiple_linear_regression.ipynb
This notebook has the exploratory data analysis I carried out as the initial step to make sense of the input dataset. 

This allowed me to understand following
 - Summary of the dataframe (list of data items, data types)
 - Null value check
 - Descriptive statistics (record_count, mean value, standard deviation of the data items etc.., )
 - Insights into number of properties in the dataset for a given number of bedrooms
 - Data visualisations using libraries such as matplotlib and seaborn
 - Correlations to understand the relation between the data features
 
### final_model_for_submission.ipynb
**This is the artifact for the submission.**

This notebook conatins the following
- Changes based on feature engineering decisions made
- Applied the following algorithams to asses their model accuracy
  - Decision Tree Regressor
    - Learning curve plots
    - GridsearchCV
    - RandomizedSearchCV
  - Linear Regression
  - RANSACRegressor 
  - Ridge Regression 
  - Lasso Regression 
  - ElasticNet Regression 
  - PolynomialFeatures
  - SGDRegressor
  
 This allowed me to demonstrate which model fits best for the input dataset.
 
 Analysis showed that the following two models generated using ML hyper parameters techniques gave similar results, hence submmiting both the models.
 - GridsearchCV
 - RandomizedSearchCV

### production_deployment.ipynb
**This is the artifact demonstrating deployment steps.**

Serialised model from the previous step needs to be deserialised using pickle library on production servers.

It is a prerequisite for the runtime environment to contain pickle library, use the below command to install it.
> !pip install pickle


### models/DecisionTreeRegressor_GridSearchCV.sav
This is the output model based on GridSearchCV


### models/DecisionTreeRegressor_RandomizedSearchCV.sav
This is the output model based on RandomizedSearchCV
