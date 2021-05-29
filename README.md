# churn
Dataset Info: Sample Data Set containing Telco customer data and showing customer left last month
While performing EDA I came with some insights.

These are some of the quick insights from this:
1. Electronic check medium are the highest churners
2. Contract Type - Monthly customers are more likely to churn because of no contract terms, as they are free to go customers.
3. No Online security, No Tech Support category are high churners
4. Non senior Citizens are high churners


![image](https://user-images.githubusercontent.com/66546997/120060895-0193bd00-c078-11eb-80b1-1b565689de24.png)



![image](https://user-images.githubusercontent.com/66546997/120060921-21c37c00-c078-11eb-9770-2410636f39cb.png)



### Model Building
1.PCA model gave me an accuracy of 62%.

2.SVM model gave me an accuracy 77%.

3.KNN model gave me an accuracy of 78%.

4.Logistic regresssion gave me an accuracy of 80%.

5.XG boost gave me an accuracy of 80% and after performing hyperparameter tuning result came out to be 81%.

As you can see that the accuracy is quite low, and as it's an imbalanced dataset, we shouldn't consider Accuracy as our metrics to measure the model, as Accuracy is cursed in imbalanced datasets.

Hence, we need to check recall, precision & f1 score for the minority class, and it's quite evident that the precision, recall & f1 score is too low for Class 1, i.e. churned customers.


6.Decision tree gave 79% and applying smote gave 82%.

7.Random forest gave 80% and applying smote gave 84%.

#### So, i finalised the model which was created by RF classifier

#### Model deployment is done with other account on Heroku using Flask.

