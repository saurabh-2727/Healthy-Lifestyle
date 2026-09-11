
# Healthy Lifestyle Prediction

## About Project
This is my self project in which I have built a ML model to predict whether a person is leading a 'healthy' lifestyle or not. The model performance was judged by **F1 score** metric.


## Tools used
+ NumPy
+ Pandas
+ Seaborn
+ Matplotlib
+ Scikit-learn
+ Imblearn

## Procedure
+ Nature of numerical and categorical features was identified, and then suitable techniques like **modal imputation** for filling **NaN** values for categorical features was employed.
+ **Box-plots** showed the **presence of outliers** in **numerical columns**, but further analysis showed that the outliers did'nt affect the **statistics** of the numerical features much, so they weren't dropped.
+ **Data visualization** was done using **histograms**, **countplots** and **correlation heatmap**. **Correlation heatmap** explained some correlation between some features. (ensemble methods like random forest are robust to correlations as In each split of a decision tree, only a subset of features is considered, reducing the impact of correlation)
+ As the dataset was **imbalanced**, both **undersampling** and **oversampling** was done, to assess model selection and performance.
+ Various models were chosen like Logistic regression, SVMs, Decision Trees and Random Forest. Out all these, **Random Forest** performed the best with data that was **oversampled** (scaling sometimes helped and sometimes not), achieving a **f1 score** of **0.799 to 0.803**.
+ **Hyperparameter-tuning** was performed in an attempt to improve it's performance.
+ CSV file for GridSearchCV process was saved where we can access the hyperparameters and corresponding scores for better understanding.

## Results
+ Finally the model with best params achieved a **F1 score** of **0.847558**.
+ A score of **82.0274** was achieved on  test set. (rf was trained on entire train set to check if score increases)

## References
+ [https://numpy.org/](https://numpy.org/)
+ [https://pandas.pydata.org/](https://pandas.pydata.org/)
+ [https://scikit-learn.org/stable/](https://scikit-learn.org/stable/)
+ [https://seaborn.pydata.org/](https://seaborn.pydata.org/)
+ [https://matplotlib.org/](https://matplotlib.org/)
+ [https://imbalanced-learn.org/stable/](https://imbalanced-learn.org/stable/)
+ [https://odsc.medium.com/optimizing-hyperparameters-for-random-forest-algorithms-in-scikit-learn-d60b7aa07ead](https://odsc.medium.com/optimizing-hyperparameters-for-random-forest-algorithms-in-scikit-learn-d60b7aa07ead)
