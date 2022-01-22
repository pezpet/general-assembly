# Executive Summary for Project 2
## Problem Statement
The classic Real Estate expression for property prices is: "Location, location, location." In this project we seek to evaluate the merits of this phrase, specifically, if property location is enough information to accurately predict its price.
## Description of data
For this project we have used the Ames Housing dataset:
- NAME: AmesHousing.txt
- TYPE: Population
- SIZE: 2930 observations, 82 variables
- ARTICLE TITLE: Ames Iowa: Alternative to the Boston Housing Data Set

- DESCRIPTIVE ABSTRACT: Data set contains information from the Ames Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010.

- SOURCES: Ames, Iowa Assessor’s Office

- SUBMITTED BY: Dean De Cock, Truman State University, 100 E. Normal St., Kirksville, MO, 63501, decock@truman.edu

The data is split into a training and a testing set, respectively train.csv and test.csv, with the training set used for all model training, and the testing set used to submit predictions to the kaggle competition.

## Conclusions & Recommendations
Allthough our location based models have better RMSEs than our null-baseline model, a straightforward linear regression model that didn't include location features performed better than location only models.

Our recommendation is to incorporate a diverse mix of factors when estimating property prices, including but not limited to location characteristics.