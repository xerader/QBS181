# QBS181 Project

Repository for the final QBS181 project. This project involves data cleaning, imputation, and prediction scripts for heart disease datasets.

## Team Members
- Biratal
- Haoyang
- Kevin
- Rob

## Description
Heart disease is the leading cause of death for men, women, and people of most racial and ethnic groups, accounting for approximately 1 in every 5 deaths in 2022 in the United States (, 702,880 people died from heart disease)
Heart disease cost about $252.2 billion from 2019 to 2020. This includes the cost of healthcare services, medicines, and lost productivity due to death.
From 2009-2019, around 6% prevalence in the total population with men more likely to have disease compared to woman
Prevalence of heart disease increases as you age

![Geography](/Image/geo.png)

### Cleaned Data
Contains cleaned datasets from various sources including Framingham, Kaggle, Mendeley, and UCI.

### Data Cleaning Scripts
Jupyter notebooks for cleaning and processing the datasets:
- `MergingDF.ipynb`: Script for merging dataframes.
- `Processing_UCI.ipynb`: Script for processing the UCI heart disease dataset.

### Data Dictionary
Contains data dictionaries for the datasets used:
- `Framingham_DD.csv`
- `Mendeley_dataset.csv`
- `Mendeley1_DD.csv`
- `UCI_DD.csv`

### Imputed Data Algorithms
Scripts for data imputation:
- `181Project_ML_SynData.Rmd`: R Markdown file for data imputation using MICE method.
- `synthesis_data.ipynb`: Jupyter notebook for synthesizing data.

### Prediction Scripts
Contains scripts for predicting heart disease:
- `Prediction.ipynb`: Jupyter notebook for running prediction models.

## Usage

### 1. Obtain Raw data sets. 
These can found from the links below: 
heart_disease - https://archive.ics.uci.edu/dataset/45/heart+disease
heart - https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction
Medicaldataset - https://data.mendeley.com/datasets/wmhctcrt5v/1
Cardiovascular_Disease_Dataset - https://data.mendeley.com/datasets/dzz48mvjht/1
framingham - https://www.kaggle.com/datasets/aasheesh200/framingham-heart-study-dataset 

### 2. Data Cleaning. 
Follow the guidelines in `Data Cleaning Scripts` and the UCI_DD in Data Dictionary for cleaning the UCI/heart_disease dataset. 

For the other data sets follow the data dictionaries associated with the dataset (read in csv format)

heart - Kaggle_DD
Medicaldataset - Mendeley_dataset
heart_disease - UCI_DD
Cardiovascular_Disease_Dataset - Mendeley1_DD
framingham - Framingham_DD

At this point you should have 5 separately cleaned data sets

### 3. Data Merging
 In the `Data Cleaning Cleaning Scripts` run the MergingDF python file. The outputted file should include a full dataframe with all combined data sets. 

### 4. Data Imputation
To impute missing data, run the scripts in the `Imputed Data Algorithms` directory.
The `181Project_ML_SynData.Rmd` will impute the data using the MICE method (ran in R)
The `synthesis_data.ipynb` will impute data using Python's Faker method
The 

### Prediction
To run predictions, use the `Prediction.ipynb` notebook in the `Prediction Scripts` directory.
This script will utilize the imputed data method of choice (read in an as a csv) to predict the 'Result' column and provide a corresponding accuracy and F1 measurement. 

