---
layout: cover
transition: fade
hideInToc: false
background: /img/validation.webp
---

# Validating Database and Spreadsheets

---
layout: li
---
::li::
- To be able to describe the concept of validation in working with spreadsheets and databases
- To be able to apply:
    - existence checks
    - type checks
    - range checks

::sc::
- Create a validation strategy for:
    - a spreadsheet
    - a database
---
layout: center
transition: fade
---

# Validation

Validation is the process of ensuring that data is reasonable and usable.

- If is not checking that data is correct: only that it is reasonable.
- We check that data:
    - exists (existence check)
    - is of the correct type (type check)
    - is within an appropriate range (range check)

---
layout: center
transition: fade
---

# Existence Check

An existence check is a validation check that ensures that data has been entered into a field or column. 

- A database might do this by adding a<span v-mark.highlight.orange> `NOT NULL` constraint</span> to a column.
```sql {all|3}
    CREATE TABLE students (
        id INT PRIMARY KEY,
        name VARCHAR(50) NOT NULL
    );
```

- A spreadsheet might do this by using <span v-mark.highlight.orange>conditional formatting</span> to highlight empty cells.

---
layout: center
transition: fade
---

# Type Check

A type check is a validation check that ensures that data is of the correct type.
- A database might do this by adding an <span v-mark.highlight.orange> `INTEGER` constraint</span>to a column. 
  ```sql {all|4}
    CREATE TABLE students (
        id INT PRIMARY KEY,
        name VARCHAR(50) NOT NULL,
        age INT
    );
    ```
- A spreadsheet might do this by using <span v-mark.highlight.orange>data validation</span> to restrict the type of data that can be entered into a cell, or by using <span v-mark.highlight.orange>conditional formatting</span> to highlight cells that are of the wrong type.

---

# Range Check

A range check is a validation check that ensures that data is within an appropriate range.
- A database might do this by adding a <span v-mark.highlight.orange> `CHECK` constraint</span> to a column.
```sql {all|1,3}
    CREATE TABLE students (
        id INT PRIMARY KEY,
        name VARCHAR(50) NOT NULL,
        age INT CHECK (age >= 0 AND age <= 120)
    );
```
or 
```sql
    ADD CONSTRAINT age_check CHECK (age >= 0 AND age <= 120);
```

- A spreadsheet might do this by using <span v-mark.highlight.orange>data validation</span> to restrict the range of values that can be entered into a cell, or by using <span v-mark.highlight.orange>conditional formatting</span> to highlight cells that are outside of the range.



---
layout: iframe-right
url: https://support.microsoft.com/en-au/office/apply-data-validation-to-cells-29fecbcc-d1b9-42c1-9d76-eff3ce5f7249
transition: fade
---
 
 # Data Validation in Excel

 Data Validation in Excel allows you to restrict the type of data that can be entered into a cell.
- You can use it to create drop-down lists, restrict data to a certain type, and set limits on the values that can be entered.
- You can also use it to create custom validation rules using formulas.

---
layout: iframe-right
url: https://support.microsoft.com/en-au/office/use-conditional-formatting-to-highlight-information-in-excel-fed60dfa-1d3f-4e13-9ecb-f1951ff89d7f
transition: fade
---

# Conditional Formatting in Excel

Conditional Formatting in Excel allows you to change the appearance of a cell based on its value.

- Existence check: highlight empty cells
- Type check: highlight cells that are of the wrong type.
    - `Use a formula to determine which cells to format`
    - `=ISTEXT(A1)` for text (where A1 is the first cell in the range)
    - `=ISNUMBER(A1)` for numbers
- Range check: highlight cells that are outside of the range.

<style>
    ul li {
        margin-bottom: 0em;
        line-height: 1.5em;
    }
</style>
---
layout: center
---

# Validation vs Data Cleansing

- Both validation and data cleansing are important steps in ensuring data is usable and reliable.
- Validation occurs at the point of <span v-mark.underline.purple>data entry</span>, while data cleansing occurs <span v-mark.underline.blue>after data has been loaded</span>.
- Validation is a <span v-mark.underline.purple>preventative</span> measure, while data cleansing is a <span v-mark.underline.blue>corrective</span> measure.

---
