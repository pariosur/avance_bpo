# Forecasting recovery rates for debt collection agency: Avance BPO
> ML workflow used to prioritize dialing lists for a debt collection agency.
## Table of Contents
* [General Info](#general-information)
* [Project Process](#project-process)
* [Room for Improvement](#room-for-improvement)
* [Acknowledgements](#acknowledgements)
## General Information
- A non-performing loan (NPL) is a loan that is in default due to the fact that the borrower has not made the scheduled payments for a specified period. 
- Non-performing loans are purchased from the bank by a debt collection agency which must prioritize which users to prompt first. One of the most important factors regarding this decision is the recovery rate: the percentage of exposure that can be recovered from each borrower through the debt collection process. The recovery rates achievable by the debt collector are unknown at the time of purchase of the portfolio and need to be predicted.
- Based on the information given by the bank, the objective of this model is to predict the recovery rates on non-performing loans (NLP) using a private database from a Colombian debt collection agency called Avance BPO.
## Project Process
- Set target variable as the rate of recovery, computed as the sum of recovery payments made by a given loan Id, divided by the initial amount of the loan.
- Merged target variable with features dataset grouping by Loan ID. 
- Preprocessed data by removing missing values, dropping outliers and defining categorical variables.
- Split train and test data for modelling. 
- Create Model Pipeline, one hot encoding categorical variables and scaling numerical variables. 
- Based on applied literature, used 3 recommended estimators and cross validated them to pick the best one for this dataset.  
- Predict baseline on test set and sort results in descending order. 
- Plot and display feature importance. 
## Room for Improvement

Room for improvement:
- Include more socio demographic from the borrower. 
- Include more socio demographic data from the borrower. 
- Include loan data from the bank regarding client payment behaviour before being transfered to the debt collecting agency. 
- Include business cycle variables like macroeconomic and ﬁnancial macro economic indicators that capture economic uncertainty and other variables that may affect payment behaviour. 

## Acknowledgements
- Many thanks to the authors of this [paper](https://www.researchgate.net/publication/342467001_Forecasting_recovery_rates_on_non-performing_loans_with_machine_learning) for their advancements and recommending the appropiate model. 
TY  - JOUR
AU  - Bellotti, Anthony
AU  - Brigo, Damiano
AU  - Gambetti, Paolo
AU  - Vrins, Frederic
PY  - 2021/01/01
SP  - 428
EP  - 444
T1  - Forecasting recovery rates on non-performing loans with machine learning
VL  - 37
DO  - 10.1016/j.ijforecast.2020.06.009
JO  - International Journal of Forecasting
ER  - 
