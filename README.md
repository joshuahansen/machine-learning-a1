# machine-learning-A1

# COSC 2673 Machine Learning

# Assignment 1

# Introductory Machine Learning

### Learning outcomes:
* Develop familiarity with solving a machine learning task on a real dataset
* Practice loading and analysing the data
* Practice setting up evaluation framework to compare different approaches
* Develop written communication skills to describe approach taken,  
  explaining the reasoning for it and present results to justify the choices.

### Introduction

In this assignment, you’ll apply machine learning techniques and approaches to a regression  
problem. The assignment is aimed to develop your familiarity with applying machine learning  
techniques to learning problems, and to participate in a Kaggle in-class competition to compete with  
your class mates and get bragging rights (and bonus marks).  

### Task

Prediction is an important aspect of machine learning and data science in general. For this  
assignment, you’ll be predicting the cancer death rate of some local regions in the US. The dataset  
consists of a number of features relating to the demographics of these regions, and the task is to use  
these to train a regression approach to predict the cancer death rate on test and unseen data.  
You will also setup the evaluation framework, including selecting appropriate performance  
measures and determining how to split the data into training and testing.  
As one of the aims of the assignment is to get you familiar with the machine learning paradigm, you  
should also evaluate a few different regression algorithms to determine which one would be most  
appropriate to predict the death rates.  


### Data

The data is available as part of the assignment download (see Canvas). We have cleaned it up for  
you, such that all the attributes/features are integers or floats, and missing values has been estimated  
and filled in. There are the following files:

* train.csv, contains the training dataset. Use this for both training your Kaggle submission and for  
  your own exploration and evaluation of which approach you think is “best” for this prediction task.
* test.csv, containts the testing dataset for the Kaggle competition. It has all the independent features  
  but not the dependent one (TARGET_deathRate). For Kaggle, you predict the values for the unknown  
  TARGET_deathRate and submit them. There will be more details about this within the Kaggle competition page.  
  For your own evaluation etc, this file may be useful for exploring the features.
* The file metadata.csv contains some brief description of each of the fields.
   
The original data is from https://data.world/nrippner/ols-regression-challenge, and the data we  
provided is based on this, with some perturbation. Online, there are one or two scripts and kernels  
available for this dataset and have found the target feature is strongly correlated with several  
independent features. As the aim of this assignment is to encourage you to learn to setup evaluation  
and explore different approaches, your attempted approaches must not explicitly perform feature  
selection, i.e., your learning models should have all features as input.  


### Kaggle in-class Competition

In addition to doing your own evaluations (strongly recommended), we would like you to enter the  
Kaggle in-class competition we have setup for this.  
The location of the competition will be released with about 2 weeks to go, as we wish you to first  
explore with your own code before entering Kaggle, which can be dangerous for beginning machine  
learning students (real machine learning is not about optimising ones model to fit the test data,  
which is what sometimes Kaggle competitions boils down to). However, we do want you to  
explore and we are using Kaggle as an extra incentive for that.  
The top 3 submissions will have bonus marks given to the individuals – 5 bonus marks for first, 3  
bonus marks for second and 1 bonus mark for third.  
To be able to evaluate this properly, we need you to use an account name that either is your full  
name or your student number. If you have a Kaggle account already and it isn’t one of the above,  
please create a new one for this in-class competition. If you haven’t got one, please create one, and  
hopefully this in-class competition will introduce you to the interesting and exciting competitions  
that occur on Kaggle.  
Once created, log onto Kaggle and provided URL (to be provided, as described above). Within  
Kaggle there are more details, but essentially you will be predicting the unknown values for  
test.csv, and your position on the leader board will be based on how well you perform. There is a  
limit of 2 submissions per day, as we want to encourage you to develop off-line and do your own  
evaluation first before submitting periodically to Kaggle.  


### Report

In addition to the Kaggle in-class competition, part of your assessment is based on a (up to) 7 A4  
page report, at least in font size 12. In this report you’ll describe your final selected approach, why  
you selected this approach, parameter settings and some other regression approaches you have tried.  
This will allow us to understand your rationale, but also encourage exploration and not just focused  
on maximising a single performance metric (i.e., the Kaggle in-class).   


### Getting Started

To help you get started, we suggest the following:

* Load dataset into your Jupyter or your favourite Python IDE
* Do some preliminary data exploration, to understand it better (this will help you later on with  
  trying to figure which regression approach is ideal and how to improve it)
* Setup your data into training and testing datasets
* Select the basic linear regression algorithm and train it then evaluate it
* Analyse the results and see what is going on (to help you determine what needs to be changed  
  to improve the regression model)