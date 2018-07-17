# Notes from Chapter 3
## Abbreviations used
    1. RSS - Residual sum of squares. --> This is basically the Squared Error
       (kinda like the variance) of your predictive line. 
    2. RSE - Residual Standard error. Kinda like the standard deviation of your
       predictive dataset. Strictly speaking, it is an *estimator* for the
       standard deviation of \ep, the unavoidable "noise" in the dataset from
       the true regression line. 
    3. R^2 Statistic - It is the amount of variability in your data set that can
       be explained by your regression line. Calculated as (1 - RSS / TSS),
       where TSS is the variance of the y-component of the dataset. 
    4. Residuals - Another word for error. It is the difference between the true
       value and the predicted value. 

## Multiple Linear regression
    There are four fundamental questions in multidimensional linear regression. 
    1. Is there enough evidence to believe that at least one of the variables
       is correlated with the output variable
    2. If (1) is true, then which variables are correlated with the output
       variables?
    3. After finding the best model, how well does this model fit the dataset?
    4. Given some fixed input vector (X), what response value should we predict,
       and how accurate is this value?

Solutions:
    1. Use the F-Statistic, and see if it is greater than 1. 
    2. This is not an easy problem, and will be covered in greater depth in ch6.
       However, the idea is to do an iterative approach by seeing which
       variables have the lowest p-value and adding them to some model, then
       judging the model by some statistical criterion. 
    3. Related to 2, is used in the answer


## Other notes:
Increasing the number of variables correlated must, by definition, increase the
R^2 value. However, it won't increase it by much and that's one way of
identifying useless variables? A way of quantifying what a "good" increase is,
is to use the p-value of the variable coefficient. 

For qualitative predictors with more than two levels, we use more indicator
random variables rather than use an indicator variable with different values.
For instance, if you wanted to encode that a certain person is Asian / Caucasian
/ Indian, you would use two dummy variables, rather than use one variable which
can take on 3 values. 

Which value you use as the baseline value doesn't affect much, but it does
affect the p-values (which decide whether Asian v Indian is statistically
significant). So, first you must do an F-test to determine that at least one
variable is significant.

## Issues with multiple regression
High leverage points vs Outliers:
    - Outliers are points in the training set for which the predicted value is
      far off from the actual value
    - High leverage points are points which have a large x value compared to the
      other points; this means that the point has a large impact on the least
      squares lines coefficients.

Collinearity - When two or more predictor variables are *very* strongly
correlated in the training set. This means that it is hard to know whether an increase in y is due to which one of those variables. 

## Linear Regression vs Naive KNN

The upshot is that for lower dimensional data, KNN is normally better, but for
higher dimensional data, Linear regression usually gives better results due to
the curse of dimensionality. 

What can we do about the curse of dimensionality affecting the results of the
KNN parametrization? 


