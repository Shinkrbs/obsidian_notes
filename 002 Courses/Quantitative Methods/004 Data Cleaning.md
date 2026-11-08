Tags: #DataCleaning #Quantitative #QuantitativeMethods

------

## What is Data Cleaning?

- The process of **detecting, diagnosing, and correcting errors, inconsistencies and quality issues** in a dataset so that it is *accurate, complete, and suitable for analysis*.
- Also called **data wrangling or data scrubbing.**

## Why Raw Data is Almost Never Clean 

- Survey respondents skip questions or enter nonsensical values
- Sensors or instruments malfunction, producing erroneous readings
- Data entry operators make typos and format inconsistencies
- System migrations introduce encoding errors and structural changes
- Multiple data sources use different conventions (date formats, units, namings)

## The Golden Rule

- Garbage in, Garbage Out (**GIGO**)
- No statistical method can compensate for poor data quality
- A perfectly executed analysis on dirty data produces wrong conclusions

## Five Types of Data Quality Issues

- **Missing Data**: Values that were not recorded or were intentionally left blank
- Can appear as empty cells, NULL< NaN, -999. or N/A
- **Duplicate Records**: The same observation appears more than once - caused by double submissions, ETL errors, or merging overlapping datasets
- **Inconsistent Format:** The same variable is recorded in multiple formats across rows, making comparison or computation impossible without standardization
- **Invalid Types**: Values that are syntactically present but logically impossible or out of range for the variable

## Standard Profile Checks

- **Row and column counts**  - Confirm expected dimensions; unexpected row count suggests duplicates or missing data
- **Missing value count per column** - Flag any column with > 5% missing values for investigation
- **Unique value count for categoricals** - Detects format inconsistencies 
- **Min/Max/Range check** - Catches out-of-range values and extreme outliers immediately
- **Duplicate Row Detection** -  Exact and near-duplicate identification
- **Data Type Check** - Confirms numeric columns did not import as text; date columns parsed correctly
