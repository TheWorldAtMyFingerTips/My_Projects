# Python

### Introduction
Python was the final *language* in the curriculum. We had started off with the basics (of data types, flow control, functions, dictionaries, classes, etc.), learnt how to automate repetitive tasks, data analytics, create dashboards, and build machine learning models (of linear regression, k-nearest neighbours, support vector machines, random forests, neural networks, deep learning with Keras and TensorFlow, etc).

### [Capstone Project: Build Machine Learning Models for the Instagram Top Post Dataset](https://github.com/TheWorldAtMyFingerTips/My_Projects/blob/main/python/Instagram%20Top%20Post.ipynb)

### Abstract
In today's society, smartphones have become ubiquitious and an essential tool for most of us. Especially with the lockdown of COVID-19, humans have increasingly turned to social media platforms to get their daily fixes of interaction. Instagram is one of the most-used social platforms today, with a concept built around image and video sharing. While the app started off based on personal interactions, it has now evolved to encompass business-to-consumer interactions, making the landscape increasingly competitive and thus, imperative to capture customers' attention by having their content as one of the top posts.

This project aims to better understand Instagram's algorithm and, from a user-standpoint - find out which are the "super" variables to focus efforts on in the trajectory to making Instagram top posts.

###### Top Posts in the Explore and Home tabs
![What is an Instagram Top Post](https://github.com/TheWorldAtMyFingerTips/My_Projects/blob/main/python/images/What%20is%20an%20Insta%20Top%20Post.png)</br>


### Dataset Introduction
The [Instagram Top Post Dataset](https://www.kaggle.com/rezaunderfit/instagram-top-post) consists of 16 independent variables (of `like_count`, `hashtag_count`, `is_verified`, `is_video`, etc.) with a target column of "is_top". It is a balanced dataset which contains a total of 2170 entries, with 1099 top posts and 1071 not top posts.</br>

### Problem Statement
**Which variables hold higher weightage in making a post come up on top?** This project uses Machine Learning Models of `Logistic Regression` and `Random Forest` in sifting out the "super" variables.</br>

### Process Workflow
The dataset was checked and clean of missing values, datatypes were streamlined into two types (object, and non-object) to enable easy visualizations for the purpose of exploratory data analysis. Data was then pre-processed using label-encoding and one-hot-encoding, and then data was split and model trained. Due to the data being previously categorical and numerical, the range of the encoding was wide and so I scaled the data using `sklearn.preprocessing`'s `StandardScaler`, then fitted it to the training data and applied transformations to the data.

I warmed up by doing a baseline model using Logistic Regression and took note of the F1 Score.

After which I got down to serious business by setting up my Machine_Learning_Model_1 - Logistic Regression, then getting down and dirty with hyperparameter tuning. Using the best hyperparameters and estimators (from my tuning), I fitted them to the training data, predicted with the test data, to obtain the classification report for the model. My Machine_Learning_Model_1 - Logistic Regression F1 Score topped the baseline model. I am happy.

Next, I carried out the same steps with my Machine_Learning_Model_2 - Random Forest. Setup, hyperparameter tuning, ... you get the drift. This new model's F1 Score topped the previous (Machine_Learning_Model_1 - Logistic Regression). With this as my best model, I moved on to predicting and evaluating using my test data.

![ML model comparison](https://github.com/TheWorldAtMyFingerTips/My_Projects/blob/main/python/images/ML%20Models%20Comparison.JPG)</br>

### Results
Fortunately, the model metrics for the test data did not vary significantly (vs the training data). The results look good as well with immaterial FPs and FNs.</br>

###### Results in a Confusion Matrix Visualization
![confusion matrix](https://github.com/TheWorldAtMyFingerTips/My_Projects/blob/main/python/images/Confusion%20Matrix.JPG)

Having plotted the features importance into a visualization, we can deduce that the top "super" variables are `like_count`, `comments_count`, and `followers_count`.

![features importance](https://github.com/TheWorldAtMyFingerTips/My_Projects/blob/main/python/images/Features%20Importance.JPG)

The data-driven approach suggests to focus on creating content which:
* aim to provide instant gratification --> `like_count`
* encourages engagement --> `comments_count`
* is addictive --> `followers`</br></br>


### Contact me
Contact Platform | Contact Address
---------------- | ------------------
LinkedIn | https://www.linkedin.com/in/megan-ng-7708a74/
Email | megan_ng@hotmail.com
