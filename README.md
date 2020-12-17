# StockReturnTrend

## Project Overview

The Project aims at prediciting if the return for a stock/portfolio will be positive or negative as compared to previous day. We use Fama-French model as our basis and further develope it using different Machine Learning algorithms to build better prediction Models . The image below shows the Fama-French model equation

![image](https://user-images.githubusercontent.com/68875257/102532944-bca03f00-4072-11eb-9440-864befbb1af1.png)


## Data Preview

![image](https://user-images.githubusercontent.com/68875257/102533291-35070000-4073-11eb-9151-fae1475316ae.png)

## Methodology

In the project since I am finding the trend of retrn. I created a new variable - Trend that had value 1 if the exret of next day was higher as compare to today ; 0 if the exret was the same and -1 if next days exret was lower as compare to today.
![image](https://user-images.githubusercontent.com/68875257/102533837-e9a12180-4073-11eb-8e25-2d4a023c11f1.png)

Upon finalizing Trend as the Y variable, I performed co-rrelation analysis and feature importance to select only relevant variables for my Machine Learning models. 

## Machine Learning Models

Three Machine Learning Models were compared and the best model with refined using grid search to give us the best possible accuracy
1) KNN
2) Decision Tree
3) Xgboost

## Results
 XGboost had the best AUC-ROC curve and the model was 75% accurate in predicting trend on the test set.
