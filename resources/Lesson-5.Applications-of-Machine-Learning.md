# Lesson - 5. Applications of Machine Learning 

## Deep Learning
Deep Learning Algorithms are a special case of ML algorithms and have the capability of learning a accurately complex, non-linear functions from the data.

![deep learning](/images/img13.PNG)

*Characteristics* - 
- Highly effective in learning multi-dimensional, non-linear functions
- Massive amount of training data
- Excels with raw, unstructured data
- Automatic feature extraction
- Computationally expensive

*Benefits* - 
1. Non-parametric approach taken by neural nets allow them to learn arbitrally complex functions
2. Learn complex patterns without explicitly seeing them
3. Effective across various types of data
4. Work on very large sets of data
5. Can be distributed for parallel training 
6. Learn time-related patterns
7. Capable of reaching on-par performance with certain human activities

*Applications* - 

![deep learning applications](/images/img15.PNG)


## Similarity Learning
### Classification Approach 
Similarity function maps pairs of entitiies to a finite number of similarity level

### Regression Approach
Similarity function maps pairs of entities to numerical values

### Ranking Similarity Approach 
A variation of this approach where supervision form is weakened from an exact measure to an ordering measure
![approaches for recommenders system](/images/img20.PNG)


## Text Classification
**Text Embedding**: It requires text to be translated in some kind of numerical representation. Types - 
1. Word Embedding and Sentence Embedding
2. Scoring 
![classification from text](/images/img19.PNG)


## Feature Learning
Also called as representation learning, it is a part of feature engineering used to derive new features in ones dataset. Approaches -
- *Supervised*:
  - Datasets that have multiple categorical features with high cardinality
  - Image Classification
- *Unsupervised*:
   - Principal Component Analysis (PCA)
   - Independent Component Analysis
   - Autoencoders
   - Matrix Factorization

*Applications* - 
1. Image Classification
2. Image Search
![image classification with CNN](/images/img17.PNG)
3. Feature Embedding
![image search with autoencoders](/images/img18.PNG)


## Anomaly Detection
It is concerned with finding the data points that deviate significantly from the norm, resulting in a bad behavior.
- *Supervised Approach*: 
   - Binary Classification problem where entities must be classified as normal (or) abnormal
   - These two classes are highly imbalanced
   - Based on using a training dataset that has already been labeled as normal/abnormal
- *Unsupervised*: 
   - Problem of identifying two major groups(clusters) of entities
   - Two classes are highly imbalanced
   - Based on using a training dataset that has no labels available
- *Applications*: 
1. Monitoring
2. Fraud Detection
3. Intrusion Detection
4. Anti-malware Protection
5. Data Preparation
![anomaly detection in machinery maintenance](/images/img14.PNG)


## Forecasting
It deals with the sets which can be ordered in time and it takes the numerical values as the main ones, others are taken to train the model. Algorithms - 
- Auto Regression Integrated Moving Average(ARIMA)
- Multi-variate regression
- Prophet
- Forecast Temporal Convolution Network
- recurrent Neural Network(RNN)
![forecasting](/images/img16.PNG)
