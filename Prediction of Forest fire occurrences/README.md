# Machine-Learning

In this project, I propose five classification models: **Support Vector Machines (SVMs), Logistic Regression, Random Forest, K Nearest Neighbors(KNNs) and Multi-layer Perceptron (MLP)** to predict the possibility of a forest fire in the future. I have used the Nearest Means Classifier as my Baseline system.

**Data Set : Algerian forest fires**

All these models are compared based on the performance measures: Test Accuracy, F1-score, and confusion matrices on the Algerian Fires dataset, which originally consisted of 9 real-valued input features.

Among them, the SVM, Logistic regression and Random forests have reported the **highest test accuracy of 91.67%**. The model that gave the best test accuracy and F-1 score is the random forest classifier that achieved test accuracy of 91.67% along with the **highest F-1 score of 0.8936**.

In addition to these features, I have performed feature engineering to generate 9 more new features, which are the previous 3-day rolling averages of the original 9 features. This has enabled me to obtain a 3% higher test accuracy of 91.67% on my SVM model over unnormalized original data and thereby giving the highest test accuracy measure among all the models. 

I have coded the function for Data Normalization partly by myself and partly by using the Standard Scaler function from sklearn. Using this function, I have normalized the input data and have observed an increase in accuracy of over 1.67% for SVMs, Logistic regression classifier and MLP and, 1% for KNNs with a significantly lower training and inference times, thus making it on par with the engineered-feature dataset in terms of accuracy and overwhelmed the latter in terms of training and inference speeds.

I have opted to use the K-fold cross validation algorithm for hyperparameter tuning and model selection in addition to using a grid search. However, one change I have made in my implementation is the removal of shuffling the dataset step for reproducibility of the results.

The libraries used for this project are:

1. seaborn
2. numpy
3. pandas
4. sklearn
5. math

A deeper insight into the project is presented in the report.pdf file.
