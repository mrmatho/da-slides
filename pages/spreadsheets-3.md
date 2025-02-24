---
layout: cover
transition: fade
hideInToc: false
background: /img/stats.webp
---

# Correlation in Spreadsheets

---
layout: center
class: text-center
zoom: 1.4
---

# Do Now

Answer on the whiteboard table

What does it mean if two variables are correlated?

What is the difference between positive and negative correlation?

---
layout: li
---

::li::
- To be able to describe the concept of correlation between two variables
- To be able to calculate the correlation coefficient between two variables using spreadsheets
- To be able to interpret the correlation coefficient between two variables

::sc::
- Describe the concept of correlation between two variables
- Use Excel to calculate the correlation coefficient
- Interpret the correlation coefficient meaningfully

---
layout: center
---

# Correlation

Correlation is a statistical measure that describes the extent to which two variables are related.
- A positive correlation means that as one variable increases, the other variable also increases.
- A negative correlation means that as one variable increases, the other variable decreases.
- Correlation describes a general pattern of the data

## Examples of Correlation

<v-clicks>

- Height and weight
- Seatbelt usage rates and traffic fatalities
- Hours studied and exam score
- Temperature and ice cream sales

</v-clicks>
---
layout: center
---
# Correlation

<img src="/img/milk-divorce.svg" alt="Correlation between milk consumption and divorce rates in Colorado" width="450px"/>

What do we think is happening?

```mermaid
flowchart LR
    A[Milk Consumption] -->|Increases| B[Divorce Rates]
    B -->|Increases| A
```
---
layout: cover
---

# Correlation does not imply causation!

Just because two variables are correlated does not mean that one variable causes the other to change.

---
layout: center
---

# Pearson's Correlation Coefficient - `r`

Pearson's correlation coefficient (usually labelled as `r`) is a measure of the strength and direction of the linear relationship between two **numeric variables**.

- r = 1 means a perfect positive correlation
- r = -1 means a perfect negative correlation
- r = 0 means no correlation
- r is a number between -1 and 1

---
layout: center
zoom: 1.3
---

# Correlation Coefficient in Excel
<br/>

`=CORREL(array1, array2)`

- `array1` is the first set of data
- `array2` is the second set of data
- Both arrays must be the same size

eg. 

`=CORREL(A2:A20, B2:B20)`

---
layout: center
---

# Discuss

Estimate the correlation coefficient between the two variables in the tables below.

1. Hours studied and exam score

| Hours Studied | Exam Score |
|---------------|------------|
| 1             | 50         |
| 2             | 60         |
| 3             | 70         |
| 4             | 80         |
| 5             | 90         |

2. Cars sold and advertising spend

| Cars Sold | Advertising Spend |
|-----------|------------------|
| 3         | 1000             |
| 4         | 2500             |
| 6         | 5000             |
| 7         | 7000             |
| 10        | 6000             |

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

---
layout: center
---
