---
transition: fade-out
layout: li
routeAlias: sql-basics
---
::li::
- To be clear on the expectations in Data Analytics, including materials, entry and exit routines
- To understand the importance of SQL in databases

::sc::
- describe the expectations in Data Analytics
- run SQL queries in a Jupyter notebook

---
transition: fade-out
layout: center
hideInToc: false
---

# Databases and SQL

## SQL

SQL is a standard language for storing, manipulating and retrieving data in databases.

Our StepUp work is to learn some of the basics of **SQL**, which will allow you to retrieve data from a **database** using **queries**.

---
layout: center
---

# Databases and SQL

A **database** is a collection of data that is organized so that it can be easily accessed, managed, and updated.

We use **relational databases** in Data Analytics. Relational databases:

- store data in tables
- keep data organised in rows and columns
- require that data has an assigned data type
- have relationships between tables
- use SQL to **query** the data

> Vocab: **query** - a request for data or information from a database, sourced from one or more tables.

---
layout: center
---

# SQL Basics - Query

The most basic SQL query is to select everything from a table. Any time we retrieve data from a database, we use the `SELECT` statement.

```sql

SELECT * FROM table_name;

```

For example if we have a table called `rooms`, we can retrieve all the data from it with the following query:

```sql
SELECT * FROM rooms;

```

## Result: 

| room_id | room_name | capacity |
| -------- | --------- | -------- |
| 1        | Ballroom    | 30       |
| 2        | Conference Room A | 15      |
| ...      | ...       | ...      |

---
layout: center
transition: fade
zoom: 0.95
---

# SQL Basics - individual columns

If we don't want to retrieve all the data, we can just retrieve specific columns. We do this by specifying the column names in the `SELECT` statement.

```sql 

SELECT column1, column2, ...
FROM table_name

```

For example, if we only wanted to retrieve the `room_name` and `capacity` columns from the `rooms` table, we would use the following query:

```sql
SELECT room_name, capacity
FROM rooms;

```

Result:

| room_name | capacity |
| --------- | -------- |
| Ballroom    | 30       |
| Conference Room A | 15      |

---
layout: two-cols-header
transition: fade
---

# SQL Basics - using a condition

::left::

We can also change which rows are returned, based on specific conditions. We do this by using the `WHERE` clause in our query.

```sql

SELECT column1, column2
FROM table_name
WHERE condition;

```

::right::

For example, if we only wanted to name and capacity of any rooms that have a capacity greater than 20, we would use the following query:

```sql
SELECT room_name, capacity
FROM rooms
where capacity > 20;

```

**Result:**

| room_name | capacity |
| --------- | -------- |
| Ballroom    | 30       |

---
layout: center
---

# Conditions - Other conditions

We can use **comparison operators** to create conditions in our queries.

- **=** equal to
- **!=** or **<>** not equal to
- **>** greater than
- **<** less than
- **>=** greater than or equal to
- **<=** less than or equal to

When looking for a specific text value, we use **single quotes** around the value. 

```sql
select * from rooms where room_name = 'Ballroom';
```

> SQL commands are not case sensitive, but the text values are. So if we had asked for 'BALLROOM', the query would not have returned any results.

---

layout: center
---

# Check for understanding - queries

Below is a table called `books` that contain information about books that Roger has in his personal library.

| book_id | title | author | year_published | genre |
| ------- | ----- | ------ | -------------- | ----- |
| 1       | The Great Gatsby | F. Scott Fitzgerald | 1925 | Fiction |
| 2       | To Kill a Mockingbird | Harper Lee | 1960 | Fiction |
| 3       | 1984 | George Orwell | 1949 | Dystopian |
| 4       | Dungeon Crawler Carl | Matt Dinniman | 2018 | Science Fiction |

On your mini-whiteboard, write an SQL query to:

1. Retrieve all the details of books published before 1950
2. Retrieve just the title and author of books in the Fiction genre

---
layout: center
---

# Linking conditions - using AND and OR

We can also link conditions together using the `AND` and `OR` keywords.

- **AND** - both conditions must be true for the row to be returned
- **OR** - either condition can be true for the row to be returned

So this query:

```sql
SELECT * FROM rooms
WHERE capacity < 20 OR room_name = 'Ballroom';

```

Would bring back both the Ballroom and Conference Room A, because the Ballroom meets the second condition, and Conference Room A meets the first condition. But this query:

```sql

SELECT * FROM rooms
WHERE capacity < 20 AND room_name = 'Ballroom';

```

would not return any results, because the Ballroom does not meet the first condition, and no other rooms are called 'Ballroom'.

---
layout: two-cols-header
zoom: 0.91
---

# SQL Basics - Sorting results

When working with many rows of data, it can be useful to sort the results of a query. We can do this using the `ORDER BY` clause.

> `ASC` - ascending order (smallest to largest, A-Z) `DESC` - descending order (largest to smallest, Z-A)

::left::

### Sorting results

```sql
SELECT column1, column2
FROM table_name
ORDER BY column1 ASC|DESC;
```

So this query:

```sql
SELECT room_name, capacity
FROM rooms
ORDER BY capacity DESC;

```

Returns all the rooms, sorted by capacity from largest to smallest.


::right::

### Limiting results

We can also limit the number of rows returned by a query using the `LIMIT` clause.

```sql
SELECT column1, column2
FROM table_name
ORDER BY column1 ASC|DESC
LIMIT number_of_rows;
```

To just return the first 2 rows of the previous query, we would use:

```sql
SELECT room_name, capacity
FROM rooms
ORDER BY capacity DESC
LIMIT 2;

```

---
layout: center
zoom: 1.4
---

# Now Try

Open the "Port Wren Records" page and complete Missions 1 - 6. If you get stuck:

- Check the slides for examples
- Use the "Hints" button on the site

> Note: You can use the "Start from a previous query" dropdown, so you don't have to retype the whole query each time.


---
layout: two-cols-header
transition: fade
---

# SQL Basics

Once we get going with databases, you will want to be able to create tables, add rows into them, and retrieve data from them. Let's look at some of the basic SQL commands that will allow us to do this.

::left::

# Create a table

```sql
CREATE TABLE table_name (
    column1 datatype,
    column2 datatype,
   ....
);
```

::right::

## Add rows into a table

```sql
INSERT INTO table_name (column1, column2, ...)
VALUES (value1, value2, ...);
```

---
layout: center
transition: fade
hideInToc: true
zoom: 1.5
---

# SQL Basics

## Joins
```sql {1|2|3}

SELECT a.column1, b.column2, ...
FROM table1 a, table2 b
WHERE a.common_field = b.common_field;

```

## Inner Join

```sql {1|2|3}
SELECT a.column1, b.column2, ...
FROM table1 a
INNER JOIN table2 b
ON a.common_field = b.common_field;
```