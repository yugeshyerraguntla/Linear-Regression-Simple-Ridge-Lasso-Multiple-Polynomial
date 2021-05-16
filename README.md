# Linear-Regression-Simple-Ridge-Lasso-Multiple-Polynomial
This repo contains Linear Regression - Simple, Ridge,Lasso,Multiple,Polynomial, Visualize Multi etc.

## 1. Linear Regression:
  - We have our features as independent variables, on which our target variable is dependent upon.
  - y=mx+b    (traditional slope-intercept form, where m and b are the variables our algorithm will try to “learn” to produce the most accurate predictions. x-input y-prediction.)
  - Multivariate: f(x,y,z)=w1x+w2y+w3z
 
 - Cost Function: We need to find the BEST FIT line. Many lines are possible but bet fit line has minimum error.
 - MSE=1/N ∑i=1->n (yi−(mxi+b))^2
 - Our goal is to minimize MSE to improve the accuracy of our model.
 
 - Gradient Descent: To minimize MSE we use Gradient Descent to calculate the gradient of our cost function.
 - Arrive at Global Minima. Use Convergance theorem to arrive slowly. 
 - Learning Rate (α) should be precise. *Select α small. If α is big, we may overshoot.*

https://www.analyticsvidhya.com/blog/2017/06/a-comprehensive-guide-for-linear-ridge-and-lasso-regression/
https://ml-cheatsheet.readthedocs.io/en/latest/linear_regression.html

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
fit() model estimates the prameters and returns model information to variable:

**Model Diagnostics:**

1. R^2 - Coeff. of Determination: R^2 = SSR/SST = Explained Variation/Total Variation. Lies btw 0-1 and Higher R^2, better the fit.
2. Hypothesis Test for Regression Co-Efficient 
3. ANOVA - Analysis Of Variance F=MSR/MSE
4. Residual Analysis: 1. P-P Plot and Residual Plot
5. Outlier Analysis:
  - Z Score: If > 3; Outlier
  - Cooks Distance: If > 1; Outlier
  - Leverage Values: Graph with bubbles
  - Mahalanobis Distance

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 2. ## 
In case of Linear Regression, due to low training data, cost function can give 0 with training data. But with test data, it will give error.
    This causes 'OverFitting.'
     OverFitting -> High Variance
     With help of Ridge and Lasso, -> we can reduce Variance.
     
- __Ridge__: RSS + α * (sum of square of coefficients)
- __Lasso__: RSS + α * (sum of absolute value of coefficients)

Penalizing the features with higher slopes. 
Lasso Reg helps with overfitting problem and also with feture selection.

***Use Lasso if we have more number of Features
***Use Ridge if we have strong relationship b/w features

https://www.analyticsvidhya.com/blog/2016/01/ridge-lasso-regression-python-complete-tutorial/


3. Multiple Linear Regression:
Multiple linear regression (MLR), also known simply as multiple regression, is a statistical technique that uses several explanatory variables to predict the outcome of a response variable. 
y=β1x1+β2x2+⋯+βnxn+β0
3D Space - Look at Propensity and Brittleness
https://aegis4048.github.io/mutiple_linear_regression_and_visualization_in_python

4. MultiCollinearity: In regression, "multicollinearity" refers to predictors that are correlated with other predictors. Multicollinearity occurs when your model includes multiple factors that are correlated not just to your response variable, but also to each other. In other words, it results when you have factors that are a bit redundant




