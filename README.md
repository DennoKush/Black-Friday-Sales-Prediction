## Introduction

[Analytics Vidhya](https://www.analyticsvidhya.com/) organized a weekend hackathon called [Black Friday Data Hack](https://datahack.analyticsvidhya.com/contest/black-friday-data-hack/) which was held on 20th November to 22nd November, 2015.

The challenge was to predict the purchase amount of various products by users across categories given historical data of purchase amounts using supervised machine learning models.

## File Descriptions

Three datasets have been provided. 
`train.csv`: training dataset that consists of 550068 rows and 12 columns.
`test.csv` : testing dataset consisting of 233599 rows and 11 columns
`sample_submission_LMg97w5.csv` : sample submission dataset

## Approach

The first step was to understand available features and do some feature engineering. During my analysis I realized **Product_Category_2** and **Product_Category_3** had missing values thus I had to take care of that through imputation(for both features I filled in missing values with 9999).

Response variable showed positive skewness, peakedness and deviated from from normal distribution.

## Model

I tried out 3 models, **Lasso Regression**, **Linear Regression** and **RandomForest Regressor** . The first two models were too simple for this problem and produced a relatively big RMSE, 4605 and 4685 respectively. RandomForest Regressor performed well and had a RMSE of 2650.

## Acknowledgements

Special thanks to [Analytics Vidhya](https://www.analyticsvidhya.com/) for organizing the competition and providing some clean datasets. I would also pass my sincere gratitude to [Roshan Sharma](https://www.kaggle.com/roshansharma/black-friday-regression-analysis) and [Shamalip](https://www.kaggle.com/shamalip/black-friday-data-exploration) for your comprehensive data analysis which informed a better part of this project.