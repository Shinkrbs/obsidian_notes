Tags: #MachineLearning #IntelligentSystems

## Introduction

**Machine Learning**
1. Gives Computers the ability to learn without being explicitly programmed
2. A computer program that is said to learn from experience **E** with respect to some task **T** and some performance measure **P**, if its performance on **T**, as measured in **P**, improves with experience **E**.

![[Pasted image 20251125234507.png]]

*Examples of Machine Learning*:
1. Recognizing Patterns
2. Generating Patterns
3. Recognizing Anomalies
4. Prediction

*Examples of Applications of Machine Learning:*
1. Web Search 
2. Computational Biology
3. Finance
4. E-commerce
5. Space Exploration
6. Robotics
7. Information Extraction Social Networks
8. Debugging Software

## Classifications Based on Goal, Tasks, Target Function

**Prediction**: system predicts the desired output for a given input based on previous input/output pairs

*Examples:*
- prediction of stock values given other (input) parameters values (market index, interest rates, currency conversion, etc.).

**Regression**: system estimates a function of many variables (*multivariate*) or single variable (*univariate*) from scattered data.

*Examples:*
- prediction of stock values given other (input) parameters values (market index, interest rates, currency conversion, etc.).

**Classification (Categorization)**: system classifies an object into one of several categories (or classes) based on features of the object. 

*Examples*:
- Diagnosis System which has to classify a patient's cancer tumor into one of the three categories: avascular, vascular, angiogenesis.

**Clustering**: system task is to organize a group of objects into homogeneous segments.

*Example*: satellite image analysis system which groups land areas into forest, urban and water body, for better utilization of natural resources.

**Planning**: system has to generate an optimal sequence of actions to solve a particular problem. 

*Example:* 
- Robot path planning.

## Classification Based on the Model

1. Decision Trees
2. Linear Separators (Perceptron Model)
3. Neural Networks
4. Genetic Programming
5. Evolutionary Algorithms
6. Graphical Models
7. Support Vectors Machines
8. Hidden Markov Models

**Classification Based on Experience:**
1. Supervised (*inductive*) Learning
	- Given: Training Data + Desired Outputs (labels)
2. Unsupervised Learning
	- Given: Training Data (Without Desired Outputs)
3. Semi-supervised Learning
	- Given: Training Data + a few desired output
4. Reinforcement Learning
	- Rewards from sequence of actions

**Supervised Learning:** the machine is given the desired outputs and its goal is to learn to produce the correct output given a new input.
- deals with learning a function from available training data.

*Challenges in Supervised Machine Learning*:
1. Irrelevant input feature present training data could give inaccurate results
2. Data preparation and pre-processing is always a challenge
3. Accuracy suffers when impossible, unlikely, and incomplete values have been inputted as training data.
4. If the concerned expert is not available, then the other approach is "brute-force". It means you need to think that the right features (input variables) to train the machine on. It could be inaccurate.

*Disadvantages of Supervised Machine Learning*:
1. Decision boundary might be over trained if your training set which doesn't have examples that you want to have in class.
2. You need to select lots of good examples from each class while you are training the classifier.
3. Classifying big data can be a real challenge.
4. Training for supervised learning needs a lot of computation time.

*Best Practices for Supervised Machine Learning*:
1. Before doing anything else, you need to decide what kind of data is to be used as a training set.
2. You need to decide the structure of the learned function and learning algorithm.
3. Gather corresponding outputs either from human experts or from measurements.

**Unsupervised Learning**: The goal of the machine is to build a model of input that can be used for reasoning, decision making, predicting things, and communicating. 
- Makes sense of unlabeled data without having any predefined dataset for its training.
- an extremely powerful tool for analyzing available data and look for patterns and trends. It is most commonly used for clustering similar inputs into logical groups

*Prime reasons for using unsupervised learning*:
1. finds all kind of unknown patterns in data
2. Help you find features which can be useful for categorization 
3. Taken place in real time, so all the input data to be analyzed and labeled in the presence of learners.
4. Is easier to get unlabeled data from a computer than labeled data, which needs manual interventions.

*Applications of Unsupervised Machine Learning*:
1. Clustering automatically split the dataset into groups base on their similarities
2. Anomaly detection can discover unusual data points in your dataset. It is useful for finding fraudulent transactions.
3. Association mining identifies sets of items which often occurs together in your dataset.
4. Latent variable models are widely used for data pre-processing. Like reducing the number of features in a dataset or decomposing the dataset into multiple components.

*Disadvantages of Unsupervised Machine Learning*:
1. Cannot get precise information regarding data sorting, and the output as data used in unsupervised learning is labeled and not known.
2. Less accuracy of the results is because the input data is not known and not labeled by people in advance. This means the machine requires to do this itself.
3. The spectral classes do not always correspond to informational classes.
4. The user needs to spend time interpreting and label the classes which 