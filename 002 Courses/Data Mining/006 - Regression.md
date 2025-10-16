Tags: #Regression #RegressionModel

**Regression Model*** provides a function that describes the relationship between one or more independent variables and a response, dependent, or a target variable

**Regression Analysis** is the basis for many types of prediction and for determining the effects on target variables. 

**Types of Regression**

1. Linear
2. Multiple
3. Non-Linear
4. Stepwise Regression Modeling

*For this topic, the types that will be used are: Linear and Multiple.*

**Linear**: a linear regression is a model where the relationship between inputs and outputs is a straight line. 

**Linear Regression** finds the line of best fit line through your data by searching for the regression coefficient (**B1**) that minimizes the total error (**e**) of the model.

**Multiple**: a multiple regression indicates that there are more than one input variables that may affect the outcome, or target variable. 

---
## Simple Linear Regression

**Formula for Simple Linear Regression**

![[Pasted image 20251017004231.png]]

- **y** is the predicted value of the dependent value variable (**y**) for any given value of the independent value (**x**)
- **B0** is the **intercept**, the predicted value of **y** when the **x** is 0.
- **B1** is the regression coefficient – how much we expect **y** to change as **x** increases.
- **x** is the independent variable ( the variable we expect is influencing **y**).
- **e** is the **error** of the estimate, or how much variation there is in our estimate of the regression coefficient.

---
## Excel Stuff

- `SUMSQ`: Sum of squares, first squares each number in a range, and then adds up those squares
- `COUNTA`: Counts any cell that is not empty. Includes numbers, text, error values, and even cells that contains a formula returning an empty string. It only ignores truly blank cells.
---
## MSE Formula for Excel

**Mean Squared Error (MSE)**: is an estimate that measures the average squared difference between the estimated values and the actual values of a data distribution. It calculates the average squared differences between the points and the regression line. That is, the mean of the squares of the residuals.

- Find Difference: ` Difference = Forecasted - Actual`
- Square the Difference and find Average to get MSE: `MSE = Average(Difference * Difference)`

---
## RMSE Formula for Excel

**Root Mean Square Error (RMSE)** is a metric that tells us how far apart our predicted values are from our observed values, on average.

- Find Difference: ` Difference = Forecasted - Actual`
- Use Formula `SQRT(SUMSQ(rows) / COUNTA(rows))`

## How to Interpret RMSE

- **RMSE** is a useful way to see how well a regression model is able to "fit" a dataset. 
- The **larger** the RMSE, the larger the difference between the predicted and observed values, which means **worse** the regression model fits the data.
- The **smaller** the RMSE, the better a model is able to fit the data

---
## MAE Formula for Excel

**Mean Absolute Error** is the measure of error between the observed and the expected values in a given data set.

- Find Difference: ` Difference = Forecasted - Actual`
- Calculate Absolute Values: `ABS(row of Difference)`
- Calculate for MAE: `MAE = AVERAGE(rows of ABS)`

---
## Linearity Test

**Normality Test**: Check whether the dependent variable follows a normal distribution (bell).

	`hist(income.data$happiness)`

FUCK THIS SHIT