# Titanic Survival Analysis

In the early hours of the morning of 15 April 1912, the RMS Titanic sank on its maiden voyage across the Atlantic Ocean after it struck an iceberg. As part of an independent investigation into the tragedy, I have taken part in conducting the analysing into the survival logs of passengers aboard the Titanic. 

The purpose of this notebook is to use machine learning to create a model that predicts which passengers survived the Titanic shipwreck. Additionally, to understand which groups of passengers were more or less likely to survive due to various factors (i.e. Sex, Socio-economic).

The components of this analysis will include:
- Exploratory Data Analysis (Part of RM-24-10-2022-Titanic-EDA-and-Data-Cleaning notebook)
- Data Cleaning (Part of RM-24-10-2022-Titanic-EDA-and-Data-Cleaning notebook)
- Data Modeling (Part of RM-25-10-2022-Titanic-Data-Modeling-and-Predictions notebook)
- Data Prediction (Part of RM-25-10-2022-Titanic-Data-Modeling-and-Predictions notebook)


All models inspected:
- [DecisionTreeClassifier](https://scikit-learn.org/stable/modules/tree.html)
- [RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
- [AdaBoostClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostClassifier.html)
- [BaggingClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.BaggingClassifier.html)
- [GradientBoostingClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html)
- [HistGradientBoostingClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.HistGradientBoostingClassifier.html)
- [Generalized Linear Model](https://www.statsmodels.org/dev/glm.html)


The final model selected is a generalized linear model (GLM).
- GLM's are a flexible generalization of ordinary linear regression.
- Model comparisons are performed using the difference in Deviation
- Model checking is conducted by inspecting the Studentized Residuals and Leverage


This project is part of a Kaggle competition: [titianic-compeition](https://www.kaggle.com/competitions/titanic/overview)

My leaderboard scores for Accuracy

| Score  | Date | Notes |
| --- | --- | --- |
| 0.760  | 24-10-22 | Base Model | 
| 0.763	 | 25-10-22 | XGBRegressor for Age prediction |
