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

< img src = 'assets/e04dbc43-dccf-416c-bd66-bb3846d931d6.png' width = '100' />
< img src = [Screenshot 2024-08-11 125008](https://github.com/user-attachments/assets/2de9aa61-b512-4e64-a976-254761fc5f96) width = '100' />


Here we can see a mojority of customers do not churn, approx. 85.5% of customers have stayed with the company.

## Modeling 

The modeling process for this specific problem utilized 2 general types of models. A base logistic regression model, and a decision tree classifier.

The 'vanilla' model is used to build upon and compare other models to, to see how they improve upon the base model, if at all. This model started with no additional addatives other then some standard train-test split and scaling to assure a working model process. This model functioned mediocrely, not presenting to well with some of the tests taken. After altering the model, using techniques such as SMOTE and variance selection, it was decided a different model all together may be a better aproach.

The next model used is a decision tree classifer. This model essentialy asks questions to narrow down what the potential outcome may be. This model performed significantly better then the standard model, performing failry well with the tests conducted. Here is a visualization of the model.

![Screenshot 2024-08-11 130508](https://github.com/user-attachments/assets/26335365-1c39-4d88-9537-45acc56638eb)

This model is indeed large and complex. The next logical step includes limiting this model to see if we can get it to function faster and display a readable visual representation. These steps include things like limiting the size of the tree, maximum features the tree uses and so on. After running through these tree reduction exercises, it was determined even though this tree is large, it performes better as is.

## Evaluation 

Decision tree classifier outperformes the other model and model iterations. It has extreme ease of access and simply put, just worked better. The model performed well with the ROC curve, confusion martix, and has a 91% accuracy score. Here are those graphs:

![Screenshot 2024-08-11 131422](https://github.com/user-attachments/assets/ebed43fc-c2ae-4c06-a2f3-23b04ac4f4ec)

![Screenshot 2024-08-11 131403](https://github.com/user-attachments/assets/2fff6687-fd08-4bb9-80b0-6aa989c58f7e)
