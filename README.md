# Project 4: Customer Classification

## Table of Contents
[1. Project Description](README.md#Project-Description)  
[2. Business Problem](README.md#Business-Problem)  
[3. Data Overview](README.md#Data-Overview)  
[4. Project Workflow](README.md#Project-Workflow)  
[5. Results](README.md#Results)  
[6. Conclusions](README.md#Conclusions)  

---

## Project Description
This project focuses on building a machine learning model for classifying bank customers. Using historical data from previous marketing campaigns, we train a model to predict whether a customer will open a deposit account.  

**Business Value:**  
- Optimizing bank marketing expenses.  
- Increasing conversion rates by targeting potential customers more effectively.  

[See the full notebook here](https://github.com/AndKober/Project_4/blob/master/Project_4_ML.ipynb)  

---

## Business Problem
The dataset contains information about a bank's marketing campaign aimed at attracting customers to open deposit accounts.  

### Objective:
Identify the characteristics of customers who are more likely to open a deposit, improving the efficiency of marketing campaigns.  

### Technical Tasks:
- Handle missing values and outliers.  
- Perform exploratory data analysis (EDA).  
- Select key features, build, and evaluate classification models.  

### Evaluation Metrics:
- Accuracy  
- F1-score  

---

## Data Overview
### Customer Information:
- *age* – age  
- *job* – employment sector  
- *marital* – marital status  
- *education* – education level  
- *default* – has credit in default (yes/no)  
- *housing* – has housing loan (yes/no)  
- *loan* – has personal loan (yes/no)  
- *balance* – account balance  

### Marketing Campaign Data:
- *contact* – contact method (telephone, email)  
- *month* – last contact month  
- *day* – last contact day  
- *duration* – last contact duration in seconds  

### Other Features:
- *campaign* – number of contacts during the current campaign  
- *pdays* – number of days since last campaign contact  
- *previous* – number of previous contacts before the current campaign  
- *poutcome* – outcome of the previous campaign  

### Target Variable:
- *deposit* – whether the client opened a deposit (0 – No, 1 – Yes)  

---

## Project Workflow
1️⃣ **Data Preprocessing:**  
- Handling missing values  
- Detecting and processing outliers (Interquartile Range (IQR) method)  

2️⃣ **Exploratory Data Analysis (EDA):**  
- Feature distribution visualization  
- Correlation analysis  

3️⃣ **Feature Selection & Transformation:**  
- Encoding categorical variables (Label Encoding)  
- Scaling numerical features  

4️⃣ **Model Training & Classification:**  
- Logistic Regression  
- Decision Trees  
- Ensemble Models (Random Forest, Gradient Boosting)  

5️⃣ **Model Evaluation & Insights:**  
- Comparing performance metrics (Accuracy, F1-score)  
- Identifying key influential features  

---

## Results
✅ The best-performing model achieved **Accuracy = 83%** and **F1-score = 82%** on the test set.  
✅ The most significant features influencing deposit decisions:  
   - **balance** (customer account balance)  
   - **duration** (last contact duration)  
   - **poutcome_success** (success of the previous campaign)  

---

## Conclusions
🔹 **Simple models (Logistic Regression, Decision Trees) performed almost as well as complex ensemble models.**  
🔹 **Outliers were detected and removed using the Interquartile Range (IQR) method, improving model accuracy.**  
🔹 **In real-world scenarios, computational costs must be considered, as complex models do not always justify their added expense.**  
