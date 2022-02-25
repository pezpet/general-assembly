# Project 5 - US Census from 1900

Table 33: FOREIGN BORN POPULATION, DISTRIBUTED ACCORDING TO COUNTRY OF BIRTH, BY STATES AND TERRITORIES: 1900

## Problem Statement

Is the foreign born population of each state in 1900 predictive of the state's most common household language (ex. English and Spanish) in 2019?

## Description of the data

### 1900 Census Data
Stacker Media has collected a data set from the 1900 US Census, cleaned it and made it available as a .csv file through GitHub.

From [Stacker](https://blog.stacker.com/stackers-first-data-drop-immigrant-populations-of-1900/): 
>"We chose Table 33 of the 1900 U.S. Census as our first dataset, which details the countries of origin for immigrant populations in all 50 states, Washington D.C., and one territory: a total of 10,460,085 individuals. Previously inaccessible due to the poor quality of the PDF, the dataset is now publicly available and can be used to explore how statewide communities have evolved since the turn of the 20th century.
Stacker staff transcribed the data by first uploading the PDF from the U.S. Census Bureau to pdftoexcel.com. This yielded an easy-to-read tabular dataset, but still had gaps where the original file was simply illegible to computers. The base transcription was reformatted, corrected, and checked by hand, resulting in a clean CSV as the final product."

This data is collected for our project from [Stacker's GitHub](https://github.com/stacker-media/data/blob/main/1900-census-immigrant-state/1900-census-immigrant-pop-state.csv).

### Household Languages Data
This data was manually collected from [this Migration Policy Institute article](https://www.migrationpolicy.org/article/frequently-requested-statistics-immigrants-and-immigration-united-states-2020#demographic-educational-linguistic) which is based on the US Census Bureau 2019 American Community Survey.

[This map](./images/Lang_map_.png) summarizes the relevant data used for common languages by state.

## Models

Classification models used in this project and their testing accuracy:

1. Baseline -> 32.69% Accuracy
1. Logistic Regression -> 30.77%
1. Decision Tree -> 7.69%
1. Random Forest -> 46.15%

## Conclusions and Recomendations

We find that our Random Forest classification model outperforms the baseline and can predict most common household language from our data.