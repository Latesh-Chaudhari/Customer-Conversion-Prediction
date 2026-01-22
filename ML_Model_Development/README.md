<h1 align="center"> :large_orange_diamond: ML Model Development :large_orange_diamond: </h1>

To predict the consumer response to the telemarketing campaign , we need to use binary classification models. As part of this project , Logistic, Naïve Bayes and SVM, Neural Network and Tree Based Model as Decision Tree, CART, Random Forest models are trained and tested . The results of each model are mentioned below .  

## Logistic Regression Model
- Logistic regression is a statistical model that uses a logistic function to model a binary dependent variable. In regression analysis, logistic regression (or logit regression) is estimating the parameters of a logistic model (a form of binary regression). It models the probability of the classes from target variable.  These probability predictions will be transformed into binary values (0 or 1) so that the appropriate classes can be obtained as output of the model.
- As a part of feature engineering, multicollinearity check and the variable inflation factor concludes the significant features comes out to be contact, month, duration, pdays, emp.var.rate, Campaign, cons.conf.idx, poutcome, day of week
- Performance measures on Test dataset - Accuracy = 91.23 , AUC = 0.9328 and Gini Coefficient = 0.9363

 ## Naïve Bayes Model
- Naïve Bayes is one of the "probabilistic classifiers" based on Bayes' Theorem with an assumption of independence among predictors. It is a Supervised Machine Learning algorithm. In simple terms, a Naive Bayes classifier assumes that the presence of a particular feature in a class is unrelated to the presence of any other feature. It uses the probability terms from training set to classify the target variable.
- Performance measures on Test dataset - Accuracy = 90.50 , AUC = 0.6793 , Gini Coefficient = 0.0615

 ## Neural Network
- Neural networks are a set of algorithms, modeled loosely after the human brain, that are designed to recognize patterns. They interpret sensory data through a kind of machine perception, labeling or clustering raw input
- As a requirement of the neural network, scaling the variables is to be performed so that weights will be assigned by neural network model.
- The neural network is built with max 2000 iterations and converges after 730 iterations. There are 9 Inputs layers and 21 hidden nodes in single hidden layer and one output node.
- Performance measures on Test dataset - Accuracy = 90.50 , AUC = 0.6793 , Gini Coefficient = 0.0615

 ## Support Vector Machine
- Support Vector Machine algorithm tries to maximize the margin between classifiers using support vectors i.e hyper planes . The kernel trick means transforming data into another dimension that has a clear dividing margin between classes of data. Using kernel trick one can easily draw a hyper plane between the various classes of data.cost function and gamma functions are used as hyperparameters to optimize the output of the models.
1) Linear Kernel : - Linear Kernel is used when the data is linearly separable, that is, it can be separated using a single Line . 
                   - Performance measures on Test dataset - Accuracy = 94.15 , AUC = 0.7348 , Gini Coefficient = 0.0468
2) Radial Kernel : - While tuning the performance parameters, we found that cost function=0.1 was not at all able to predict the subscribe yes class. After passing the                               regularization parameters, cost function C =1 and gamma value as 1,svm model has been built which is used for the predicting the class. 
                   - Performance measures on Test dataset - Accuracy = 92.06 , AUC = 0.689 , Gini Coefficient = 0.0412
3) Polynomial Kernel: - Polynomial kernel is a kernel function that represent the similarity of vectors (training samples) in a feature space over polynomials of the original                           variables, allowing learning of non-linear models
                      - Performance measures on Test dataset - Accuracy = 92.66 , AUC = 0.7119 , Gini Coefficient = 0.0528

 ## XGboost  
 - XGBoost i.e Extreme Gradient Boosting is ensemble method which uses many trees to take decision by gaining power from previously grown trees
 - Since this is classification problem, Booster parameter is gbtree , and learning rate (eta) will be 0.3 and maximum depth of trees to be created is 6,with 20 rounds has been  used
 - Performance measures on Test dataset - Accuracy = 93.30 , AUC = 0.7796 , Gini Coefficient = 0.91478

 ## Decision Tree based CART Model
 - Decision Trees are non-parametric supervised learning method used can be used for classification as well
 - It can be seen from the accuracy that the model can be over fit with fully grown tree because of all features. Hence smaller sub tree can be built by pruning which will provide comparable results with fewer splits and better interpretation at the cost of little bias
 - In pruned tree and according to variable importance measurement , high information value can be observed for features duration ,nr.employed , euribor3m , pdays , emp.var.rate, cons.conf.idx and cons.price.id
 -  Performance measures on Test dataset - Accuracy = 92 , AUC = 0.8652 , Gini Coefficient = 0.5136

 ## Random Forest Model 
 - Random Forest is the supervised classification algorithm which randomly creates forest with several trees
 - Random forest is based on the idea of bagging which is used to reduce the variation In prediction by combining the result of multiple decision trees on different sample of test set
 - After incorporating the hyper parameters, random forest model gives Out-of-Bag has been reduced to 8.55% and the class error has been reduced to 0.48
 - The duration, euribor3m, nr.employed, pdays, emp.var.rate, cons.price.idx,cons.conf.idx , poutcome_success seems to be significant variables
 - Performance measures on Test dataset - Accuracy = 96 , AUC = 0.9247 , Gini Coefficient = 0.9092

# Model Summary 
- Based on the performance measures of the models **"Random forest"** seems to be most performant model.
- Unlike Cart, Random forest reduces the variation in prediction by combining the result of multiple decision trees on different sample of test set. Thus averaging the result causing less variation is the unique feature which comes makes random forest best model according to this dataset.
- Duration, pdays, nr.employed, euribor3m seems to be most important features which comes out to be significant in almost all models.
