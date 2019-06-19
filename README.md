# Sparkify-Churn-Prediction

## File Contents
    .
    ├── Images
        └── Inside this folder, you will find various figures used in the Notebook
    ├── Sparkify.ipynb    
    ├── LICENSE
    └── README.md

## Libraries Used
The notebook was run on Python 3.6.3, please ensure your version is at or above this version level to run.

- pyspark
- numpy
- pandas
- matplotlib
-seaborn
- plotly

## Sparkify Overview
Since customer churn is such an important need for most businesses I decided to do my Udacity Capstone project on Sparkify. Sparkify is a music service much like Spotify where users can either listen to music for free or subscribe to listen to music without adds. Within the app, any user can choose to upgrade, downgrade or cancel their subscription. Canceling their subscription means that they will cease to use the app and all revenue gained by having the customer as either a free or paid user will be lost.

## Problem Statement
The main focus of this project is to try and predict customer churn by only looking at customer behavior. A large amount of data has to be analyzed since every interaction a user has with the app is recorded. Since there is so much data, a big data framework needs to be used. For this project, I will be using Apache Spark.

## Project Outline
1. Data cleaning and exploration
2. Feature selection & engineering
3. Model Building
4. Model evaluation and improvement

## Model Selection
I compare the Random Forest, Gradient boosting, Linear SVM and Logistic regression models. I finally picked the Random Forest Classifier as it outperforms all the other models based on F1 score as well as training time.

## Conclusion
The final model that was selected looked very promising as it achieved an 86.69% accuracy by just training it on the small dataset.

To put the accuracy into perspective, consider that if there is no churn prediction a company will either choose to continue as usual in which case they assume no customer will churn or they will give out promotions or special service to all customers in which case they assume all customers will churn. If they assume no customers will churn they would have gotten a 76.88% accuracy and if they assumed all customers would churn they would have gotten a 23.11% prediction accuracy. In both of these cases, the prediction accuracy is lower than what my model achieved on very little data. I also believe that a company like Sparkify would usually assume all customers as potential churn customers considering how important customer retention is.

## Project Reflection
I found it very interesting that the model was able to perform so well on so little data and I was also pretty surprised to see that some of the features I thought would be good predictors turned out to not have a very big impact.

## Future Work and Improvement
The biggest lack of this project is the size of the dataset the model was trained on. Since this model was built to run on big data platforms like AWS I think the next step to improving this project will be to run train this model on a bigger dataset.

Another improve will be to include more and better features than those that were included in this dataset, as I believe there might be some very good features that were left unexplored during the course of this project.

## References
1. https://www.superoffice.com/blog/reduce-customer-churn/
2. https://towardsdatascience.com/hands-on-predict-customer-churn-5c2a42806266
3. https://towardsdatascience.com/accuracy-precision-recall-or-f1-331fb37c5cb9.
