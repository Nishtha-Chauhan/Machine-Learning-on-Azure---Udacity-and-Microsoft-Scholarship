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
   - More approiate features for some algorithms
- *Reasons for feature engineering*
   - 
   
   
   
   
   
   
   
   
