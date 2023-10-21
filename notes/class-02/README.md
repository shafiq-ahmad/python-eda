# Class 02: Exploratory Data Analysis (EDA)

## Steps in EDA

1. Import data
2. Big picture
    - df.dtypes
    - df.info()
        - get datatypes, and total entries, and missing values
        find missing values
        - df.isnull().sum()
        - get percentage of null values
        - df.isnull().sum() * 100 / len(df)

## Rules of data science

- in many cases if percentage of any column is more than 70% or 75% that column become value less
- depend on scenario so usually drop column of missin values
- if percent of missing value is less than 2% then remove those rows
- for rest impute with 3-4 ways
  - replace with average
  - replace with mean
  - replace mod

## Replace null values

Replace with mean of stat

```python
df2 = df['age'].fillna(df['age'].mean())
```

technique replace with mode
drop column with

```python
df['field'].fillna(df['field'].mode()[0], inplace=True)
```

## Definitions of mod, mean, median

- mean: average
- median: when arranged
  - the centered value is median
  - if odd values then center two values average
- mode: max number of occurance of a number
  - if it is more two then both are mod and we will pick first

## Steps

- Import
- Dataset
- Explore your data
  - Information
  - datatypes
  - missing values
  - take sense of you data
- understanding the variable
- relationship between the variable (headmap, pairplot,correlation)
- brainstroming
  - Normalize: to remove the difference
    - method finding: assignment
  - Removing outliers
    - how to remove them
  - Tidy data, clean data we got
    - ready for statistic analysis
    - ready for machine learning
    - ready for DL

## Dealing with missing value EDA analysis

Categorial / object, numeric
