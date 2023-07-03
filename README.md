# Numerical_methods_in_stat
Projects were made using R language
# lab1.ipynb


"Mammals" dataset analysis for building a regression model
1. Outliers analysis, data logarithmization
2. Shapiro-Wilk normality test
3. Residuals analysis(QQ-plot, Skewness, Kurtosis, Heteroscedasticity)


# lab2.ipynb

Findinf the optimal set of regressors for predicting the mpg value in the mtcars dataset

Detection of collinearity

1. The main problem with multivariate regression is collinearity. If two or more predictor variables are highly correlated and they are both entered into a regression model, this inflates the true standard error and you get very unstable slope estimates. We can estimate collinearity by the variance inflation factor (VIF). Let's look at the variance inflation factors if we add all the variables to the model. VIF = $\frac{1}{1-R^2_j}$
2. Staged selection method

Among the available methods, we chose to perform a stepwise selection to help us select the subset of variables that best explain MPG. This test is performed using the Akaike information criterion
3. Nested likelihood ratio test

# lab3.ipynb
The purpose of the work: to derive a formula for classifying the sex of sparrows
1. Resampling with return for imbalanced data
2. Using the lda function, we perform linear discriminant analysis
3. Although the training data gives a slightly better result in the quadratic discriminant analysis, it is worth noting that in the test we got a very large error for females, that is, overtraining took place. So, we leave the linear approach. Let's write down the formula for gender classification.
Let the vector v = (v1, v2, .., v10) - a set of features for a certain sparrow, ld - a vector obtained during linear discriminant analysis, that is, a vector on which we will project points from 10-dimensional space, then the projection: $proec_v = v1*ld1 + ... + v10*ld10$.Threshold for classification: $treshold = 0.5*(m1 + m2)$,where m1 is the mean value of males on ld, and m2 is the mean value of females on ld. 1 - male, 0 - female $f = \begin{cases} 1, & proec_v > treshold \\ 0, & proec_v < treshold  \end{cases}$ Specifically for our case ld = (0.61408642,
-0.03368088,
0.26926476,
0.02444667,
-0.37714267,
-33.17219503,
-0.29803378,
-10.39953553,
5.99321982,
20.23730007), a treshold = 33.6399679291373

# lab4.ipynb
The purpose of the work: using clustering methods to find out whether 3 species of trilobes are different from each other

1. Elbow method for pivking up the best number of clusters(3 in our case)
2. K-means clustering
   
