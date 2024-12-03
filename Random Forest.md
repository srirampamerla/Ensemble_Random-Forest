# Random Forest

A popular bagging algorithm that uses decision trees as base models. It further introduces randomness by selecting a random subset of features at each node of the tree, leading to more diverse and robust models.

Why we use DT in random forest. (Problems in 1. DT has Low Bias and High varience 2.Pruning can be done but lot of expensive  3. Overfitting without hyper parameter).

Low Bias-> When i am creating the DT to the depth--> It will train properly on the training dataset.
When combining through bootstrapping algorithm the High Varience converted to Low Varience by voting majority(Generalized Model Means Low Bias & Varience)

While Passing the data to the model we will use FS+RS (Feature and Row Sampling).--> Usually we need to select the Rows and features give to the model(feature & Rows may or maynot repeat)

Normalization not required for DT & Random Forest. DT will split the features. If you minimize the data then also it will split. That won't imp in case of DT.
When DT is constructed all points must be classified even outliers can be classified. 

It will only affect DT only when we selected Boosting.

Custom Bagging--> We can define our own model with out any ML algorithm.



