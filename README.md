# credit-risk-classification
## Overview of the Analysis

This project aims to train and evaluate a model based on loan risk. I used a  dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. The model classified the customers into high-risk and low-risk loans. 

## Steps:

1. The CSV file was read into Pandas data frame.
   <img width="566" alt="image" src="https://github.com/bhartikaushal/credit-risk-classification/assets/124011061/7a2e45da-e717-468c-838a-93e981f5ae2b">

2. A label 'y' was created from the loan_status column, and a data frame was created from the rest of the columns. 
3. The dataset was then split into training and testing datasets by using tain_test_split.
4. A linear regression was instantiated and fit into the training dataset. A confusion matrix and a classification report were created for data analysis.
5. A second model was created using the 'Random Oversampler' module. A logistic regression was run on the resampled training data. 

## Results

The classification report for the first model:
<img width="316" alt="image" src="https://github.com/bhartikaushal/credit-risk-classification/assets/124011061/1bfe5f4c-71c8-47a3-a056-bd4391cb52ac">


The classification report for Model 1 shows that the accuracy of the test dataset is less than that of the training dataset. The accuracy for the test dataset is 87 %, while it is 100 % for the training dataset. The difference is not stark, and this model can predict whether the loan risk is high or low to a good extent.

The classification report for Model 2 (resampled dataset) shows high accuracy for both the training(100%) and the test dataset(99%). This model accurately predicts whether the loan is high-risk or low-risk.
<img width="308" alt="image" src="https://github.com/bhartikaushal/credit-risk-classification/assets/124011061/52d635cd-32cb-47d9-9067-31aab67bb36e">


The resampled data performs best as its accuracy is high for training and test datasets. It is precise in predicting the creditworthiness of borrowers.
