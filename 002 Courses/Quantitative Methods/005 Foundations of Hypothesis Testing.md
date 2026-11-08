Tags: #Hypothesis #HypothesisTesting


### Statistical Inference

- process of using sample data to draw conclusions about an unknown population parameter
- quantifying the probability that those conclusions are wrong

### Sampling Variability

- the natural variation in statistics (e.g., sample means) that occurs when different random samples are drawn from the same population
- Even under identical conditions, no two samples are exactly the same

### Hypotheses and the Significance Level

- **Null Hypothesis (H0)**: the no-effect claim; the default assumed true until evidence shows otherwise.
- **Alternative Hypothesis (H1)**: the research claim; what we expect to find
- **Level of Significance**: the maximum probability of wrongly rejecting null hypothesis that the researcher is willing to accept. It is set before data collection, not after.

**LEVEL OF SIGNIFICANCE**
![[{AC62B416-7BA8-4841-B648-505091DE281E}.png]]

- Must be chosen before collecting data - changing level of significance after seeing results is p-hacking.
- Lower level of significance -> stricter standard -> harder to reject the null hypothesis -> fewer false positives but more false negatives

### The p-Value

- the probability of obtaining a test statistic as extreme as, or more extreme than, the one observed in our sample, given that Null Hypothesis is true.
*![[{26A49D31-7DE4-4C62-8784-68A0287ACECB}.png]]

### Type I and Type II Errors

![[{36CA9233-E32F-4023-9CE7-01D0F5BA4880}.png]]

**Type I Error (False Positive)**: You reject the null hypothesis when it is actually true. This means your test claims there is a real effect, but in reality, there is no effect. 

**Type II Error (False Negative)**: You fail to reject the null hypothesis when it is actually false. This means your test claims there is no effect, but in reality, an effect does exist. 

**The trade-off**: Decreasing level of significance (stricter) reduces Type I errors but increase Type II errors. You cannot minimize both simultaneously without increasing sample size.

### The 5-Step Hypothesis Testing Procedure

1. State the hypothesis
2. Set the significance level
3. Select the appropriate test 
4. Compute the test statistic
5. State the conclusion in context

### Two-Tailed Test (Non-Directional)

- H₁: μ₁ ≠ μ₂
- The effect could go either direction. The critical region is split equally between both tails of the distribution
- ![[{DE0EC518-425E-45F5-A730-7C7945FD2913}.png]]
- Critical region = level of significance / 2 in each tail, Use when direction is unknown

### One-Tailed Test (Directional)

- H₁: μ₁ > μ₂ (right-tailed)
- The effect is expected in a specific direction
- The entire critical region of level of significance is in one tail - making the test more powerful for detecting that direction
- ![[{0B33FD20-A895-4EEF-BF47-9E10164E040D}.png]]
- Full level of significance in one tail, Use only when direction is theoretically justified

### One-Tailed vs Two-Tailed Tests

- Default two-tailed unless prior literature strongly supports a specific direction
- A one-tailed test cannot detect an effect in the opposite direction - and surprising findings in the "wrong" direction have scientific value

### Parametric Tests

- Statistical Tests (t-test, ANOVA, Pearson Correlation) that make specific assumptions about the population distribution
- Violating these assumptions may invalidate the test results

### Parametric Tests (Core Assumptions)

- Normality - The dependent variable (or residuals) is approximately normally distributed in the population
- Independence - Observations are independent of each other; no subject appears in multiple conditions simultaneously
- Homogeneity of Variance - for tests comparing groups, the variances of the groups are roughly equal (homoscedasticity)
- Scale of measurement - Data must be interval or ratio scale for parametric tests to be valid
- ![[{2862845A-5A08-42B7-82F4-56A97526DAA4}.png]]
- Always check assumptions before running a test
- The Shapiro-Wilk test (normality) and Levene's tests (equal variance) are the standard assumption checks