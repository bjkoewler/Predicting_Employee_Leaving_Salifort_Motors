# Predicting_Employee_Leaving_Salifort_Motors

## Overview
The human resources department at Salifort Motors wants to improve employee satisfaction. Their question is: What makes an employee likely to leave the company? The task is to build a machine learning model that can predict those who would leave, and identify those factors that play the largest role in this prediction.

## Business Understanding
The company wants to improve employee satisfaction, an admirable objective no matter the industry. By improving satisfaction and increasing retention, the company will save significant amounts of money in the locating, interviewing, hiring and training of new employees, both direct costs and losses of productivity. With a successful implementation of insights derived from this project, both the company and employees will benefit, making it a win-win. 

## Data Understanding
The data was collected by the Salifort Motors human resources department. The dataset consists of 15,000 records with 10 columns of variables. Some features include tenure, monthly average hours, last evaluation score, and number of projects. The outcome variable was a binary column named 'left'. A feature named 'overworked' was engineered to reveal insight about those who worked greater than 174 hours. The plot below shows how satisfaction level varies by tenure, with the nadir at tenure year 4.
![alt text](https://github.com/bjkoewler/Predicting_Employee_Leaving_Salifort_Motors/blob/main/images/satisfaction_by_tenure.png?raw=true)


## Modeling and Evaluation
After testing multiple models, the XGBoost ensemble demonstrated the highest results and was chosen as the champion model. The model achieved an auc of 94%, accuracy of 97%, precision of 91% and a recall of 90%. The plot below shows the top three most important features in classifying whether an employee left or not are: last_evaluation, tenure, and n_projects.


## Conclusion
This model accurately predicts thos employeees who would leave, and has the potential to save the company signficant time and money. However, it does not tell us why the employees are dissatisfied, and more information can further improve Salifort's efforts to increase satisfaction across its workforce. Building an unsupervised model(K-means) may provide further insight after analysis of how it clusters the dataset.
