# Lesson - 6.Managed Services for Machine Learning

## Types of Computing Resources available through managed services
1. Training Compute 
2. Inferencing Compute
3. Notebook Environment


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
![notebook paradigm](/images/img21.PNG)


## Basic Modelling
1. *Experiment*: Generic content for handling runs
2. *Runs*: Used to build the trained model
3. *Model Registry*: Once the model is trained, it keeps a track of all the models in an Azure ML Environment 
4. *Models*:
   - Run is used to produce a model
   - It's a piece of code that takes an input and produces output
   - Training is an "iterative process" 
   ```
   Model = Algorithm + Data + Hyperparameters
   ```
   - They are identified by name and version
   
   
## Advanced Modelling






