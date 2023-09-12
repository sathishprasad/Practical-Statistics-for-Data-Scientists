# Exploratory Data Analysis

---
## Elements of Structured Data
Data comes from many sources - sensor measurements, events, texts, images etc. Majority of these data are unstructured and to convert these data into actonable
information, the unstructured raw data needs to be processed and manipulated into a structured form. 

There are two basic type of structured data <br>
- Numeric data
- Categorical data

### Numeric data 
- Numeric data are data that are expressed on a numeric scale.
- Numeric data comes in two forms
  - __Continuous Data__
    - Data that can take on any value in an interval. Ex - Wind speed, time duration.
  - __Discrete Data__
    - Data that can take on only integer values. Ex - Count of occurance of event, age etc. 
### Categorical data
- Data that can take on only a specific set of values rpresenting a set of possible categories.(Synonyms: Enums,factors, nominal, enumerated)
- Categorical data comes in two forms
  - __Binary data__
    - A special case of categorical data with just two categories of values. Ex - 0/1,true/false,male/female etc.
  - __Ordinal data__
    - Categorical data that has an explicit ordering. Ex - Customer start rating of 1-5.

### Advantages of ordering the data
- Data typing in software acts as a signal to the software on how to process the data.
- Knowing the data is categorical can act as a signal to analysts on how to perform actions with the data.
- Storage and indexing can be optimised.

---
## Rectangular Data
The typical frame of reference for an analysis ind ata science is a rectangular data object, like a spreadsheet or database table. <br> </br>
It is called "rectangular" because it is organized into rows and columns, forming a grid-like structure. Each row represents a single data record or observation, and each column represents a different attribute or variable associated with those records.
It's also the specific format in R and Python.

### Key Terms for Rectangular Data
- __Data frame__ : A rectangular data(like spreadsheet) is the basic data strucutre for statisical and machine learning models.
- __Feature__ : A column within a table is commonly referred to as a feature.
  - __*Synonyms:*__ attribute, input, predictor, variable.
- __Outcome__ : Many data science projects involve predicting the outcome. The features are sometimes used to predict the outcome in an experiment.
  - __*Synonyms:*__ Dependent variable, response, target and output.
- __Records__ : A row within a table is commonly referred to as a record.
  - __*Synonyms:*__ case, example, instance, observation, pattern, sample.

### Data Frames and Indexes
Indexes are essential components of data frames, serving as unique labels or identifiers for rows. They enable efficient data retrieval and manipulation and can be numeric or alphanumeric, allowing for quick access to specific data points within the data frame.

### Nonrectangular Data Structures
Non-rectangular data structures are data formats that don't conform to the traditional tabular or grid-like structure of rows and columns found in rectangular data. These data structures are more flexible and can represent data in various forms, such as hierarchical, nested, or graph-like structures. One common example of a non-rectangular data structure is JSON (JavaScript Object Notation).

---
## Estimates of Location
Variables with measured or count data might have thousands of distinct values. A basic step in exploring your data is getting a *typical value* for
each feature.

Some of the estimates of location/point are:
- Mean
- Weighted Mode
- Median
- Percentile
- Weighted Median
- Trimmed mean
- Robust
- Outlier

### Mean
- The most basic estimate of location is the mean, or average value.
- The mean is the sum of all values divided by the number of values. 



|   Name   | Age |     City     |
|:--------:|:---:|:------------:|
|  Alice   |  25 |   New York   |
|   Bob    |  30 | Los Angeles  |
| Charlie  |  35 |   Chicago    |
|  David   |  28 |   Houston    |
Table 1: sample dataframe 

```python
#Implementation in Python
import pandas as pd

# Calculate the mean for the 'Age' column
age_mean = df['Age'].mean()

# Print the mean
print("Mean Age:", age_mean)
```
```R
# Calculate the mean for the 'Age' column
age_mean <- mean(df$Age)

# Print the mean
cat("Mean Age:", age_mean)
```

## Estimates of Variability 
## Exploring the Data Distribution
## Exploring Binary and Categorical Data
## Exploring Two or More Variables



