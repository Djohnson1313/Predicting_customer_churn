# Predicting Customer churn

---

- Darryn Johnson
- Instructor: Mark Barbour
- Date: 08/11/2024
- Blog: (My First Model)[https://datascienceandyou.blogspot.com/2024/08/my-first-model.html]

---

## overview 
In this repository, we look into a dataframe containing 3,333 entries with 21 columns. Each row represents a customer and their respective account iformation including data like the state the reside in, the account length, what plans they purchase and so on. This data was collected by (SyriaTel)[https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset], a telecommunications company.

---

## Business Understanding 
Customers ending their servises with SyriaTel is not ideal, so the goal behined this project is to predict whether a customer will leave or not. This is represented by `churn`. All entries within this dataset has an entry of either true (did churn) or false (did not churn). Uaing this information, as well as all other aspects recorded by SyriTel, we aim to produce a model that can notify us of a customers potential to churn.

---

## Data Distribution 

![Screenshot 2024-08-11 125008](https://github.com/user-attachments/assets/e04dbc43-dccf-416c-bd66-bb3846d931d6)

Here we can see a mojority of customers do not churn, aprox. 85.5% of customers have stayed with the company.

