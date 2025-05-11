# multivariable_LinearRegression
Multivariable Linear Regression is an extension of simple linear regression, where the goal is to predict a dependent variable (target) using multiple independent variables (predictors). It models the relationship between the target variable and several predictors by fitting a linear equation to observed data.


#### 1. **Linear Relationship**:

* In multivariable linear regression, the assumption is that the target variable ($y$) is linearly dependent on the independent variables ($x_1, x_2, \dots, x_n$).
* The relationship between the target and the predictors is expressed as a linear equation.

#### 2. **Equation**:

The general form of the multivariable linear regression model is:

$$
y = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \dots + \beta_n x_n + \epsilon
$$

* $y$ is the dependent variable (target).
* $x_1, x_2, \dots, x_n$ are the independent variables (features or predictors).
* $\beta_0$ is the intercept (constant term).
* $\beta_1, \beta_2, \dots, \beta_n$ are the coefficients (weights) associated with each predictor.
* $\epsilon$ is the error term (residuals), which represents the difference between the predicted and actual values of $y$.

#### 3. **Objective**:

The goal of multivariable linear regression is to find the values of the coefficients $\beta_0, \beta_1, \dots, \beta_n$ that minimize the error term $\epsilon$, which is the difference between the observed values and the predicted values. This is done using a method called **Ordinary Least Squares (OLS)**.

#### 4. **Ordinary Least Squares (OLS)**:

* **OLS** is a method used to estimate the coefficients of the regression model by minimizing the sum of the squared differences between the observed and predicted values.
* The error term is calculated as:

  $$
  \epsilon = y - (\beta_0 + \beta_1 x_1 + \beta_2 x_2 + \dots + \beta_n x_n)
  $$
* The goal is to minimize the sum of squared errors:

  $$
  \text{Sum of Squared Errors (SSE)} = \sum_{i=1}^{m} (y_i - \hat{y}_i)^2
  $$

  where $\hat{y}_i$ is the predicted value for the $i$-th observation.

#### 5. **Assumptions**:

Multivariable linear regression relies on several assumptions:

* **Linearity**: The relationship between the target variable and the independent variables is linear.
* **Independence**: The residuals (errors) are independent of each other.
* **Homoscedasticity**: The variance of the residuals is constant for all values of the independent variables.
* **Normality**: The residuals are normally distributed.
* **No multicollinearity**: The independent variables should not be highly correlated with each other.

#### 6. **Evaluating the Model**:

* Once the model is trained, its performance can be evaluated using different metrics:

  * **R-squared**: Measures the proportion of the variance in the target variable that is explained by the independent variables.
  * **Adjusted R-squared**: A modified version of R-squared that adjusts for the number of predictors in the model.
  * **Mean Squared Error (MSE)**: The average of the squared differences between the actual and predicted values.
  * **Root Mean Squared Error (RMSE)**: The square root of the MSE, which provides a more interpretable measure of error in the same units as the target variable.

#### 7. **Applications**:

Multivariable linear regression is widely used in many fields such as:

* **Econometrics**: Predicting economic indicators.
* **Healthcare**: Predicting medical outcomes based on multiple factors.
* **Marketing**: Analyzing customer behavior based on multiple factors (e.g., income, age, etc.).
* **Engineering**: Modeling physical processes that depend on multiple variables.

#### 8. **Limitations**:

* Multivariable linear regression can suffer from **multicollinearity** if the predictors are highly correlated with each other.
* The model assumes that the relationship is linear, which may not always be the case.
* The presence of outliers can heavily influence the model, making it less robust.

In summary, multivariable linear regression helps in understanding the relationship between multiple predictors and a continuous target variable, allowing predictions based on new data. However, it's crucial to check the underlying assumptions and assess the model's performance before using it for decision-making.
