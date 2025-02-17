---
layout: cover
transition: fade
---

# Spreadsheets

---
layout: two-cols-header
hideInToc: true
---
# Do Now

Answer in your book

A local basketball team has created a database to track players and their statistics. They store information about each player in a database that uses the tables shown below. Create an SQL query to find the names of players who play for "Kilsyth Kougars" and are taller than 185cm.

::left::

### Players

| Column | Data Type | Note |
|-----------|-----|-------------|
| player_id | int | PRIMARY KEY |
| player_name | text|             |
| height    | int | (in cm)     |
| team_id   | int | FOREIGN KEY |

::right::

### Teams

| Column | Data Type | Note |
|---------|-----|-------------|
| team_id | int | PRIMARY KEY |
| team_name    | text|        |
| home_court   | text|        |

<style>
th {
  background-color:rgb(164, 160, 160);
  font-weight: bold;
  border: 1px solid black;
}

td {
  border-collapse: collapse;
  border: 1px solid black;
}

</style>
---
layout: center
hideInToc: true
---

# Spreadsheets

## From the Study Design

- techniques for effectively and efficiently manipulating and cleansing data, including:
    - formulas and functions to perform calculations

---
layout: center
hideInToc: true
---

# Which do you already know ?
We are working from the assumption that you don't know many of these. But if you do - it will speed things up for you.

1. Creating a new spreadsheet
2. Entering data
3. Formatting cells (e.g. currency, date, percentage)
4. Simple Calculations (e.g. addition, subtraction, multiplication, division)
5. Using basic functions (e.g. SUM, AVERAGE, MAX, MIN)
6. Using relative and absolute cell references
7. Using sorting and filtering
8. Creating charts
9. Using Lookup functions (e.g. VLOOKUP, XLOOKUP)
10. Using pivot tables

---
layout: two-cols
hideInToc: true
zoom: 0.8
---

## Spreadsheet Activity: Forbes Richest Athletes Analysis

- **0 – 10 min: Open CSV File**
  - Students open the provided CSV file in their spreadsheet software.
  - Explore and review the data.
- **10 – 20 min: Formatting**
  - Format the **"earnings ($ million)"** column as **Currency** or **Number with 2 decimal places**.
  - Format the **"Year"** column as **Number**.
- **20 - 30 min: Simple Calculations & Basic Functions**
  - Add a new column called **"Earnings in Thousands"** to convert earnings from millions to thousands.  
    *(e.g., `=Earnings * 1000`)*
  - Use basic functions:
    - **SUM** – Calculate total earnings in a selected year.
    - **AVERAGE** – Find the average earnings in a selected year.
    - **MAX / MIN** – Find the highest and lowest earners.

::right::
- **30 – 45 min: Relative & Absolute References**
  - Add an exchange rate cell (e.g., **B1** with value **1.5** for USD to AUD).
  - Create a new column **"Earnings in AUD"** using an absolute reference: *(e.g., `=Earnings * $B$1`)*
- **45 – 60 min: Sorting, Filtering & Charts**
  - **Sort** the data by **earnings** in descending order.
  - **Filter** the data for a specific **sport** (e.g., Basketball, Soccer).
  - Create a **Bar Chart** showing **Top 10 highest-earning athletes**.
- **60 – 75 min: Lookup Functions**
  - Add a second sheet with an **Exchange Rate Table** (e.g., USD, AUD, EUR).
  - Use **VLOOKUP/XLOOKUP** to retrieve the exchange rate based on **Nationality**.
  - Calculate **Earnings in Local Currency** using the retrieved exchange rate.
- **75 – 95 min: Pivot Tables**
  - Create a **Pivot Table** to:
    - Show **total earnings by sport** across all years.
    - Show **average earnings by nationality**.
    - Analyze **top-earning athletes over time (by year)**.

