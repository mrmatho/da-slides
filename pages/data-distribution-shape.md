---
title: Shape of Data Distributions
description: Understanding the shape of data distribution is crucial for effective analysis and modeling.
layout: li
hideInToc: false
transition: fade
---

::li::
- To be able to identify and interpret the shape of data distribution.
- To understand the implications of different distribution shapes on data analysis and modeling.

::sc::
- Identify the shape of the given data distribution using visualizations in Excel

---
layout: center
---

# Measures of Shape

(from the Australian Bureau of Statistics)

Measures of shape describe the distribution (or pattern) of the data within a dataset.

The distribution shape of quantitative data can be described as there is a logical order to the values, and the 'low' and 'high' end values on the  x-axis of the histogram are able to be identified. 

The distribution shape of a qualitative data cannot be described as the data are not numeric.

|Shape|Description|
|---|---|
|Symmetrical|The left and right sides of the distribution are mirror images of each other.|
|Positively skewed|The tail on the right hand side of the histogram is longer than the left side. More of the values cluster towards the smaller end of the x axis.|
|Negatively skewed|The tail on the left hand side of the histogram is longer than the right side. More of the values cluster towards the larger end of the x axis.|

---
layout: center
---

# Symmetrical Distribution

```mermaid {scale: 0.7}
xychart-beta
    title "Sales Revenue"
    x-axis  0 --> 12
    y-axis "Revenue (in $)" 0 --> 11000
    bar [2000, 6000, 7500, 8200, 9500, 10500, 11000, 10200, 9200, 8500, 5000, 3000]
    line [2000, 6000, 7500, 8200, 9500, 10500, 11000, 10200, 9200, 8500, 5000, 3000]
```

Note: The left and right sides are very close to being mirror images of each other. They aren't exactly the same, but there is a clear pattern.

---
layout: center
---
# Positively Skewed Distribution

```mermaid {scale: 0.7}

xychart-beta
    title "Sales Revenue"
    x-axis  0 --> 12
    y-axis "Revenue (in $)" 0 --> 11000
    bar [5000, 6000, 7500, 9200, 8500, 7500, 5000, 3000, 2100, 1200, 500, 600]
    line [5000, 6000, 7500, 9200, 8500, 7500, 5000, 3000, 2100, 1200, 500, 600]
```
Note: The tail on the right hand side of the histogram is longer than the left side. More of the values cluster towards the smaller end of the x axis.

---
layout: center
---
# Negatively Skewed Distribution

```mermaid {scale: 0.7}
xychart-beta
    title "Sales Revenue"
    x-axis 0 --> 12
    y-axis "Revenue (in $)" 0 --> 11000
    bar [1200, 3000, 5000, 6000, 7500, 8200, 9500, 10500, 11000, 10200, 9200, 5000]
    line [1200, 3000, 5000, 6000, 7500, 8200, 9500, 10500, 11000, 10200, 9200, 5000]
```
Note: The tail on the left hand side of the histogram is longer than the right side. More of the values cluster towards the larger end of the x axis.

---
layout: center
---

# Creating a Histogram in Excel

1. Select the data you want to create a histogram for.
2. Click on the "Insert" tab in the Excel ribbon.
3. In the Charts group, click on the "Insert Statistic Chart" button.