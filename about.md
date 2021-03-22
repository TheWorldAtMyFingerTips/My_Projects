# Python

### Introduction
Python was the final *language* in the curriculum. We had started off with the basics (of data types, flow control, functions, dictionaries, classes, etc.), learnt how to automate repetitive tasks, data analytics, create dashboards, and build machine learning models (of linear regression, k-nearest neighbours, support vector machines, random forests, neural networks, deep learning with Keras and TensorFlow, etc).

### Capstone Project: Build Machine Learning Models for the Instagram Top Post Dataset

#### Abstract
In today's society, smartphones have become ubiquitious and an essential tool for most of us. Especially with the lockdown of COVID-19, humans have increasingly turned to social media platforms to get their daily fixes of interaction. Instagram is one of the most-used social platforms today, with a concept built around image and video sharing. While the app started off based on personal interactions, it has now evolved to encompass business-to-consumer interactions, making the landscape increasingly competitive and thus, imperative to capture customers' attention by having their content as one of the top posts.

This project aims to better understand Instagram's algorithm and, from a user-standpoint - find out which are the "super" variables to focus efforts on in the trajectory to making Instagram top posts.

###### Top Posts in the Explore and Home tabs
![What is an Instagram Top Post](https://github.com/TheWorldAtMyFingerTips/My_Projects/blob/main/images/What%20is%20an%20Insta%20Top%20Post.png)


#### Dataset Introduction
The [Instagram Top Post Dataset](https://www.kaggle.com/rezaunderfit/instagram-top-post) consists of 16 independent variables (of "like_count", "hashtag_count", "is_verified", "is_video", etc.) with a target column of "is_top". It is a balanced dataset which contains a total of 2170 entries, with 1099 top posts and 1071 not top posts.

#### Problem Statement
Which variables hold higher weightage in making a post come up on top? This project uses Machine Learning Models of `Logistic Regression` and `Random Forest` in sifting out the "super" variables.


#### Results
Based on the F1 Score for both models, I had decided that `Random Forest` was the best model to 
