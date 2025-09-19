Tags: #R #RProgramming #RSyntax #Syntax 

- Assign a value to a variable: **x <- value**
- Create a vector: **c(value, value, value)**
- Generate Regression Line: **x <- lm(child ~ parent, galton)**
- See a more concise display of the regression data: **summary(x)**
- Check mean of specific variables: **mean(x$residuals)**
- Check correlation between specific variable (change residuals): **cov(x$residuals, galton$parent)**
- Test for equality: all.eqal(var1, var2)