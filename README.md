# Linear-Regression-Simple-Ridge-Lasso-Multiple-Polynomial
This repo contains Linear Regression - Simple, Ridge,Lasso,Multiple,Polynomial, Visualize Multi etc.

1. Linear Regression:
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

2.  In case of Linear Regression, due to low training data, cost function can give 0 with training data. But with test data, it will give error.
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
