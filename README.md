# charityanalysis
Detailed Report: Predicting Income Using Random Forest Classifier
1. Introduction
This report outlines the process of predicting whether an individual’s income exceeds 50K using a machine learning model (Random Forest Classifier) based on various features such as workclass, education level, marital status, and more. The dataset demographic data such as age, education, occupation, and income class.

Model Evaluation Report
Accuracy
The model achieved an accuracy of 85.20%, which indicates that approximately 85% of the predictions made by the Random Forest classifier were correct.
Classification Metrics
The classification report includes precision, recall, and F1-score for both classes: <=50K (Class 0) and >50K (Class 1). 
The Random Forest classifier performs well overall, especially for predicting the <=50K class. However, its performance on the >50K class could be improved. The recall for >50K is relatively lower, indicating that the model is missing a significant number of individuals in this income category.
One potential area for improvement is addressing the class imbalance between the two classes (more individuals with <=50K than >50K). 

Visualizing Feature Importance
A bar plot was created to visualize the importance of each feature in predicting income:

![feature_importance](https://github.com/user-attachments/assets/69569d9e-aba9-456a-b156-3a8cc1df4f15)

Age is the most important feature in predicting whether an individual's income is greater than or less than $50K. The plot suggests that the model heavily relies on the age, capital gains, relationship, hours per week of an individual to make predictions about income.Sex (gender) was the least important feature for this model, meaning it had little to no impact on predicting income.

The income distribution plot you generated suggests that the majority of individuals in the dataset fall under the income category <=50K, represented by 0. In the dataset, there are more than 30,000 instances for 0 (<=50K), and approximately 10,000 instances for 1 (>50K).
![income_distribution](https://github.com/user-attachments/assets/48ecae3f-a2d3-46f6-9307-ef3a20f5806f)

Interpretation of the Income Distribution:
0 (Income <= 50K):
The count for this category is significantly higher, indicating that most individuals in this dataset earn less than or equal to $50K. This could be due to various factors such as lower education levels, fewer working hours, or other socioeconomic factors.
1 (Income > 50K):
The count for individuals earning more than $50K is relatively lower. This suggests that the dataset has fewer high-income earners compared to low-income earners. It could be reflective of income distribution patterns in the real world, where the number of people with higher incomes generally tends to be smaller compared to those with lower or middle incomes.
