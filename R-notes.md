t is the matrix transpose function

outer is the outer product of two vectors according to some function f,
where the outer function forms a 2D matrix where the (i,j)th entry is the result
of applying f(i,j)

# Linear Regression
Syntax for creating Linear regression plots is:
lm.fit = lm(y~x1+x2+x3, data=DATA)

To do all of the regressions at once, syntax is:
lm.fit = lm(y~., data=DATA)

## Understanding Diagnostic Plots for Linear Regression Analysis
1. Residuals vs Fitted
    - You want to see a horizontal line without distinct patterns
    - Otherwise, you have non-linear relationships

2. Normal QQ plot
    - You want to see it follow the diagonal line, if not you have deviation
      from the assumption of normality and thus a lot of assumptions don't work. 

3. Scale-Location plot
    - This plot shows if residuals are spread equally along the ranges of
      predictors. This is how you can check the assumption of equal variance
      (homoscedasticity).
    - It's good if you see a horizontal line 

4. Residuals vs Leverage
    - Helps in identifying influential outliers
    - Points which have a high residual value and high leverage are worth
      looking at.
    - You want to find cases that lie outside the the Cook's distance line 


