---
transition: fade-out
layout: li
---
::li::
- To be clear on the expectations in Data Analytics, including materials, entry and exit routines
- To understand the importance of SQL in databases

::sc::
- describe the expectations in Data Analytics
- run SQL queries in a Jupyter notebook

---
transition: fade-out
layout: image-right
image: https://cover.sli.dev
---

# Databases and SQL

## SQL

SQL is a standard language for storing, manipulating and retrieving data in databases.

We investigated SQL at a theoretical level during StepUp, and now we will learn how to use SQL in practice.

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/features/slide-scope-style
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

h2 {
  color: #2B90B6;
  font-weight: bold;
}

  p{
    font-size: 150%;
    line-height: 1.2em;
  }
</style>

---
layout: quote
class: steps
---

## GitHub CodeSpaces

We are using GitHub CodeSpaces to run our SQL exercises, using a database system called **DuckDB** in a **Jupyter notebook**. 

To access the SQL exercises, you will need to:

<img src="/img/github-mark.png" alt="GitHub" style="width: 250px; float:right;"/>

1. Sign up for a GitHub account (if you don't have one already)
2. Accept the invitation to the GitHub Classroom assignment (link is on Compass)
3. Open the assignment in GitHub Classroom
4. Click on the link to open the assignment in GitHub CodeSpaces



Hopefully most of the steps are relatively well explained in the notebook, but make sure you ***ask questions*** if you are not sure.

---
layout: iframe-right
url: https://heathmontdataanalytics.github.io/topics/databases.html
zoom: 0.6
---

## You can always use the Website

---
layout: full
transition: fade
hideInToc: true
---

# SQL Basics

```sql {1|2|3}

SELECT column1, column2, ...
FROM table_name
WHERE condition;

```

