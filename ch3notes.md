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

## Multiple Linear regression
    There are four fundamental questions in multidimensional linear regression. 
    1. Is there enough evidence to believe that at least one of the variables
       is correlated with the output variable
    2. If (1) is true, then which variables are correlated with the output
       variables?
    3. After finding the best model, how well does this model fit the dataset?
    4. Given a set of predictor values, 

Solutions:
    1. Use the F-Statistic, and see if it is greater than 1. 
    2. This is not an easy problem, and will be covered in greater depth in ch6.
       However, the idea is to do an iterative approach by seeing which
       variables have the lowest p-value and adding them to some model, then
       judging the model by some statistical criterion. 
    3. Related to 2, is used in the asnwer
I stopped at page 75

