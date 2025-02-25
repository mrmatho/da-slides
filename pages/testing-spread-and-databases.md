---
layout: cover
transition: fade
hideInToc: false
background: https://cover.sli.dev/
---

# Testing Spreadsheets and Databases

---
layout: li
---

::li::
- To be able to describe the concept of testing in working with spreadsheets and databases
- To be able to create test cases for testing formulas and queries
- To be able to document test results in a test table

::sc::
- Successfully document a full set of test cases for both a spreadsheet and a database task
---
layout: cover
---

# What do we need to test in spreadsheets and databases?

---
layout: center
zoom: 1.2
---

# From the study design

- techniques for testing databases and spreadsheets, including: 
    - testing formula and query results
    - testing validation
    - test cases comparing expected and actual results in testing tables

---
layout: center
---

# Testing formula and query results

- How do we do it?
    - Create a test case. A test case is a set of conditions (usually a set of data) that we already know the expected result for.
    - Eg. if we have a formula that adds two numbers together, we can create a test case with the numbers 2 and 3, and the expected result of 5. Or if I have a query that returns all the adults in a database, I can create a test case with a set of data that I know contains 3 adults and 2 children, and then check that the query return the correct rows for just the adults.
- What do we need to test?
    - We need to test that each formula or query returns the expected result for a set of data.
    - We also need to test that the formula or query handles invalid data correctly. This is done by creating test cases with invalid data and checking that the formula or query returns an error message or an empty result.

---
layout: center
---

# Validation in spreadsheets and databases

- What is validation?
    - Validation is a way of checking that the data entered into a spreadsheet or database is correct and meets certain criteria.
    - For example, we might want to check that a date is in the correct format, or that a number is within a certain range.
- How do we test validation?
    - We create test cases with valid and invalid data and check that the validation rules are applied correctly.
    - For example, if we have a validation rule that checks that a number is between 1 and 10, we can create test cases with the numbers 0, 5, and 11, and check that the validation rule returns an error message for the first and last test cases, but not for the second.

---
layout: center
---

# Test Table

- A test table is a table that documents the test cases we have created, the expected results, and the actual results.
- A test table should include the following columns:
    - Test case: a description of the test case
    - Input data: the data used in the test case
    - Expected result: the expected result of the test case
    - Actual result: the actual result of the test case

---
layout: center
---
# Example Test Table

| Test Case | Input Data | Expected Result | Actual Result |
|-----------|------------|-----------------|---------------|
| Checking Adults | 3 adults, 2 children | 3 rows | 3 rows |
| Checking Adults No results | 0 adults, 5 children | 0 rows | 0 rows |
| Checking Validation | 0, 5, 11 | Error for 0 and 11, no error for 5 | <span v-mark.circle.blue>Error for 0, 5 and 11. Need to fix so 5 has no error.</span> |

<v-clicks>

Remember: we **want** to document errors in our test table, so we can fix them! A test table where `Expected Results` always matches `Actual Results` makes Mr Matheson suspicious!

</v-clicks>

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