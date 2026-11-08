Tags: #ParametricTests #T-Tests

### T-Test

- A statistical tool for comparing the mean of a dataset

### Types of T-Tests

1. One-Sample T-tests: Does the sample mean differ significantly from a known or hypothesized population mean?
   - 1 sample size vs. a fixed value
2. Paired Samples T-Test: Is there a significant difference between two measurements on the same subjects?
   - 1 group measured twice (before/after)
3. Independent Samples T-Test: Do two independent groups have significantly different means?
   - 2 separate, unrelated groups


### One-Sample T-Test

- Tests whether the mean of a single sample is significantly different from a specified population mean
- Used when population mean is known from prior research industry standards, or SLA benchmarks.

#### Assumptions

- Scale: Interval or Ratio Data
- Normality: Population is approximately normal or n >= 30
- Independence: Observations are independent of each other
- Known population mean: The reference population mean is specified from theory, standards, or prior work - not estimated from the same data

#### Hypotheses

![[{4B5B1E5B-E6D9-4546-87E1-A8F2ED76BC79}.png]]


### Paired-Sample T-Test

- Tests whether the mean of the within-subject differences (d = x1 - x2) is significantly different from zero
- Treats each matched pair as one observation
- Use paired t-test whenever the same subjects or matched units are measured under both conditions - it always has more power than an independent t-test for the same data.

#### Assumptions

- Paired design: each observation in group 1 has a corresponding observation in group 2 (same subject, matched pair, or same unit)
- Scale: Interval or Ratio
- Normality of differences: the d values(not the raw scores) are approximately normally distributed 
- Independence of pairs: each pair is independent of other pairs (no repeated measures structure beyond two time points)

### Independent Sample T-Test

- Tests whether two independent groups have significantly different population means
- Each observations belongs to exactly one group, with no relationship between observations across groups

#### Assumptions

- Scale: Interval or ratio data in both groups
- Normality: Both groups are approximately normally distributed (or n1, n2,  >= 30)
- Independence: The two groups are completely separate; no subject appears in both
- Homogeneity of variance: Test with Levene's Test

### Comparing the Three T-tests

![[{825E540C-07FC-4E19-B012-B25F8E145F55}.png]]