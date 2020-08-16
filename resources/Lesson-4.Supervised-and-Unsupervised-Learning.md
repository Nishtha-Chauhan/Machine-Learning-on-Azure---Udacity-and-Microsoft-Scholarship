# Lesson - 4. Supervised and Unsupervised Learning

## Supervised Learning
Task of learning a function from data that contains both input and expected output. Types - 
- Classification: Outputs are categorical. *Examples*: Computer Vision, Speech Recognition, Biometric Identification, Document Classification 
![2-class classification](/images/img9.PNG)
- Regression: Outputs are continuous and numerical. *Examples*: Housing prices, Customer lifetime value, Forecasting(time-series), Anomaly Detection. **Algorithms**: Linear Regression, Decision Forest Regression, Neural Network Regression 
- Similarity Learning: Learns from examples using similarity function that measures how similar two objects are
- Feature Learning: Learns to automatically discover the representation/features from raw data
- Abnomaly Detection: Learns from data labeled as normal/abnormal

### Multi-Class Classification Algorithms
1. Multi class Logistic Regression Algorithm - It is used to predict the probability of an outcome, used for classification task. Two parameters used to configure this algorithms are - 
- Optimization Technique
- Regularization Weight 
2. Multi class Neural Network - Three parameters used to configure this algorithm are - 
- Number of hidden nodes 
- Learning Rate
- Number of learning iteration
3. Multi class Decision Forest - It is the ensemble of D-Trees. Five key parameters to configure this algorithm - 
- Resampling Method
- Number of D-Trees
- Maximum depth of D-Trees
- Number of random splits/node
- Minimum number of samples/leaf node
![multi-class classification algorithms](/images/img10.PNG)


## Automated Machine Learning 
Intelligently test multiple algorithms and hyper-parameters in parallel and returns the best one. 
![auto ML](/images/img11.PNG)


## Unsupervised Learning
Task of learning a function from data that contains only inputs and find hidden structure in data. Types - 
- Clustering: Assigns entities to clusters/groups
- Feature Learning: Features are learned from unlabeled data
- Abnomaly Detection: Learns from unlabeled data, using assumption that the majority of entities are normal
- **Algorithms**: Clustering, Feature Learning, Neural Networks, Principa Component Analysis (PCA)


## Semi-Supervised Learning
It combines supervised and unsupervised approaches; involving small amounts of labeled data and large amount of unlabeled data. 
- Approaches:- 
  - Self Training: Trains the model using labeled data and then, uses it to make predictions for unlabeled data. The end result is a dataset that is fully labeled and can be used in supervised learning approach 
  - Multi-view Training: Train multiple models on different views of data that includes various features selection, parts of training data/various model architectures
  - Self-Ensemble Training: It is similar to multi-view training except, one uses a single base model and different hyper-parameter settings
  
  
## Clustering 
It involves the problem of organizing entities from input data into a finite number of subsets/clusters ; goal is to maximize both intra-cluster similarity and inter-cluster differences
- Applications: 
1. Personalization and target marketing 
2. Document classification
3. Fraud Detection
4. Medical Imaging
- Types: 
  - Centroid-based Clustering 
  - Density based Clustering
  - Distribution based Clustering
  - Hierarchical Clustering


## K-Means Clustering 
- Centroid based clusters
- Locates upto a target(k) number of cluster, grouping similar members
- *Objective*: To minimize intra-cluster distances 
![k-means](/images/img12.PNG)


## Reinforcement Learning
Task of learning how an agent should take action in an environment to maximize a reward function.
- Markov D-Tree: Mathematical process to model decision-making in situations where outcomes are partly random and partly under the control of a decision-maker. 
