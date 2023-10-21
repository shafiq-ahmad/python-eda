# Class 04: Missing values

Configure VS Code to open conda in VS Code Terminal. Follow below steps

- Press `ctrl+,` for settings
- Search for setting 'Conda path'
- Save the path here as following and close
  - >C:\Users\username\miniconda3
- `Ctrl+Shift+P`: Select python interpreter
- Open the terminal from above. Note that it will run only in `cmd.exe` not `powershell`

Missing values rules

- If too much missing value remove them mostly (if more than 50% and field isn't important)

See exercise file [Click Here ...](../../exercise-files/class-04/missing-values.ipynb)

## Explore the Data

- Feel the Data
- Find out who gathered the Data (the source)
- What is this data about
- find Meta data. eg what are meaning of column name and what they hold, and what value means
- find data dimension by `info()` function.

### Find the following 4 things of data

- Composition of data
- Correlation: 1 0 -1
  - Highly correlative: 0.5 or more
  - Highly correlative negitive:  -0.5 or less

- Comparison: using group by function
- Distribution of data

### Descriptive data analytics

When using above 4 methods are used to analyze the data then its called

Diagostic: is when handling missing value with above

### EDA is also called

- Data exploration
- Data wranggling
- data munging
- data pre processing
- data cleaning

## Statistical terms

- Mean: The mean (average) of a data set is found by adding all numbers in the data set and then dividing by the number of values in the set
- Median: The median is the middle value when a data set is ordered from least to greatest
- Mode: The mode is the number that occurs most often in a data set.

## Methods to impute the missing values

- Mean/median/mode imputation: This involves replacing missing values with the mean, median, or mode of the non-missing values in the column.
- K-nearest neighbors imputation: This method finds the k most similar rows to the row with the missing value and replaces the missing value with the average of the non-missing values in those k rows. This is more accurate than last one.
- Multiple imputation: This method creates multiple imputed versions of the dataset, each with the missing values replaced using a different imputation method. It can be more accurate and unbias
- Regression imputation: This involves using a regression model to predict the missing values based on the non-missing values in the dataset.
- Interpolation: This involves using a statistical method to estimate the missing values based on the neighboring values.
- Pattern substitution: This involves identifying patterns in the data and using those patterns to impute the missing values.
- Maximum likelihood estimation: This statistical method estimates the missing values in a way that maximizes the likelihood of the observed data.
