# Neural_Network_Charity_Analysis
## Overview
This analysis studies the performance and feedback of several charity organizations to create a model that can classify which ones are a good choice to invest in & which ones aren't
### Background
The analysis uses a dataset containing 34,000 organizations from the historic information of a company's charity funding. The dataset can be found in the following link:
https://github.com/Lamismn/Neural_Network_Charity_Analysis/blob/main/charity_data.csv

The dataset contains the following entries for each of the organization:

1. EIN and NAME—Identification columns
2. APPLICATION_TYPE—Alphabet Soup application type
3. AFFILIATION—Affiliated sector of industry
4. CLASSIFICATION—Government organization classification
5. USE_CASE—Use case for funding
6. ORGANIZATION—Organization type
7. STATUS—Active status
8. INCOME_AMT—Income classification
9. SPECIAL_CONSIDERATIONS—Special consideration for application
10. ASK_AMT—Funding amount requested
11. IS_SUCCESSFUL—Was the money used effectively

The study uses neural networks to create a deep learning model that can predict the authenticity of teh organization based on the data provided. The target is the (IS SUCCESSFUL) column, & the parameters are the other columns (other than name & EIN)

The dataset is divided into train & test sections, the train is used to train the model, while the test is used to test the performance of the trained model.
## Results
The data was preprocessed before performing the analysis, preprocessing involved the following:
1. dividing the data columns to target variables & features, the target value is the IS_SUCCESSFUl column, since the purpose of the model is to determine if the money given to a certain charity is a good investment
2. The features for this models are the different parameters that an application shows (Application type, affiliated sector, classification, Income amount & if there are any special considerations)
3. EIN & Name, are useless for the analysis & were removed in the preprocessing.

Then the dataset was divided to train & test parts, thhe train was used to train the model & test is to test the performance, a neural network was used to create the model.
1. Two hodden layers were used for the initial analysis, the first with 80 neurons & the second with 30.
2. The initial model achieved an accuracy level of 0.72, which is less than the required 0.75
3. The model was optimized to increase the accuracy, by adding neurons, which increased  the accuracy to 0.73, & adding an extra hidden layer, which also achieved 0.73

## Summary
The model required performance was not achieved, which means that we will need to work more on the data to achieve it, firstly by reducing the parameters, by decreasing the tested variables & then by optimizing the model, increasing neurons to the layers helped more than adding a layer.
