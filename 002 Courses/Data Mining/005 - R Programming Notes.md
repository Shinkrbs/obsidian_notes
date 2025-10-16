Tags: #R #RProgramming #RSyntax #Syntax 

- Assign a value to a variable: **x <- value**
- Create a vector: **c(value, value, value)**
- Generate Regression Line: **x <- lm(child ~ parent, galton)**
- See a more concise display of the regression data: **summary(x)**
- Check mean of specific variables: **mean(x$residuals)**
- Check correlation between specific variable (change residuals): **cov(x$residuals, galton$parent)**
- Test for equality: all.eqal(var1, var2)
- Compute the correlation between sets: **cor(set1, set2)**
- Look at the sigma portion of the summary of var: **summary(var)$sigma**
- Library for Metrics:(MSE, RMSE, MAE)
	- `install.packages("MLmetrics")`
	- `library(MLmetrics)`
- Find MSE: 
	- First find predictions: `y_pred <- predict(income.happiness.lm, income.data)`
	- Extract Actual Data: `y_true <- income.data$happiness`
	- Find MSE: `MSE(y_pred, y_true)`

---
# Simple Linear Regression

*The data used is titled **income.data.***

- For simple linear regression: `income.happiness.lm <- lm(happiness ~ income, data = income.data)`
- Equation for the linear model: `lm()`
- Get forecast/predicted data: `y_pred <- predict(income.happiness.lm, income.data)`
- Extract Actual Data: `y_true <- income.data$happiness`
