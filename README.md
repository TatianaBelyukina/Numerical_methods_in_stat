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
