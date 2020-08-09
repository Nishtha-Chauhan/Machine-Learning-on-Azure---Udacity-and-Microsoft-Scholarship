# Lesson - 3. Model Training

## Data Wrangling
It is the process of cleaning and transforming data to make it appropriate for analysis steps involved - 
1. Explore raw data and check general quality of dataset
2. Transform the raw data, by restructuring, normalizing and cleaning the data
3. Validate and publish the data
4. **It is an ITERATIVE PROCESS**


## Data Management Tools by Azure Machine Learning
- **Datastore**: It offers a layer of abstraction over supported Azure storage services
    - They store all information needed to connect to a particular storage service
    - Provides an access mechanism that is independent of compute resources that is used to drive a ML process
    - *Example*: Azure Blob Container, Azure File Share, Azure Data Cake, Azure SQL Database
    - **Versioning** is done when new data is available for retraining or different approaches are applied to data preparation/feature engineering
 
- **Dataset**: It consists of the resources for exploring, transforming, and managing data in Azure ML
    - A reference that points to data in storage
    - Used to get specific data files in datastores
    - Azure ML Workspace supports 2 types of dataset:
    1. Tabular Dataset
    2. Web URL
    
 
## Steps of Data Access Workflow
1. Create a datastore, to access storage services in Azure
2. Create a dataset, used for model training in ML experiments
3. Create a dataset monitor, to detect issues in data such as data drift 
![Data Access Workflow steps](/images/img5.PNG)


## Feature Engineering
It is used to drive new features based on values of existing features. It improves model training and is applied on numbers, text, and images. Tasks involved in feature engineering - 
- Aggregation 
- Part-of
- Binning: Grouping the items into bins and then applying aggregation 
- Flagging: Boolean value operations
- Frequency-Based
- Embedding 
- *Benefits* 
   - Improves model accuracy
   - More appropriate features for some algorithms
   
**Feature Selection**: It is the process of selection of most important features
- Reasons for feature selection -  
   - Elimination of irrelevant, redundant or highly correlated features
   - Reduction of dimensionality to increase performance 
- Azure ML modules for feature selection -
   - Filter Based Feature Selection
   - Permutation Feature Importance 
   
**Dimensionality Reduction**: It is used to decrease the number of features. Techniques -
1. Principal Component Analysis(PCA) 
2. t-SNE
3. Feature Embedding


## Data Drift 
It is the change in input data for the model. It causes degredation in model performance over time so, data monitors are used to alert one about data drift and even take automatic actions to correct data drift. Process of monitoring for data drift involves - 
- Specifying baseline dataset
- Specifying target dataset
- Comparing these two dataset over time, to monitor for differences
![data drift examples](/images/img7.PNG)


## Data Science Process
![data science lifecycle](/images/img6.png)

**Hyperparameters**: Some model parameters not learnt from data and their values are set before training, example:-
1. Number of layers in deep neural network  
2. Number of clusters 
3. Learning rate of model

**Splitting the data** into three parts - 
- *Training data* - to learn the values for parameters
- *Validation Data* - used to check model's performance on the data and tune hyperparameters until model performs well with the data
- *Test Data* - used to do a final check of model performance
   
   
## Classification
Outputs are categorical or discrete. 3 main types include - 
1. Binary Classification *Example*: Anamoly/Fraud Detection
2. Multi-class Single lable Classification *Example*: Recognition of written number
3. Multi-class Multi lable Classification *Example*: Text Tagging

*Example*:Classification Algorithms - 
- Logistic Regression
- Support Vector Machine(SVM)


## Regression
Output is numerical or continuous. 2 types of regression - 
1. Regression to arbitrary values
2. Regression to values between 0 and 1

*Example*:Regression Algorithms -
- Linear Regressor
- Decision Forest Regressor


## Confusion Matrics
![confusion matrix](/images/img8.PNG)

**Evaluation Metrics for Classification**
```
1. Accuracy = (TP + TN)/(TP + TN + FP + FN)

2. Precision = TP/(TP + FP)

3.Recall = TP/(TP + FN)

4. F-Score = 2X[(P X R)/(P + R)]
```

**Model Evaluation Charts for Classification**
- *Receiver Operating Characteristics(ROC) Chart*: Shows the rate of TP against the rate of FP
- *Gain and Lift Chart*: It deals with rank ordering the prediction probabilities and they measure how much better one is expected to perform by using classifier as opposed to random guessing


## Model Evaluation Metrics for Regression 
1. Root Mean Square Error(RMSE): Average of square difference between predictions and true values
2. Mean Absolute Error(MAE): Measures the absolute difference between each prediction and the true value
3. R-Squared: Coefficient of measurement to measure how close the values on the fitted regression line are on the predicted values
4. Spearman Correlation: Used to measure the strength and the direction of correleation, 
   the relation between the predicted values and the true values
   
**Model Evaluation chart for Regression** 
- Predicted v/s True Value
- Histogram of Residuals


## Ensemble Learning 
It combines multiple ML models to produce one predictive model. Three types: 
1. Bagging/Bootstrap Aggregation 
   - helps reduce variance 
   - homogeneous learners
   - random sampling with replacement 
   - equally weighted average

2. Boosting 
   - weak, homogeneous learner 
   - reduce bias
   - sequential learning 
   - weighted average prediction
   
3. Stacking 
   - hetrogeneous learner
   - meta model that learns to combine prediction from base learners
   - improves prediction accuracy

## Automated Machine Learning 
It automates many of the iterative, time-consuming tasks involved in model development. It also allows data scientists, analyst and developers to build models with: greater scale, efficiency, productivity while sustaining model quality.
