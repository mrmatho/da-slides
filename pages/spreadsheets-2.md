---
layout: cover
transition: fade
hideInToc: false
background: /img/stats.webp
---

# Descriptive Statistics in Spreadsheets

---
layout: li
---
::li::
- To be able to use spreadsheets to calculate descriptive statistics,(average, median, minimum, maximum, range, standard deviation, count/frequency, sum)
- To be able to interpret the results of descriptive statistics for a given data set.

::sc::
- Calculate each of the studied descriptive statistics in Microsoft Excel
- Interpret the values of each of the descriptive statistics calculated

---
layout: center
---
# Descriptive Statistics

Descriptive statistics are used to describe the basic features of the data in a study. They provide simple summaries about the sample and the measures. Together with simple graphics analysis, they form the basis of virtually every  analysis of data.

The descriptive statistics we study fall into three categories:

- Measures of Central Tendency (Averages)
    - Average (Mean)
    - Median
- Measures of Spread (Variability)
    - Minimum & Maximum
    - Range
    - Standard Deviation
- Measures of Size (Frequency)
    - Count
    - Sum 

Each of these measures is applied to <span v-mark.circle.green>numerical data</span> to provide a summary of the data set.

---
layout: two-cols-header
---

# Average and Median

::left::

## Average (Mean)

- Described in Applied Computing as Average, but mathematically as the mean.
- The sum of all values divided by the number of values.
- The most common measure of central tendency.
- Can be affected by outliers
    - Which may not be representative of the data set
- Can be calculated using the `AVERAGE` function in Excel eg. `=AVERAGE(A1:A10)`

::right::

## Median

- The middle value of a data set.
- The median is not affected by outliers.
- Can be calculated using the `MEDIAN` function in Excel eg. `=MEDIAN(A1:A10)`
- If there are an even number of values, the median is the average of the two middle values.
- Also represents the 50th percentile of the data set.

---
layout: two-cols-header
---

# Minimum and Maximum

::left::

## Minimum

- The smallest value in a data set.
- Can be calculated using the `MIN` function in Excel eg. `=MIN(A1:A10)`
- Can be used to identify the range of values in a data set.

::right::

## Maximum

- The largest value in a data set.
- Can be calculated using the `MAX` function in Excel eg. `=MAX(A1:A10)`
- Can be used to identify the range of values in a data set.

---
title: Range and Standard Deviation
layout: two-cols-header
---

# Range and Standard Deviation

Measures of spread (such as range and standard deviation) provide information about the variability of the data set. Two data sets could have very similar averages but very different ranges or standard deviations, indicating that one data set is more spread out than the other.

::left::

## Range

- The difference between the maximum and minimum values in a data set.
- Can be calculated using the `MAX` and `MIN` functions in Excel eg. `=MAX(A1:A10) - MIN(A1:A10)` (Not able to be calculated on its own)
- Provides a measure of the spread of the data set.
- Can be affected by outliers.

::right::

## Standard Deviation

- A measure of the amount of variation or dispersion of a set of values.
- Can be calculated using the `STDEV` function in Excel eg. `=STDEV(A1:A10)`
- The standard deviation is the square root of the variance.
- The variance is the average of the squared differences from the mean.
- Can be affected by outliers.

---
layout: two-cols-header
---

# Count and Sum

Count and sum are measures of size. Count provides the number of values in a data set, while sum provides the total of all values in a data set. It is important to consider whether the sum or count is relevant for the particular data values being analysed. If you cannot explain what the sum or count represents, it is not useful.

::left::

## Count

- The number of values in a data set.
- Can be calculated using the `COUNT` function in Excel eg. `=COUNT(A1:A10)`. This counts the number of cells in a range that contain numbers (ignores empty cells).
- Can be used to identify missing data.
- Can be used to identify the size of a data set.

::right::

## Sum

- The total of all values in a data set.
- Can be calculated using the `SUM` function in Excel eg. `=SUM(A1:A10)`
- Can be used to identify the total of a data set.

---
layout: center
---

# Your Turn

Answer in your book

The tables below show the descriptive statistics for the number of goals scored by two football teams in each of their games across the season. Compare the two teams using the descriptive statistics provided.

| Croydon City | Mitcham Monarchs |
|--------------|------------------|
| Mean: 2.5    | Mean: 3.0        |
| Median: 2    | Median: 3        |
| Min: 1       | Min: 1           |
| Max: 4       | Max: 5           |
| Range: 3     | Range: 4         |
| Std Dev: 0.5 | Std Dev: 1.0     |
| Count: 4     | Count: 5         |
| Sum: 10      | Sum: 15          |

<style>
th {
  background-color:rgb(164, 160, 160);
  font-weight: bold;
  border: 1px solid black;
  padding: 2px 10px;
}

td {
  border-collapse: collapse;
  border: 1px solid black;
  padding: 0px 10px;
}

</style>