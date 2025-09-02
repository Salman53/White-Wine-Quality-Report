📌 Introduction

This project focuses on predicting white wine quality (good or bad) using machine learning techniques.
The dataset includes physicochemical features such as acidity, sugar, pH, alcohol, and density.
By applying Logistic Regression, Decision Tree, and Random Forest, the goal is to identify the most influential features and select the best-performing model.

📂 Dataset

Source: UCI Wine Quality Dataset (White Wine)

Observations: 3,917 (train), 354 (test)

Features: 11 physicochemical attributes (e.g., acidity, sugar, pH, alcohol)

Target Variable: quality_binary (1 = good, 0 = bad)

🔬 Methods

Exploratory Data Analysis (EDA): Histograms, correlation heatmaps, scatter plots

Feature Engineering: Converted quality scores to binary classification

Modeling Approaches:

Logistic Regression

Decision Tree

Random Forest

Evaluation Metrics: Accuracy, Precision, Recall, Balanced Accuracy, AUC, Kappa

| Model               | Accuracy  | Precision | Recall (Bad) | Recall (Good) | AUC       | Kappa     |
| ------------------- | --------- | --------- | ------------ | ------------- | --------- | --------- |
| Logistic Regression | 77.0%     | 69.2%     | 56.5%        | 87.3%         | 0.794     | 0.459     |
| Decision Tree       | 75.9%     | 66.9%     | 54.9%        | 86.4%         | 0.739     | 0.432     |
| Random Forest       | **83.1%** | **79.0%** | **67.6%**    | **90.9%**     | **0.894** | **0.607** |


✅ Random Forest delivered the best performance with 83% accuracy and the highest AUC (0.894).

🛠️ Technologies Used

Language: R

Libraries: tidyverse, caret, randomForest, rpart, pROC, corrplot, GGally

📌 Key Insights

Alcohol content is strongly associated with higher quality wines.

Volatile acidity negatively impacts quality.

Density and sulfur dioxide levels also play key roles in classification.

🚀 How to Run

Clone the repository
git clone https://github.com/Salman53/White-Wine-Quality-Report

Open the project in R or RStudio

Run the scripts in the /code folder or open the .Rmd file

