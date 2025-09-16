# Artificial Intelligence and Machine Learning

Tags: #AI #ML #ArtificialIntelligence #MachineLearning

##  3.1 Why is AI and Machine Learning happening not at scale?

Because processing and storage are rapidly becoming faster and cheaper, algorithms are smarter, and the AI ecosystem is larger.

---
## 3.1 AI All Around US

Tags: #Entertainment #Agriculture #Medicine #Retail #Fitness

**AI is changing our day-to-day activities**

**Entertainment**: Classification algorithms can help viewers find videos they will like. Based on a customer's profile, their video rental behavior, and the video rental behavior of other customers with similar demographics, the algorithm predicts which videos a customer is likely to enjoy and makes recommendations to the customer.

**Agriculture**: Farmers use cellphones to provide researchers with images of plan diseases. These images are used in image recognition systems to diagnose plant diseases. Combined with environmental data regression, algorithms predict future disease outbreaks.

**Medicine**: Researchers have developed machine learning model that uses probability to classify breast cancer by examining medical histopathology images. This approach may eventually be capable of detecting cancer sub types and classifying benign and malignant tissue.

**Retail**: Artificial intelligence solutions in some retail stores improve customer engagement through interactive chat programs or Chat bots. Chat bots can be an effective way to communicate with customers. They can answer frequently asked questions, recommend products, address grievances, collect valuable customer data, and divert calls to a human telesales executive if needed. They can also be programmed to self-learn from past data to keep refining and personalize subsequent customer interactions.

**Fitness**: The fitness app on your smartphones, or fitness tracker, collects data fed into an application that can provide you with valuable health information. Apps must build a model of your movements to identify what constitutes taking a step and the distance you cover with each one. Some fitness trackers are even using self-learning AI software that can recognize and adapt to a wide variety of movements and can learn new fitness activities based on repetitive, cyclical patterns.

---
## 3.2 Big Data and Machine Learning

Tags: #MachineLearning #BigData #ML #MachineLearningAnalysis #Classifiers #Algorithms

### What is Machine Learning?

Traditionally, computers solve problems through programs or instructions given to them by a human. Machine Learning just means the computer can figure out a solution without being specifically programmed. These machines have the ability to continuously learn by looking at data and finding patterns, and they do this much faster than a human could. 

**Two Key Terms in Machine Learning:**
1. **Classifiers:** the workhorse of machine learning that categorize observations.
2. **Algorithms**: are the techniques that organize and orient classifiers. 

## Types of Machine Learning Analysis

Tags: #Supervised #Unsupervised #Reinforcement 

Machine learning is divided into three primary learning model approaches: **Supervised, Unsupervised, and Reinforcement**. 

**Supervised Machine Learning** algorithms are the most commonly used for predictive analytics. It requires human interaction to label data read for accurate supervised learning. In this model, the model is taught by example using input and output data sets processed by human experts, usually data scientists. The model learns the relationships between input and output data and then uses that information to formulate predictions based on new datasets.

**Unsupervised Machine Learning** algorithms do not require human experts bu autonomously discover patterns in data. Unsupervised learning mainly deals with unlabeled data. The model must work on its own to find patterns and information. 

***Examples of problems solved with unsupervised methods:***

* **Clustering methods** - is the grouping of data that have similar characteristics. It helps segment data into groups and analyzes each to find patterns. 
* **Association methods** - consists of discovering groups of items frequently observed together. Online retailers use associations to suggest additional purchases to a user based on the content of their shopping cart.

**Reinforcement Machine Learning** teaches the machine through trial and error using feedback from its actions and experiences, also known as learning from mistakes. It involves assigning positive values to desired outcomes and negative values to undesired effects. The results is optimal solutions; the system learns to avoid adverse outcomes and seek the positive. Practical applications of reinforcement learning include building ratification intelligence for playing video games and robotics and industrial automation.

---
## The Machine Learning Process

Tags: 

Developing a machine learning solutions is not always a linear process. Several trial-and-error steps are necessary to fine-tune the solution. Here are the steps in the process of machine learning.

**Step 1. Data Preparation:** Perform data cleaning procedures such as transformation into a structures format and removing missing data and noisy/corrupted observations.

**Step 2a. Learning Data**: Create a learning data set used to train the model.

**Step 2b. Testing Data**: Create a test dataset used to evaluate the model performance. (Only perform this step in the case of supervised learning)

**Step 3. Learning Process Loop - Selection**: An algorithm is chosen based on the problem. Depending on the selected algorithm, additional pre-processing steps might be necessary.

**Step 4. Learning Process Loop - Evaluation**: This selected algorithm's performance is evaluated on the learning data. If the algorithm and the model reach an acceptable performance on learning data, the solution validates the test data. Otherwise, repeat the learning process with a proposed new model and algorithm.

**Step 5. Model Evaluation**: Test the solution on the test data. The performance on learning data are not necessarily transferrable to test data. The more complex and fine-tuned the model is, the higher the chances are that the model will become prone to over fitting, which means it cannot perform accurately against unseen data. **Overfitting** can result in going back to the model learning process.

**Step 6. Model Implementation**: After the model achieves satisfactory performance on test data, implement the model. **Implementing the model** means performing the necessary tasks to scale the machine learning solution to big data.

![[Pasted image 20250916092200.png]]

---
## Training Machines to Recognize Patterns

Tags: #MachineLearning #Training #ArtificialIntelligence  #AI #ML

***Machine Learning is a subset of artificial Intelligence***. 

**Artificial Intelligence** is the concept that a system can learn from data, identify patterns, and make decisions with little or no human intervention. 

**Machine Learning** has many valuable applications in the field of data analytics. One application is pattern recognition.

**Pattern Recognition** utilizes machine learning algorithms to identify patterns in digital data. These patterns are then applied to different datasets with the goal of recognizing the same or similar patterns in the new data. 

**Pattern Recognition** uses the concept of learning to classify data based on statistical information gained from patterns and their representations. Learning enables the pattern recognition systems to be "trained" and adaptable to provide more accurate results. 

***The training data set is used to build the model and consists of about 80% of the data.***

***The testing data set consists of about 20% of the data and measures the model's accuracy.***

![[Pasted image 20250916093356.png]]

Pattern recognition algorithms can be applied to different types of digital data, including images, texts, or videos, and can be used to automate and solve complicated analytical problems fully. Examples:

1. Mobile Security: Identifying fingerprints or facial recognition to gain access to a smartphone
2. Engineering: Speech recognition by digital assistant system such as Alexa, Google Assistant, and Siri. 
3. Geology: Detecting specific types of rocks and minerals and interpreting temporal patterns in seismic array recordings.
4. Biomedical: Using biometric patterns to identify tumor and cancer cells in the body.

---
## What Did I Learn in This Module?

**Topic Objective:** Explain the concept of AI

AI uses computer systems to perform tasks that formerly required human intelligence. AI completes processes more efficiently and effectively. AI impacts numerous aspects of our lives, such as marketing, blogging, healthcare, agriculture, retail experiences, and fitness.

**Topic Objective**: Explain how big data enables machine learning.

Machine learning is a subset of artificial intelligence based on the concept that a system can learn from data, identify patterns, and make decisions with little or no human intervention. Machine learning is comprised of both classifiers and algorithms. Classifiers categorize operations, while algorithms are the techniques that organize and orient classifiers.

Machine learning is divided into three primary learning model approaches: Supervised, Unsupervised, and Reinforced.

A machine learning solution includes: 

* Step 1 - Data Preparation
* Step 2a - Learning Data
* Step 2b - Testing Data
* Step 3 and 4 - Learning Process Loop (Selection and Evaluation)
* Step 5 - Model Evaluation
* Step 6 - Model Implementation

