# Lesson-2.What is Machine Learning?

## Machine Learning 
Data science technique used to extract patterns from data, allowing computers to identify related data and forecast future outcomes, behaviours and trends.
```
Rules   + Data = Traditional Programming      
Answers + Data = Machine Learning
```


## Applications of Machine Learning 
1. Natural Language Processing 
   - Text: Summarization, Topic Detection, Similarity and Search 
   - Speech: Speech to Text, Text to Speech and Translation
2. Computer Vision 
   - Self Driving Cars
   - Object Detection 
   - Object Identification
   - LIDAR and Visible Spectrum
3. Analytics 
   - **Regression**, **Classification**, Forecasting
   - **Clusering**
4. Decision Making 
   - Sequential decision making problems
   - Recommendations


## Examples of Machine Learning 
- Automating recognition of disease
- Recommend next best actions for individual care plans 
- Enabling personalized, real-time banking experience with chatbots
- Identify the next best action for customers
- Capture, prioritize and route service requests to correct employee to improve response times


## Scaling Data
It is the process of transforming the vector(simple arrays of numbers) so that the values fit within some range(or)scale. It consists of two approaches - 
### **Standardization**
Rescaling the data such that the mean = 0 and variance = 1
```
(x - μ ) / σ
```

### **Normalization**
Rescaling the data into the range [0,1]
```
(x - xmin ) / (xmax - xmin) 
```

## Encoding Categorical Data 
1. Ordinal Encoding: It converts the categorical data into integer codes ranging from 0 to (number of categories - 1). **Drawback**:  It implicitly assumes an order across categories
2. 1-Hot Encoding: Transforms each categorical value into a column. If an item belongs to a category then the cell is assigned a value of 1 otherwise, it represents 0. **Drawback**: It can potentially generate a very large number of columns


## Image Data
It is described as height X width X channels value (Red-Green-Blue data). The color of each pixel is represented with a set of values:-
- Greyscale Image: Each pixel can be represented by a single number which ranges from 0 to 255. This value determines how dark the pixel appears.
- Coloured Images: Each pixel can be represented by a vector of 3 numbers, each ranging from 0 to 255 for 3 primary channels

### Encoding an image
It requires 3 features - horizontal position of each pixel, vertical position of each pixel and color of each pixel. Preprocessing operations to clean the input images include rotation, cropping, resizing, denoising and centering the image.


## Text Data
Data type that is initially non-numerical and must be processed before it can be fed into ML algorithms. 

### Normalization 
Process of transforming a piece of text into a canonical form, example:*Lemmatization* which reduces multiple inflections to single dictionary form

### Tokenization 
Removal of stop words with high frequency that are unnecessary during the data analysis

### Vectorization 
It identifies the particular features of the text that are relevant for a particular task to be performed and then get those features extracted in a numerical form that is accessible to ML algorithm. Common approaches: 
- Term Frequency - Inverse Document Frequency (TF-IDF) vectorization
- Word Embedding 


## Perspective on Machine Learning 
1. Computer Science - Uses input features to create a program that generates desired output
```
Output = Program(Input Features)
```
2. Statistical Terminology - Finds a mathematical function that, given the values of the independent variables can predict the values of dependent variables 
```
Output variable = f(Input variable) 
```


## Main components of Machine Learning 
### Libraries
Collection of pre-written code that one can make use of in a project
Libraries | Example
--------- | --------
Core Framework and Tools | Python, Pandas, Numpy, Jupyter
Machine Learning and Deep Learning | Spark, TensorFlow, Keras, Pytorch
Visualization | Plotly, Seaborn, Matplotlib

### Dev Environment 
Software application that provides a whole suite of tools designed to help build project, example: Jupyter Notebook, Visual Studio

### Cloud Services 
Services that offers data storage/computing power over internet
#### Core Asset Management
![Core Asset Management](/images/img1.PNG)
#### Resource Management
![Resource Management](/images/img2.PNG)


## Linear Regression












