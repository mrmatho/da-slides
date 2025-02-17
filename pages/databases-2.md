---
layout: cover
transition: fade
---

# Joining Tables in SQL

---
layout: two-cols-header
transition: fade-out
zoom: 0.85
hideInToc: true
---
# Do Now

::left::
Which rows from the table below would be returned by the following SQL query?

```sql
SELECT *
FROM games
WHERE genre = 'RPG'
AND platform = 'PC';
```
::right::
| title | genre | platform |
|-------|-------|----------|
| Starcraft | RTS | PC |
| Diablo | RPG | PC |
| Civilization | Strategy | PC |
| Age of Empires | RTS | PC |
| Final Fantasy | RPG | Console |
| World of Warcraft | MMORPG | PC |
| Skyrim | RPG | PC |

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
transition: fade-out
layout: li
---
::li::
- To be able to perform joins across multiple tables in SQL
- To be able to describe the different types of joins and their purpose

::sc::
- I have been able to complete the SQL tutorials (or am ready to do so at home)
- I can describe the difference between an inner join and an outer join

---
layout: default
hideInToc: true
---

# Joining Tables in SQL

The "relational" element of relational databases refers to the ability to join tables together. This is a powerful feature that allows us to combine data from multiple tables in a single query. Data within a database is related in one of three ways:

<v-clicks depth="1">

- **One-to-One:** this data is usually stored in the same table. Eg. a user's name and email address. Each user has one name and one email address.
- **One-to-Many:** this data is stored in two tables. Eg. a user and their orders. Each user can have many orders, but each order belongs to only one user.
- **Many-to-Many:** this data is stored in three tables. Eg. a user, a product, and the user's orders. Each user can have many orders, and each order can contain many products. There is no limit as to how many users can order a product, or how many products can be ordered by a user.


<span v-mark>One to many relationships</span> are the most common example of joins, and we will focus on these in this lesson.
</v-clicks>
---
layout: default
hideInToc: true
---
# Inner Joins

An inner join returns only the rows that have **matching values in both tables**. This is the most common type of join. The syntax for an inner join is:

```sql
SELECT columns
FROM table1
INNER JOIN table2
ON table1.column = table2.column;
```

Usually the column being joined is a primary key in one table and a foreign key in the other (but it doesn't have to be). This is how the database knows which rows to match up.

---
layout: two-cols
hideInToc: true
zoom: 0.9
---
# Inner Joins - Example

Consider the following two tables:

Users Table
| user_id | name | email |
|---------|------|-------|
| 1 | Alice | alice@example.com |
| 2 | Bob | bob@madeup.net |
| 3 | Charlie | chuck23@gmail.com |

Orders Table
| order_id | user_id | product | quantity |
|----------|---------|---------|----------|
| 1 | 2 | Widget | 2 |
| 2 | 2 | Gadget | 1 |
| 3 | 1 | Gizmo | 3 |

<style>
th {
  background-color:rgb(164, 160, 160);
  font-weight: bold;
  border: 1px solid black;
  padding: 5px;
  font-size: 85%;
}

td {
  border-collapse: collapse;
  border: 1px solid black;
  padding: 5px;
  font-size: 80%;
}

table {
  margin-left: -10px;
}
</style>
::right::

<v-clicks depth="3">

- What is the relationship between these two tables? 
    - One to many - each user can have many orders, but each order belongs to only one user.
- Which product(s) has Alice ordered?
    - *Gizmo*
- Which user(s) has ordered a Widget?
    - *Bob*
</v-clicks>

---
layout: two-cols
hideInToc: true
---
# Inner Joins - Example Continued

Consider the following two tables:

Users Table

| user_id | name | email |
|---------|------|-------|
| 1 | Alice | alice@example.com |
| 2 | Bob | bob@madeup.net |
| 3 | Charlie | chuck23@gmail.com |

Orders Table

| order_id | user_id | product | quantity |
|----------|---------|---------|----------|
| 1 | 2 | Widget | 2 |
| 2 | 2 | Gadget | 1 |
| 3 | 1 | Gizmo | 3 |
<style>
th {
  background-color:rgb(164, 160, 160);
  font-weight: bold;
  border: 1px solid black;
  padding: 5px;
  font-size: 85%;
}

td {
  border-collapse: collapse;
  border: 1px solid black;
  padding: 5px;
  font-size: 80%;
}

table {
  margin-left: -10px;
}
</style>
::right::
Write an SQL query to return the following columns:

- name
- email
- product

for people who ordered any product

<v-click>
```sql
SELECT name, email, product
FROM users
INNER JOIN orders
ON users.user_id = orders.user_id;
```
</v-click>

---
layout: default
hideInToc: true
---
# Outer Joins

An outer join returns **all rows from one table**, and the matched rows from the other table. If there is no match, the result is NULL. There are three types of outer joins:

- **LEFT JOIN:** returns all rows from the left table, and the matched rows from the right table.
- **RIGHT JOIN:** returns all rows from the right table, and the matched rows from the left table.
- **FULL JOIN:** returns all rows when there is a match in either table.

---
layout: default
hideInToc: true
---
# Practice
1. Create a new database called `store.db` in the SQLite DB Browser and create the following tables:
    - `customers` with columns `customer_id`, `name`, and `email`
    - `orders` with columns `order_id`, `customer_id`, `product_id`, and `quantity`
    - `products` with columns `product_id`, `name`, and `price`

2. Insert some data into these tables:
    - Insert at least 3 customers
    - Insert at least 5 products
    - Insert at least 10 orders

3. Write SQL queries to:
    - Return the names of all customers who have placed an order
    - Calculate the total amount charged for each order


