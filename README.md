# MachineLearning_Assignment9-3
Repository for Machine Learning Assignment 9 : Posting Assignment 3

1. Find a dataset with sufficiently many labels so that overfitting is likely. Use a grid search (after doing train/test split) with either Lasso or Ridge to determine the optimal regularization parameter. Determine the score of the test set using the optimal parameter. 

Dataset used : 
"players_data-2024_2025.csv"
https://www.kaggle.com/datasets/hubertsidorowicz/football-players-stats-2024-2025?select=players_data-2024_2025.csv 

Dataset begins with 267 features that covers soccer player's statistics (minutes per game, assists per game, goals, etc). After cleaning, the dataset contains 140 features of quantative data. After performing grid search and using Lasso with an optimal parameter, the score of the test set ended up at 0.9999990321195683.

2. Find a classification problem where there only two categories for the label and at least two quantitative features which will be used to predict the label. After a train/test split use a grid search to identify the optimal regularization parameter C for a linear support vector classifier. Create a confusion matrix for the test dataset with the optimal parameter.

Dataset used :
"BankNote_Authentication.csv" Where the target is classifying the authentication (0 for fakes and 1 for real notes).
https://www.kaggle.com/datasets/mastershomya/banknote-authetication

After peforming gridsearch, an optimal parameter of C=0.1 was found with a corresponding score of 0.983. Given the confusion matrix, the linear SVC performed very well on this data, predicting that real bank notes were real almost 100% of the time. It had minimal issues also classifying some fake bank notes as real.

![Assign3pt2_CM](https://github.com/user-attachments/assets/4c713220-caad-42d2-b5b0-08b7c7287efe)
