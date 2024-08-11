# Predicting Customer churn

- Darryn Johnson
- Instructor: Mark Barbour
- Date: 08/11/2024
- Blog: (My First Model)[https://datascienceandyou.blogspot.com/2024/08/my-first-model.html]

## overview 
In this repository, we look into a dataframe containing 3,333 entries with 21 columns. Each row represents a customer and their respective account iformation including data like the state the reside in, the account length, what plans they purchase and so on. This data was collected by (SyriaTel)[https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset], a telecommunications company.

## Business Understanding 
Customers ending their servises with SyriaTel is not ideal, so the goal behined this project is to predict whether a customer will leave or not. This is represented by `churn`. All entries within this dataset has an entry of either true (did churn) or false (did not churn). Uaing this information, as well as all other aspects recorded by SyriTel, we aim to produce a model that can notify us of a customers potential to churn.

## Data Distribution 

![Screenshot 2024-08-11 125008](https://github.com/user-attachments/assets/e04dbc43-dccf-416c-bd66-bb3846d931d6)

Here we can see a mojority of customers do not churn, approx. 85.5% of customers have stayed with the company.

## Modeling 

The modeling process for this specific problem utilized 2 general types of models. A base logistic regression model, and a decision tree classifier.

The 'vanilla' model is used to build upon and compare other models to, to see how they improve upon the base model, if at all. This model started with no additional addatives other then some standard train-test split and scaling to assure a working model process. This model functioned mediocrely, not presenting to well with some of the tests taken. After altering the model, using techniques such as SMOTE and variance selection, it was decided a different model all together may be a better aproach.

The next model used is a decision tree classifer. This model essentialy asks questions to narrow down what the potential outcome may be.  
