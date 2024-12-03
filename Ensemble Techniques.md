# Ensemble techniques 

combine multiple models to improve performance and accuracy in both classification and regression tasks. 

The three main ensemble techniques are:

1. Random Forest
2. XGBoost
3. AdaBoost

Types of Ensemble Techniques: Bagging and Boosting

# Bagging (Bootstrap Aggregating):

Involves training multiple models on different subsets of the data. Given a dataset with 10,000 records, each model is trained on a random sample of 1,000 records. These samples are drawn using row sampling with replacement, a technique called bootstrap.
Each model generates an output (prediction). The final output is determined by majority voting, where the prediction with the highest consensus across models is selected.
Combining bootstrap and aggregation leads to the term Bootstrap Aggregating (Bagging). This process enhances model stability and reduces overfitting, making it a powerful ensemble method.

In case of regression we will average all the o/p or calculate mean for all the o/p from each model. That will be the final o/p.

Random Forest: A popular bagging algorithm that uses decision trees as base models. It further introduces randomness by selecting a random subset of features at each node of the tree, leading to more diverse and robust models.

We can select any models like Logistic, DT, KNN, Naive Bayers....

In Bagging --> Random Forest(Classifier and Regressor)

# Boosting: 

Boosting is a sequential approach where models are trained iteratively, with each model focusing on the errors made by the previous ones. This technique improves accuracy and handles complex patterns.

Sequential combination of models(i.e we have 4 models all are weak learners. When we combine all the weak learners will become Strong learner). if model not able to solve any thing it will be transferred to next model. Final it will give o/p

Boosting --> Adaboost, Gradient, xgboost

Adaboost (Adaptive Boosting): Assigns weights to training samples, giving more importance to misclassified instances in subsequent iterations.

Gradient Boosting: Minimizes a loss function by iteratively adding weak learners, each correcting the errors of the previous ones.

XGBoost (Extreme Gradient Boosting): An optimized implementation of gradient boosting, known for its efficiency and performance.

Bagging reduces variance by averaging predictions from multiple models.

Boosting reduces bias by sequentially correcting errors of previous models.
