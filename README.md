# Online-Food-Delivery

Food was always considered to be one of the most primary particles in the formation of a human life. Without food there would be no human life. Hence over time the business related to food has grown in size and become very important. 
In the historical times there were farmers that had the noblest work to grow the crops necessary for everyone. Slowly as time evolved instead of everyone growing their own crop, humans started picking up their choice of profession. Hence started the system of trading crops and other stuff. 
Over the years the eatery sector of society grew, various kind of food were invented at various part of the world and the monetary benefits in export and import of these products caught eye of many people.

People love to taste new foods and give their precious reviews on the food items. But as it is a general problem of places that are usually crowed the traffic makes it very frustrating for people to travel to such places. Even the restaurants could not handle so much pressure at one time. Hence in 1995 (World Wide Waiter) the first online food delivery system was started. Though before this in India the Indian dabbawalas use to deliver food in schools and offices from 1890. Over the years this business grew large and more and more online platforms opened. These platforms connected with restaurants and thus expanded their networks. 

![image](https://user-images.githubusercontent.com/62097113/149714205-7d32b6a2-2070-4bba-a809-f4eb8e0ef440.png)

In large cities or in metropolitan places this business has bloomed and star-ups like swiggy and zomato have grown. Even in this lockdown period of our society we have seen the growth of such companies. 
These companies attract students and freshers who do not have a lot of income as they offer discounts and other benefits.

# DATASET

The database use in this project has been sourced from kaggle
(https://www.kaggle.com/benroshan/online-food-delivery-preferencesbangalore-region).
The goal is to see if we can predict customer churn.
We will perform some visualizations before we go on to pre-process the data, after which we will implement classification models.

# Thenchical Understanding

Here we have used various machine learning algorithms for the completion of this project.

*LOGISTIC REGRESSION

This is a machine learning technique that is mostly used in solving classification issues. It predicts answers after analysis based on probabilistic ideas. The classification algorithm Logistic Regression is used to predict the likelihood of a dependent variable. The dependent variable in logistic regression is a binary coded variable I.e. 1 or 0 where 1 usually represents true or yes etc. and 0 represents false or no etc.

This technique works on all kinds of datasets but for greater accuracy there are some conditions required to be satisfied:

1. The dependent variable must be binary.
2. The variables required for the model should be the only ones added to it.
3. There should not be any multi-collinearity in the model.
4. The sample size must be large.

*RANDOM FOREST CLASSIFIER

Supervised technique is a part of machine learning and random forest falls under this category. We can use this classifier for both regression as well as classification base ML problems. This classifier is heavily based on the ensemble learning concept. In ensemble learning multiple various types of classifier are combined to improve model performance.
Random forest is a classifier were many numbers of decision tree created on various sub parts of the dataset are connected. The final predicted accuracy is calculated by taking the average.

Many researchers and programmers use random forest as:

1. The training time required for this model is very less than other algorithms.
2. The model usually predicts the output with much higher accuracy than most models.
3. It works well and efficiently on large dataset.
4. This algorithm maintains the accuracy even if some of the dataset variables are not available.

*K NEAREST CLASSIFIER

This algorithm falls under supervised learning and is used for classification as well as regression problems. It is primarily used to input the missing values and to resample the datasets.
Here K is a random value and KNN (K Nearest Neighbor) as we can understand from the name it takes into consideration K Nearest Neighbors to predict the value of the new data entry.

The algorithm’s learning is:
1. Instance-based learning: In this type of learning we do not take weights into consideration for predicting the output (as opposed to model- based algorithms) instead we use the entire training data for predicting the output  on unseen data.
2. Lazy Learning.
3. Non –Parametric.

*GEOSPATIAL ANALYSIS

We have 388 rows of data, but only 77 unique coordinates, which indicates that either there are only 77 customers in this data set, or the lat-lon location is not exact and adheres to a certain area. Since this dataset is derived from a survey, we can assume the latter. This is also substantiated by the fact that there are 77 unique pin codes in the dataset.

# OBSERVATION FROM CONFUSION MATRIX

We notice that not only are features from 'Ease and convenient' to 'Good Tracking system' correlated with our output variable, but also with each other. In fact, if we observe the diagonals, we can see which features are correlated with each other, which gives us an insight as to how we can compress the multiple dimensions in our variables. One of the popular dimensionality reduction methods, principal component analysis will not help in this case because the variables are of ordinal categorical nature rather than continuous. We will use other feature selection methods later in the data pre-processing stage.

# CONCLUSION

Out of all models created, Random Forest and K Nearest Neighbors give the best performance. K Nearest Neighbors has the added advantage of being relatively simpler to interpret, without any sacrifice in accuracy.

![image](https://user-images.githubusercontent.com/62097113/149714284-c9639163-d3d2-4266-aea6-060488be992b.png)

Another consideration is about the data itself. We see that most of the variables that have a material impact on customer churn relate to broad aspects of ease and convenience. In fact, the subset of features selected in the model could inform business decisions, regarding which aspects of the service could be focused on for minimizing churn, and what user segments should the marketing dollars be spent on.


# FUTURE SCOPE

1. To extract even more out of the data set, we could further explore other dimensionality reduction methods, such as multiple correspondence analysis which solves the issue of principal component analysis not being suited to categorical data.

2. We ignored the text data, i.e. reviews in this analysis, and analyzing with NLP methods could also add to the analysis.

3. We could tune the model further by adding/subtracting variables.
