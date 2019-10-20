
Mercedes-Benz Greener Manufacturing

Since the first automobile, the Benz Patent Motor Car in 1886, Mercedes-Benz has stood for important automotive innovations. These include, for example, the passenger safety cell with crumple zone, the airbag and intelligent assistance systems. Mercedes-Benz applies for nearly 2000 patents per year, making the brand the European leader among premium car makers. Daimler’s Mercedes-Benz cars are leaders in the premium car industry. With a huge selection of features and options, customers can choose the customized Mercedes-Benz of their dreams.
To ensure the safety and reliability of each and every unique car configuration before they hit the road, Daimler’s engineers have developed a robust testing system. But, optimizing the speed of their testing system for so many possible feature combinations are complex and time-consuming without a powerful algorithmic approach. As one of the world’s biggest manufacturers of premium cars, safety and efficiency are paramount on Daimler’s production lines.


Attribute information
This dataset contains an anonymized set of variables (X0 to X385), each representing a custom feature in a Mercedes car. 
** Note: This is confidential data and we will not be able to provide description for each of the anonymized set of variables.
For example, a variable could be 4WD, added air suspension, or a head-up display.
The ground truth is labeled ‘y’ and represents the time (in seconds) that the car took to pass testing for each variable.
File descriptions
Variables with letters are categorical. Variables with 0/1 are binary values.
●	train.csv - the training set
Objective: 
Tackle the curse of dimensionality (Use PCA for dimensionality reduction) and then Predict the time it takes to pass testing for cars.


Notebook contains:
1] Exploratory Visualization  – covered in notebook
2] Data Cleaning  – covered in notebook
3] Feature Engineering - Converted some categorical features into numeric values using LabelEncoder
4] Modelling & Evaluation - choose 13 models and use 5-folds cross-validation to evaluate (LinearRegression,Ridge,Lasso,RandomForestRegressor,GradientBoostingRegressor,SVR,LinearSVR,ElasticNet,SGDRegressor,BayesianRidge,KernelRidge,ExtraTreesRegressor,XGBRegressor,LassoLarsCV) models
5] Ensemble Methods - Average base models according to their weights, picked 6 best R-score models from point [4]
6] Stacking Technique - Combine information from multiple predictive models to generate a new model. Often times the stacked model (also called 2nd-level model) will outperform each of the individual models due its smoothing nature and ability to highlight each base model where it performs best and discredit each base model where it performs poorly. Also, I have combine features generated from stacking and original features.
7] Improve score using dimensionality reduction and Stacking technique
8] Apply kernel to Kaggle data - Final score was 0.56784 and rank is 1061 as per public score


