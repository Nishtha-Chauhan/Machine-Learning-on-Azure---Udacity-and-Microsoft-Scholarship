# Lesson - 6.Managed Services for Machine Learning

## Types of Computing Resources available through managed services
1. Training Compute 
2. Inferencing Compute
3. Notebook Environment

![notebook paradigm](/images/img21.PNG)

## Difference between Conventional Machine Learning Approach and Managed Service Approach
**Conventional Machine Learning Approach** -
- Lengthy installation and setup process
- Expertise to configure network
- Fair amount of troubleshooting

**Managed Service Approach** - 
- Very little setup
- Easy configuration for any needed hardware


## Compute Resources
Compute Target is a designated compute resource/environment where one run training scripts/host ones services deployment. Two types - 
1. Training Compute Target
2. Inferencing Compute Targets

**Computes used for training** - 
- Training Clusters
- Compute Instances
- Local Compute


## Training Clusters
They are used for training and batch inferencing
1. Single/multi-mode cluster
2. Can auto scale each time one submit a run
3. Automate cluster management and job scheduling 
4. Support for both CPU and GPU resources


## Inferencing/Scoring Compute 
*Types* -
- Real time 
- Batch

*STEPS involved*:
   1. After one has trained ones model, its ready to put to work, deploy it to web hosting environment/IoT devices
   2. When one uses a model, it infers things about new data it is given based on its training
   3. *Examples*: Inferencing Cluster, Batch Inferencing


## Notebooks 
- It is made up of one or more cells that allow for the execution of code snippets/commands within those cells
- They store commands and the results of running those commands

![using notebooks for classification](/images/img30.PNG)


## Basic Modelling
1. *Experiment*: Generic content for handling runs
2. *Runs*: Used to build the trained model
3. *Model Registry*: Once the model is trained, it keeps a track of all the models in an Azure ML Environment 

![model registry](/images/img29.PNG)

![example of registering a model](/images/img26.PNG)

4. *Models*:
   - Run is used to produce a model
   - It's a piece of code that takes an input and produces output
   - Training is an "iterative process" 
   ```
   Model = Algorithm + Data + Hyperparameters
   ```
   - They are identified by name and version

![ML Pipeline](/images/img22.PNG)
   
   
## Advanced Modelling
*Process Steps* - 
1. Data Ingestion and preparation 
2. Model building and training
3. Model deployment

![Deploying with Azure ML](/images/img24.PNG)

**MLOps** - Applying DevOps principle to ML pipelines
 - Automate end-to-end ML lifecycle  
 - Monitor ML processes
 - Capture tracebility data
 
 ![MLOps with Azure ML](/images/img28.PNG)

**DevOps** - It is process automation applied to classical aoftware development

![differences between DevOps and MLOps](/images/img25.PNG)
 
 
## Operationalizing Models
*Steps involved in model deployment* - 
1. Get model file
2. Create a scoring script
3. Optionally, create a schema file describing web services input
4. Create a real-time scoring web services
5. Call the web services from your applications
6. Repeat the process each time you re-train the model
 
 
## Real-time inferencing
It involves inferening things about new data based on model training and making decisions on-demand
 
*Options for creating* - 
1. Create manually from Azure ML Studio user interface
2. Create programmatically using code
 
![real-time scoring of python scikit-learn and deep learning models on Azure](/images/img31.PNG)

 
## Batch Inferencing 
It runs on large quantities(batches) of existing data, run on a recurring schedule against data stored in a database
 
*Used when* - 
- No need for real-time
- Inferencing results can be persisted
- Post processing/analysis on prediction is needed
- Inferencing is compiled

![Lambda Architecture](/images/img23.PNG)


## Programmatically accessing Managed Services
Azure ML Services support many of the popular open-source ML and deep learning python packages - 
1. Scikit-Learn 
2. Tensorflow
3. Pytorch
4. Keras

**Key areas of SDK** - 
- Manage datasets
- Organize and monitor experiments
- Model training
- Automated ML
- Model Deployment

![high level architecture of possible deployment](/images/img27.PNG)
