# SQL Mastery Checklist

> A complete, phase-by-phase learning roadmap covering SQL from absolute beginner to senior/principal level — concepts, internals, optimization, and real-world usage across platforms.

---

## Table of Contents

1. [Phase 0: Prerequisites & Foundations](#phase-0-prerequisites--foundations)
2. [Phase 1: Why SQL Exists](#phase-1-why-sql-exists)
3. [Phase 2: Databases & Tables](#phase-2-databases--tables)
4. [Phase 3: Basic Querying (SELECT)](#phase-3-basic-querying-select)
5. [Phase 4: Filtering Data (WHERE)](#phase-4-filtering-data-where)
6. [Phase 5: Sorting & Limiting](#phase-5-sorting--limiting)
7. [Phase 6: Aggregate Functions](#phase-6-aggregate-functions)
8. [Phase 7: GROUP BY & HAVING](#phase-7-group-by--having)
9. [Phase 8: Joins](#phase-8-joins)
10. [Phase 9: Subqueries](#phase-9-subqueries)
11. [Phase 10: Set Operations](#phase-10-set-operations)
12. [Phase 11: Data Manipulation (DML)](#phase-11-data-manipulation-dml)
13. [Phase 12: Data Definition (DDL)](#phase-12-data-definition-ddl)
14. [Phase 13: Constraints & Data Integrity](#phase-13-constraints--data-integrity)
15. [Phase 14: String Functions](#phase-14-string-functions)
16. [Phase 15: Numeric Functions](#phase-15-numeric-functions)
17. [Phase 16: Date & Time Functions](#phase-16-date--time-functions)
18. [Phase 17: NULL Handling](#phase-17-null-handling)
19. [Phase 18: CASE Expressions](#phase-18-case-expressions)
20. [Phase 19: Window Functions](#phase-19-window-functions)
21. [Phase 20: CTEs & Recursive Queries](#phase-20-ctes--recursive-queries)
22. [Phase 21: Views](#phase-21-views)
23. [Phase 22: Indexes](#phase-22-indexes)
24. [Phase 23: Transactions & ACID](#phase-23-transactions--acid)
25. [Phase 24: Query Execution & Internals](#phase-24-query-execution--internals)
26. [Phase 25: Query Optimization](#phase-25-query-optimization)
27. [Phase 26: Normalization & Schema Design](#phase-26-normalization--schema-design)
28. [Phase 27: Stored Procedures & Functions](#phase-27-stored-procedures--functions)
29. [Phase 28: Triggers](#phase-28-triggers)
30. [Phase 29: Platform Differences](#phase-29-platform-differences)
31. [Phase 30: SQL for Data Analysis](#phase-30-sql-for-data-analysis)
32. [Phase 31: SQL for Data Engineering](#phase-31-sql-for-data-engineering)
33. [Phase 32: SQL at Scale](#phase-32-sql-at-scale)
34. [Phase 33: Security & Access Control](#phase-33-security--access-control)
35. [Phase 34: Real Projects](#phase-34-real-projects)
36. [Final Mastery](#final-mastery)

---

## Phase 0: Prerequisites & Foundations

### What You Should Know First

- [ ] Basic computer literacy
- [ ] What a file is vs what a database is
- [ ] Spreadsheet concepts (rows, columns, tables)
- [ ] Basic logic (AND, OR, NOT)

### Core Mental Models

- [ ] A database is an organized collection of data
- [ ] A table is like a spreadsheet tab
- [ ] A row is one record / observation
- [ ] A column is one attribute / field
- [ ] SQL is the language you use to talk to the database

---

## Phase 1: Why SQL Exists

### The Problem

- [ ] Data stored in flat files (CSV, Excel) doesn't scale
- [ ] No way to query across multiple files efficiently
- [ ] No concurrency — multiple users can't write safely at once
- [ ] No data integrity guarantees
- [ ] No standard way to ask questions of data

### First Principles

- [ ] What is a Relational Database?
- [ ] What is a DBMS (Database Management System)?
- [ ] What is RDBMS (Relational DBMS)?
- [ ] What is SQL (Structured Query Language)?

### Understand

- [ ] SQL is declarative — you say WHAT you want, not HOW to get it
- [ ] The database engine figures out HOW (query planner)
- [ ] SQL is a standard (ANSI SQL) but every platform adds extensions
- [ ] SQL has been around since the 1970s and isn't going anywhere

### Popular Platforms

| Platform | Best For |
|---|---|
| PostgreSQL | Open source, feature-rich, default choice |
| MySQL / MariaDB | Web apps, LAMP stack |
| SQLite | Embedded, local, lightweight |
| SQL Server (MSSQL) | Microsoft ecosystem, enterprise |
| Oracle | Enterprise, banking, legacy |
| BigQuery | Google Cloud, analytics at scale |
| Snowflake | Cloud data warehouse |
| Redshift | AWS data warehouse |
| DuckDB | Local analytical queries, fast |
| Databricks SQL | Spark-based, big data |

---

## Phase 2: Databases & Tables

### Core Concepts

- [ ] Database (schema in some platforms)
- [ ] Table
- [ ] Row (record, tuple)
- [ ] Column (field, attribute)
- [ ] Primary Key
- [ ] Foreign Key
- [ ] Data Types overview

### Data Types

**Numeric**
- [ ] INT / INTEGER
- [ ] BIGINT
- [ ] DECIMAL / NUMERIC (exact)
- [ ] FLOAT / REAL (approximate)

**Text**
- [ ] CHAR(n) — fixed length
- [ ] VARCHAR(n) — variable length
- [ ] TEXT — unlimited length

**Date/Time**
- [ ] DATE
- [ ] TIME
- [ ] DATETIME / TIMESTAMP
- [ ] INTERVAL (PostgreSQL)

**Boolean**
- [ ] BOOLEAN / BOOL

**Other**
- [ ] JSON / JSONB (PostgreSQL)
- [ ] ARRAY (PostgreSQL)
- [ ] UUID
- [ ] BLOB / BYTEA (binary data)

### Understand

- [ ] Choosing the right data type matters for storage and performance
- [ ] DECIMAL vs FLOAT — when exact precision matters (money → DECIMAL)
- [ ] VARCHAR vs TEXT — platform differences
- [ ] TIMESTAMP vs TIMESTAMPTZ (timezone-aware)

---

## Phase 3: Basic Querying (SELECT)

### Core Syntax

```sql
SELECT column1, column2
FROM table_name;
```

### Learn

- [ ] `SELECT *` — all columns (avoid in production)
- [ ] `SELECT col1, col2` — specific columns
- [ ] Column aliases: `SELECT salary * 12 AS annual_salary`
- [ ] Expression in SELECT: math, string concat
- [ ] `DISTINCT` — remove duplicates
- [ ] `SELECT DISTINCT col1, col2`

### Understand

- [ ] SELECT * is bad in production — explicit columns are better
- [ ] Aliases make output readable
- [ ] DISTINCT applies to the combination of all selected columns

**Exercises**
- [ ] Select all employees
- [ ] Select only name and salary columns
- [ ] Select distinct job titles

---

## Phase 4: Filtering Data (WHERE)

### Core Syntax

```sql
SELECT *
FROM employees
WHERE department = 'Sales';
```

### Comparison Operators

- [ ] `=` equal
- [ ] `!=` or `<>` not equal
- [ ] `>` / `<` / `>=` / `<=`
- [ ] `BETWEEN x AND y` (inclusive)
- [ ] `IN (val1, val2, val3)`
- [ ] `NOT IN (...)`
- [ ] `LIKE 'pattern%'`
- [ ] `ILIKE` (case-insensitive LIKE, PostgreSQL)
- [ ] `IS NULL` / `IS NOT NULL`

### LIKE Patterns

- [ ] `%` — any number of characters
- [ ] `_` — exactly one character
- [ ] `'S%'` — starts with S
- [ ] `'%son'` — ends with son
- [ ] `'%an%'` — contains an

### Logical Operators

- [ ] `AND`
- [ ] `OR`
- [ ] `NOT`
- [ ] Operator precedence: NOT > AND > OR
- [ ] Use parentheses to control precedence

### Understand

- [ ] WHERE filters rows before aggregation
- [ ] NULL comparisons require IS NULL, not = NULL
- [ ] BETWEEN is inclusive on both ends
- [ ] IN is cleaner than multiple OR conditions

**Exercises**
- [ ] Find employees in Sales or Marketing
- [ ] Find salaries between 50000 and 100000
- [ ] Find customers whose name starts with 'A'
- [ ] Find records where email is NULL

---

## Phase 5: Sorting & Limiting

### ORDER BY

```sql
SELECT name, salary
FROM employees
ORDER BY salary DESC;
```

- [ ] `ORDER BY col ASC` — ascending (default)
- [ ] `ORDER BY col DESC` — descending
- [ ] Multiple columns: `ORDER BY dept ASC, salary DESC`
- [ ] Order by column position: `ORDER BY 2 DESC` (avoid in production)
- [ ] Order by expression or alias

### LIMIT / TOP / FETCH

- [ ] `LIMIT n` — PostgreSQL, MySQL, SQLite
- [ ] `TOP n` — SQL Server
- [ ] `FETCH FIRST n ROWS ONLY` — ANSI standard, Oracle
- [ ] `ROWNUM` — Oracle legacy

### OFFSET

- [ ] `LIMIT 10 OFFSET 20` — pagination
- [ ] Understand: OFFSET becomes slow on large tables (deep pagination problem)

### Understand

- [ ] Without ORDER BY, row order is not guaranteed
- [ ] LIMIT without ORDER BY gives arbitrary results
- [ ] For pagination at scale, use keyset pagination instead of OFFSET

**Exercises**
- [ ] Top 5 highest paid employees
- [ ] Page 3 of results (rows 21-30)

---

## Phase 6: Aggregate Functions

### Core Functions

- [ ] `COUNT(*)` — count all rows
- [ ] `COUNT(col)` — count non-NULL values
- [ ] `COUNT(DISTINCT col)` — count unique values
- [ ] `SUM(col)`
- [ ] `AVG(col)`
- [ ] `MIN(col)`
- [ ] `MAX(col)`

### Statistical Aggregates (platform-specific)

- [ ] `STDDEV()` / `STDDEV_POP()` / `STDDEV_SAMP()`
- [ ] `VARIANCE()` / `VAR_POP()` / `VAR_SAMP()`
- [ ] `MEDIAN()` (some platforms)
- [ ] `PERCENTILE_CONT()` / `PERCENTILE_DISC()`
- [ ] `MODE()` (PostgreSQL)

### Understand

- [ ] COUNT(*) vs COUNT(col) — NULL behavior difference
- [ ] AVG ignores NULLs — may not be what you want
- [ ] Aggregates collapse many rows into one value
- [ ] You can't use WHERE on aggregated results (use HAVING)

**Exercises**
- [ ] Total sales revenue
- [ ] Average order value
- [ ] Count of distinct customers

---

## Phase 7: GROUP BY & HAVING

### GROUP BY

```sql
SELECT department, COUNT(*), AVG(salary)
FROM employees
GROUP BY department;
```

- [ ] Groups rows by one or more columns
- [ ] Every column in SELECT must be in GROUP BY or an aggregate
- [ ] Can group by multiple columns
- [ ] Can group by expressions: `GROUP BY YEAR(order_date)`

### HAVING

```sql
SELECT department, AVG(salary) AS avg_sal
FROM employees
GROUP BY department
HAVING AVG(salary) > 60000;
```

- [ ] Filters AFTER aggregation (WHERE filters before)
- [ ] Use HAVING for conditions on aggregate results
- [ ] Can reference column aliases in some platforms

### WHERE vs HAVING

| | WHERE | HAVING |
|---|---|---|
| When | Before GROUP BY | After GROUP BY |
| On | Raw rows | Aggregated results |
| Use | Row conditions | Aggregate conditions |

### Execution Order (Critical)

```
FROM → WHERE → GROUP BY → HAVING → SELECT → ORDER BY → LIMIT
```

- [ ] Memorize this order — it explains many SQL confusions
- [ ] Why you can't use SELECT alias in WHERE (alias defined later)
- [ ] Why you CAN use alias in ORDER BY (comes after SELECT)

**Exercises**
- [ ] Sales by category, only categories > $10,000
- [ ] Departments with more than 5 employees
- [ ] Average order value by customer, top 10

---

## Phase 8: Joins

### Why Joins Exist

- [ ] Data is split across tables to avoid redundancy (normalization)
- [ ] Joins reconnect related data at query time

### Join Types

**INNER JOIN**
```sql
SELECT e.name, d.department_name
FROM employees e
INNER JOIN departments d ON e.dept_id = d.id;
```
- [ ] Returns only matching rows from both tables
- [ ] Most common join type

**LEFT JOIN (LEFT OUTER JOIN)**
- [ ] All rows from left table + matching rows from right
- [ ] Non-matching right rows → NULL

**RIGHT JOIN (RIGHT OUTER JOIN)**
- [ ] All rows from right table + matching rows from left
- [ ] Rarely used — can always rewrite as LEFT JOIN

**FULL OUTER JOIN**
- [ ] All rows from both tables
- [ ] Non-matching rows → NULL on missing side
- [ ] Not supported in MySQL (use UNION of LEFT + RIGHT)

**CROSS JOIN**
- [ ] Every row in left × every row in right (Cartesian product)
- [ ] Use case: generate all combinations
- [ ] Dangerous without WHERE — can produce massive results

**SELF JOIN**
- [ ] Join a table to itself
- [ ] Use case: employee-manager hierarchy, finding duplicates

### Join Internals (Understanding)

- [ ] Nested Loop Join — for small tables or indexed joins
- [ ] Hash Join — for large unsorted tables
- [ ] Merge Join — for pre-sorted data
- [ ] The query planner chooses automatically

### Understand

- [ ] Always use explicit JOIN syntax, not comma-separated FROM
- [ ] Table aliases are essential for readability
- [ ] JOIN condition vs WHERE condition — difference matters for outer joins
- [ ] Joining on non-indexed columns is slow
- [ ] Multiple joins: order generally doesn't matter (optimizer handles it)

**Exercises**
- [ ] Employees with their department names
- [ ] All customers including those with no orders (LEFT JOIN)
- [ ] Employees and their managers (SELF JOIN)
- [ ] Find customers who never placed an order

---

## Phase 9: Subqueries

### Types of Subqueries

**Scalar Subquery** — returns single value
```sql
SELECT name, salary,
       (SELECT AVG(salary) FROM employees) AS avg_sal
FROM employees;
```

**Row Subquery** — returns single row

**Table Subquery** — returns multiple rows (use in FROM)
```sql
SELECT dept, avg_sal
FROM (
    SELECT department AS dept, AVG(salary) AS avg_sal
    FROM employees
    GROUP BY department
) AS dept_avg
WHERE avg_sal > 60000;
```

**Correlated Subquery** — references outer query
```sql
SELECT name, salary
FROM employees e1
WHERE salary > (
    SELECT AVG(salary)
    FROM employees e2
    WHERE e2.department = e1.department
);
```

### Subquery Operators

- [ ] `IN (subquery)`
- [ ] `NOT IN (subquery)`
- [ ] `EXISTS (subquery)` — returns true if any row found
- [ ] `NOT EXISTS (subquery)`
- [ ] `ANY` / `SOME`
- [ ] `ALL`

### EXISTS vs IN

- [ ] EXISTS stops at first match (faster for large sets)
- [ ] IN evaluates entire subquery first
- [ ] NOT IN with NULLs — dangerous gotcha (returns no rows)
- [ ] NOT EXISTS is generally safer than NOT IN

### Understand

- [ ] Correlated subqueries execute once per outer row — can be slow
- [ ] Often replaceable with JOINs or window functions (better performance)
- [ ] Scalar subqueries in SELECT execute once per row

**Exercises**
- [ ] Employees earning above department average
- [ ] Customers who placed at least one order (EXISTS)
- [ ] Products never ordered (NOT EXISTS)

---

## Phase 10: Set Operations

### Operations

**UNION** — combine results, remove duplicates
```sql
SELECT city FROM customers
UNION
SELECT city FROM suppliers;
```

**UNION ALL** — combine results, keep duplicates (faster)

**INTERSECT** — rows in both queries

**EXCEPT / MINUS** — rows in first but not second
- [ ] `EXCEPT` — PostgreSQL, SQL Server
- [ ] `MINUS` — Oracle

### Rules

- [ ] Same number of columns in both queries
- [ ] Compatible data types in each column position
- [ ] Column names come from first query
- [ ] ORDER BY applies to final result

### Understand

- [ ] UNION ALL is faster than UNION (no deduplication)
- [ ] Use UNION ALL unless you specifically need deduplication
- [ ] INTERSECT and EXCEPT can usually be rewritten with JOINs

**Exercises**
- [ ] All cities from both customers and suppliers
- [ ] Customers who are also suppliers (INTERSECT)
- [ ] Products never sold (EXCEPT)

---

## Phase 11: Data Manipulation (DML)

### INSERT

```sql
-- Single row
INSERT INTO employees (name, salary, dept_id)
VALUES ('Alice', 75000, 3);

-- Multiple rows
INSERT INTO employees (name, salary, dept_id)
VALUES ('Bob', 80000, 2),
       ('Carol', 70000, 1);

-- Insert from SELECT
INSERT INTO archive_orders
SELECT * FROM orders WHERE order_date < '2020-01-01';
```

### UPDATE

```sql
UPDATE employees
SET salary = salary * 1.10
WHERE department = 'Engineering';
```

- [ ] Always use WHERE with UPDATE (or update all rows intentionally)
- [ ] Update multiple columns: `SET col1 = val1, col2 = val2`
- [ ] Update with JOIN (platform-specific syntax)

### DELETE

```sql
DELETE FROM employees
WHERE employee_id = 42;
```

- [ ] Always use WHERE with DELETE
- [ ] `DELETE FROM table` without WHERE deletes ALL rows
- [ ] TRUNCATE vs DELETE — know the difference

### TRUNCATE vs DELETE vs DROP

| | TRUNCATE | DELETE | DROP |
|---|---|---|---|
| Removes | All rows | Specified rows | Entire table |
| WHERE clause | No | Yes | No |
| Rollback | Platform-dependent | Yes | No (usually) |
| Speed | Fast | Slower | Instant |
| Resets identity | Usually yes | No | N/A |

### UPSERT (INSERT or UPDATE)

- [ ] `INSERT ... ON CONFLICT DO UPDATE` (PostgreSQL)
- [ ] `MERGE` statement (SQL Server, Oracle)
- [ ] `INSERT ... ON DUPLICATE KEY UPDATE` (MySQL)

### Understand

- [ ] Test UPDATE/DELETE with a SELECT first using same WHERE
- [ ] Use transactions to make DML reversible
- [ ] Bulk inserts are much faster than row-by-row

**Exercises**
- [ ] Give 10% raise to all managers
- [ ] Delete orders older than 5 years
- [ ] Copy inactive customers to archive table

---

## Phase 12: Data Definition (DDL)

### CREATE TABLE

```sql
CREATE TABLE employees (
    employee_id  INT          PRIMARY KEY,
    name         VARCHAR(100) NOT NULL,
    email        VARCHAR(150) UNIQUE,
    salary       DECIMAL(10,2),
    dept_id      INT          REFERENCES departments(id),
    created_at   TIMESTAMP    DEFAULT CURRENT_TIMESTAMP
);
```

### ALTER TABLE

- [ ] `ADD COLUMN`
- [ ] `DROP COLUMN`
- [ ] `RENAME COLUMN`
- [ ] `ALTER COLUMN` / `MODIFY COLUMN` (platform syntax varies)
- [ ] `ADD CONSTRAINT`
- [ ] `DROP CONSTRAINT`
- [ ] `RENAME TABLE`

### DROP TABLE

- [ ] `DROP TABLE table_name`
- [ ] `DROP TABLE IF EXISTS table_name`
- [ ] `CASCADE` — also drop dependent objects

### TRUNCATE TABLE

- [ ] Removes all rows, keeps structure

### Understand

- [ ] DDL changes are usually auto-committed (can't rollback)
- [ ] ALTER TABLE on large tables can lock the table (production concern)
- [ ] Schema migrations — concept of versioned DDL changes
- [ ] Tools: Flyway, Liquibase, Alembic for migrations

---

## Phase 13: Constraints & Data Integrity

### Types of Constraints

**PRIMARY KEY**
- [ ] Uniquely identifies each row
- [ ] Implicitly NOT NULL + UNIQUE
- [ ] Can be composite (multiple columns)

**FOREIGN KEY**
- [ ] Links to primary key in another table
- [ ] Enforces referential integrity
- [ ] `ON DELETE CASCADE` / `ON DELETE SET NULL` / `ON DELETE RESTRICT`

**UNIQUE**
- [ ] All values in column must be distinct
- [ ] NULLs handling varies by platform

**NOT NULL**
- [ ] Column must have a value

**CHECK**
- [ ] Custom condition: `CHECK (salary > 0)`
- [ ] `CHECK (status IN ('active', 'inactive'))`

**DEFAULT**
- [ ] Default value when none provided

### Understand

- [ ] Constraints are enforced by the database, not application code
- [ ] Enforcing in DB is safer than application-level only
- [ ] Foreign keys have performance cost on writes
- [ ] Disabling FK checks temporarily for bulk loads (with care)

---

## Phase 14: String Functions

### Common Functions (concept — syntax varies by platform)

**Case**
- [ ] `UPPER()` / `LOWER()`
- [ ] `INITCAP()` (PostgreSQL, Oracle)

**Length**
- [ ] `LENGTH()` / `LEN()` (SQL Server)
- [ ] `CHAR_LENGTH()`

**Trimming**
- [ ] `TRIM()` — both sides
- [ ] `LTRIM()` / `RTRIM()`
- [ ] `TRIM(LEADING 'x' FROM col)` (ANSI)

**Substring**
- [ ] `SUBSTRING(col, start, length)`
- [ ] `LEFT(col, n)` / `RIGHT(col, n)`
- [ ] `MID()` (MySQL)

**Search**
- [ ] `POSITION('sub' IN col)` / `CHARINDEX()` (SQL Server) / `INSTR()` (Oracle)
- [ ] `STRPOS(col, 'sub')` (PostgreSQL)

**Replace**
- [ ] `REPLACE(col, 'old', 'new')`
- [ ] `REGEXP_REPLACE()` — regex-based replace

**Concatenation**
- [ ] `CONCAT(col1, col2)`
- [ ] `||` operator (PostgreSQL, SQLite, Oracle)
- [ ] `+` operator (SQL Server)
- [ ] `CONCAT_WS(',', col1, col2)` — with separator

**Padding**
- [ ] `LPAD(col, length, 'char')` / `RPAD()`

**Splitting**
- [ ] `SPLIT_PART(col, delimiter, position)` (PostgreSQL)
- [ ] `STRING_SPLIT()` (SQL Server)

**Regular Expressions**
- [ ] `REGEXP_MATCH()` / `~` (PostgreSQL)
- [ ] `REGEXP_LIKE()` (Oracle, MySQL)

### Understand

- [ ] String functions differ most across platforms
- [ ] Applying functions to indexed columns prevents index use
- [ ] Regular expressions are powerful but slow — use carefully

---

## Phase 15: Numeric Functions

### Common Functions

- [ ] `ROUND(col, decimals)`
- [ ] `CEIL()` / `CEILING()`
- [ ] `FLOOR()`
- [ ] `TRUNC()` / `TRUNCATE()`
- [ ] `ABS()`
- [ ] `MOD(a, b)` / `a % b` — remainder
- [ ] `POWER(base, exp)` / `POW()`
- [ ] `SQRT()`
- [ ] `EXP()` — e^x
- [ ] `LN()` — natural log
- [ ] `LOG(base, n)` / `LOG10()`
- [ ] `SIGN()` — returns -1, 0, or 1
- [ ] `RANDOM()` / `RAND()` — random number

### Understand

- [ ] ROUND behavior on .5 differs across platforms
- [ ] Integer division vs float division — know your platform
- [ ] NUMERIC/DECIMAL for money, never FLOAT

---

## Phase 16: Date & Time Functions

### Getting Current Date/Time

- [ ] `CURRENT_DATE` — date only
- [ ] `CURRENT_TIME` — time only
- [ ] `CURRENT_TIMESTAMP` / `NOW()` — date + time
- [ ] `GETDATE()` (SQL Server)
- [ ] `SYSDATE` (Oracle)

### Extracting Parts

- [ ] `EXTRACT(YEAR FROM date_col)`
- [ ] `EXTRACT(MONTH FROM date_col)`
- [ ] `EXTRACT(DAY FROM date_col)`
- [ ] `EXTRACT(DOW FROM date_col)` — day of week
- [ ] `EXTRACT(HOUR FROM timestamp_col)`
- [ ] `DATE_PART()` (PostgreSQL)
- [ ] `YEAR()` / `MONTH()` / `DAY()` (MySQL, SQL Server)

### Arithmetic

- [ ] `date + INTERVAL '1 day'`
- [ ] `date - INTERVAL '3 months'`
- [ ] `DATEADD(unit, n, date)` (SQL Server)
- [ ] `DATE_ADD(date, INTERVAL n unit)` (MySQL)
- [ ] `DATEDIFF(unit, start, end)` — difference between dates
- [ ] `AGE(timestamp, timestamp)` (PostgreSQL)

### Formatting

- [ ] `TO_CHAR(date, 'YYYY-MM-DD')` (PostgreSQL, Oracle)
- [ ] `DATE_FORMAT(date, '%Y-%m-%d')` (MySQL)
- [ ] `FORMAT(date, 'yyyy-MM-dd')` (SQL Server)
- [ ] `TO_DATE('2024-01-15', 'YYYY-MM-DD')` — string to date

### Truncation

- [ ] `DATE_TRUNC('month', timestamp)` (PostgreSQL)
- [ ] `TRUNC(date, 'MM')` (Oracle)

### Understand

- [ ] Timezone handling is critical for production systems
- [ ] Store timestamps in UTC, convert at display time
- [ ] TIMESTAMPTZ vs TIMESTAMP (PostgreSQL)
- [ ] Date arithmetic is one of the most platform-specific areas

**Exercises**
- [ ] Orders placed in the last 30 days
- [ ] Calculate customer age from birthdate
- [ ] Monthly sales aggregation from daily data

---

## Phase 17: NULL Handling

### What NULL Means

- [ ] NULL = absence of value (not zero, not empty string)
- [ ] NULL is unknown — not comparable

### NULL Rules

- [ ] `NULL = NULL` → NULL (not TRUE) — this is the key gotcha
- [ ] `NULL != NULL` → NULL
- [ ] Any arithmetic with NULL → NULL
- [ ] Any comparison with NULL → NULL
- [ ] `NOT IN (...)` with NULL in list → returns nothing

### NULL Functions

- [ ] `IS NULL` / `IS NOT NULL` — only correct way to check NULL
- [ ] `COALESCE(col, default)` — return first non-NULL value
- [ ] `NULLIF(a, b)` — return NULL if a = b, else return a
- [ ] `IFNULL(col, default)` (MySQL)
- [ ] `NVL(col, default)` (Oracle)
- [ ] `ISNULL(col, default)` (SQL Server)

### NULL in Aggregates

- [ ] COUNT(*) counts NULLs; COUNT(col) ignores NULLs
- [ ] SUM / AVG / MIN / MAX all ignore NULLs
- [ ] This can silently give wrong results

### Understand

- [ ] Three-valued logic: TRUE, FALSE, UNKNOWN
- [ ] `WHERE col != 'Sales'` does NOT return NULL rows
- [ ] COALESCE is the most portable NULL handler
- [ ] NOT IN with NULLs is a famous SQL trap

**Exercises**
- [ ] Find all rows where phone number is missing
- [ ] Replace NULL salary with 0 using COALESCE
- [ ] Explain why NOT IN returns empty when NULL exists in list

---

## Phase 18: CASE Expressions

### Simple CASE

```sql
SELECT name,
       CASE grade
           WHEN 'A' THEN 'Excellent'
           WHEN 'B' THEN 'Good'
           ELSE 'Needs Improvement'
       END AS feedback
FROM students;
```

### Searched CASE

```sql
SELECT name, salary,
       CASE
           WHEN salary >= 100000 THEN 'High'
           WHEN salary >= 50000  THEN 'Medium'
           ELSE 'Low'
       END AS salary_band
FROM employees;
```

### CASE Uses

- [ ] In SELECT for derived columns
- [ ] In ORDER BY for custom sort order
- [ ] In GROUP BY for bucketing
- [ ] In aggregate functions for conditional aggregation

```sql
-- Conditional aggregation
SELECT
    COUNT(CASE WHEN status = 'active' THEN 1 END) AS active_count,
    COUNT(CASE WHEN status = 'inactive' THEN 1 END) AS inactive_count
FROM customers;
```

### Understand

- [ ] CASE is an expression, not a statement — it returns a value
- [ ] Can be used anywhere an expression is valid
- [ ] ELSE is optional — without it, unmatched rows return NULL
- [ ] Conditional aggregation replaces multiple GROUP BY queries

**Exercises**
- [ ] Categorize products by price range
- [ ] Pivot monthly sales into columns using CASE
- [ ] Count active vs inactive customers in one query

---

## Phase 19: Window Functions

### Why Window Functions Exist

- [ ] Aggregates collapse rows — you lose individual row data
- [ ] Window functions compute across a set of rows while keeping each row

### Core Syntax

```sql
function_name() OVER (
    PARTITION BY col
    ORDER BY col
    ROWS BETWEEN ... AND ...
)
```

### Ranking Functions

- [ ] `ROW_NUMBER()` — unique sequential number (no ties)
- [ ] `RANK()` — ties get same rank, next rank skips
- [ ] `DENSE_RANK()` — ties get same rank, no gaps
- [ ] `NTILE(n)` — divide rows into n buckets
- [ ] `PERCENT_RANK()` — relative rank 0 to 1
- [ ] `CUME_DIST()` — cumulative distribution

### Offset Functions

- [ ] `LAG(col, n)` — value from n rows before
- [ ] `LEAD(col, n)` — value from n rows ahead
- [ ] `FIRST_VALUE(col)` — first value in window
- [ ] `LAST_VALUE(col)` — last value in window
- [ ] `NTH_VALUE(col, n)` — nth value in window

### Aggregate Window Functions

- [ ] `SUM() OVER (...)` — running total or group total
- [ ] `AVG() OVER (...)`
- [ ] `COUNT() OVER (...)`
- [ ] `MIN() OVER (...)` / `MAX() OVER (...)`

### Frame Specification

```sql
-- Running total
SUM(sales) OVER (ORDER BY date ROWS BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW)

-- 7-day moving average
AVG(sales) OVER (ORDER BY date ROWS BETWEEN 6 PRECEDING AND CURRENT ROW)

-- Whole partition total
SUM(sales) OVER (PARTITION BY dept)
```

- [ ] `ROWS BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW`
- [ ] `ROWS BETWEEN n PRECEDING AND n FOLLOWING`
- [ ] `RANGE BETWEEN` vs `ROWS BETWEEN` — behavior with ties

### PARTITION BY vs GROUP BY

| | GROUP BY | PARTITION BY |
|---|---|---|
| Output | One row per group | All rows kept |
| Use | Aggregated reports | Row-level analytics |

### Understand

- [ ] Window functions execute after WHERE, GROUP BY, HAVING
- [ ] Can't use window functions in WHERE (wrap in subquery/CTE)
- [ ] PARTITION BY divides rows into independent windows
- [ ] ORDER BY inside OVER defines row order within window
- [ ] Without ORDER BY, frame is entire partition by default

**Exercises**
- [ ] Rank employees by salary within department
- [ ] Running total of monthly sales
- [ ] Compare each order to previous order (LAG)
- [ ] Top N per group using ROW_NUMBER()
- [ ] 7-day moving average of daily sales

---

## Phase 20: CTEs & Recursive Queries

### Common Table Expressions (CTEs)

```sql
WITH dept_avg AS (
    SELECT department, AVG(salary) AS avg_sal
    FROM employees
    GROUP BY department
)
SELECT e.name, e.salary, d.avg_sal
FROM employees e
JOIN dept_avg d ON e.department = d.department
WHERE e.salary > d.avg_sal;
```

### Benefits of CTEs

- [ ] Readability — name complex subqueries
- [ ] Reusability — reference same CTE multiple times
- [ ] Debugging — test each CTE independently

### Multiple CTEs

```sql
WITH
cte1 AS (...),
cte2 AS (...),
cte3 AS (... JOIN cte1 ...)
SELECT * FROM cte3;
```

### CTEs vs Subqueries vs Temp Tables

| | CTE | Subquery | Temp Table |
|---|---|---|---|
| Readable | ✅ High | ❌ Low | ✅ High |
| Reusable in query | ✅ Yes | ❌ No | ✅ Yes |
| Persists | ❌ No | ❌ No | ✅ Yes |
| Indexable | ❌ No | ❌ No | ✅ Yes |

### Recursive CTEs

```sql
WITH RECURSIVE org_chart AS (
    -- Base case
    SELECT employee_id, name, manager_id, 0 AS level
    FROM employees
    WHERE manager_id IS NULL

    UNION ALL

    -- Recursive case
    SELECT e.employee_id, e.name, e.manager_id, oc.level + 1
    FROM employees e
    JOIN org_chart oc ON e.manager_id = oc.employee_id
)
SELECT * FROM org_chart;
```

### Use Cases for Recursive CTEs

- [ ] Organizational hierarchies (employee → manager)
- [ ] Bill of materials (product → components)
- [ ] Category trees
- [ ] Graph traversal
- [ ] Date sequence generation

### Understand

- [ ] CTEs are not always materialized — optimizer may inline them
- [ ] In PostgreSQL, CTEs are optimization fences (materialized by default until pg12)
- [ ] `WITH RECURSIVE` syntax varies: PostgreSQL, MySQL 8+, SQL Server
- [ ] Always add a termination condition to avoid infinite loops

**Exercises**
- [ ] Rewrite a complex nested subquery as a CTE
- [ ] Employee hierarchy with levels using recursive CTE
- [ ] Generate a sequence of dates for a date range

---

## Phase 21: Views

### What is a View?

- [ ] A saved SELECT query with a name
- [ ] Behaves like a table in queries
- [ ] Does not store data (by default)

### Creating Views

```sql
CREATE VIEW active_customers AS
SELECT customer_id, name, email
FROM customers
WHERE status = 'active';
```

### Using Views

```sql
SELECT * FROM active_customers WHERE city = 'Mumbai';
```

### Modifying Views

- [ ] `CREATE OR REPLACE VIEW`
- [ ] `ALTER VIEW` (SQL Server)
- [ ] `DROP VIEW`

### Updatable Views

- [ ] Simple views on one table can be INSERT/UPDATE/DELETE
- [ ] Complex views (joins, aggregates) are read-only

### Materialized Views

- [ ] Stores the result physically (unlike regular views)
- [ ] Must be refreshed: `REFRESH MATERIALIZED VIEW`
- [ ] Can be indexed
- [ ] Use for expensive queries that don't need real-time data
- [ ] Available in: PostgreSQL, Oracle, SQL Server (indexed views)
- [ ] Not in: MySQL (workaround with tables + triggers)

### Understand

- [ ] Views add a layer of abstraction
- [ ] Views don't improve performance (regular views)
- [ ] Materialized views DO improve performance at cost of staleness
- [ ] Views can simplify security (expose only certain columns)

**Exercises**
- [ ] Create a view for public-facing customer data (hide sensitive cols)
- [ ] Create a materialized view for a slow monthly summary query

---

## Phase 22: Indexes

### What is an Index?

- [ ] A data structure that speeds up lookups
- [ ] Like a book's index vs reading every page

### Index Types

**B-Tree Index** (default)
- [ ] Best for equality, range, ORDER BY, LIKE 'prefix%'
- [ ] Balanced tree structure

**Hash Index**
- [ ] Only equality comparisons (`=`)
- [ ] Faster than B-Tree for equality
- [ ] PostgreSQL, MySQL

**GIN Index** (PostgreSQL)
- [ ] Full-text search, arrays, JSONB
- [ ] Generalized Inverted Index

**GiST Index** (PostgreSQL)
- [ ] Geometric data, full-text, range types

**Bitmap Index** (Oracle, some data warehouses)
- [ ] Low cardinality columns (gender, status)

**Covering Index / Index Include**
- [ ] Index includes all columns needed by query
- [ ] Query satisfied entirely from index (no table access)

**Partial Index**
- [ ] Index only rows meeting a condition
- [ ] `CREATE INDEX idx ON orders(customer_id) WHERE status = 'active'`

**Composite Index**
- [ ] Index on multiple columns
- [ ] Column order matters — leftmost prefix rule

### Creating Indexes

```sql
-- Single column
CREATE INDEX idx_employees_dept ON employees(department);

-- Composite
CREATE INDEX idx_orders_customer_date ON orders(customer_id, order_date);

-- Unique
CREATE UNIQUE INDEX idx_users_email ON users(email);

-- Partial (PostgreSQL)
CREATE INDEX idx_active_orders ON orders(customer_id)
WHERE status = 'active';
```

### When Indexes Help

- [ ] High-cardinality columns (many distinct values)
- [ ] Columns used in WHERE, JOIN ON, ORDER BY
- [ ] Foreign key columns
- [ ] Columns used in GROUP BY frequently

### When Indexes Hurt

- [ ] Tables with frequent INSERT/UPDATE/DELETE (index maintenance cost)
- [ ] Very small tables (full scan faster)
- [ ] Low-cardinality columns (e.g., boolean flag)
- [ ] Columns with functions applied in query (`WHERE UPPER(name) = ...`)

### Index Internals

- [ ] B-Tree: O(log n) lookup, balanced tree with leaf nodes
- [ ] Heap vs Index scan
- [ ] Index-only scan (covering index)
- [ ] Bitmap heap scan
- [ ] Index selectivity — how many rows match

### Understand

- [ ] Indexes speed up reads, slow down writes
- [ ] Too many indexes → slow INSERT/UPDATE
- [ ] Unused indexes waste space and slow writes — audit them
- [ ] Composite index column order = (equality cols first, range col last)
- [ ] `EXPLAIN` / `EXPLAIN ANALYZE` shows if index is used

**Exercises**
- [ ] Add index to foreign key column
- [ ] Create composite index for common query pattern
- [ ] Use EXPLAIN to verify index is being used

---

## Phase 23: Transactions & ACID

### What is a Transaction?

- [ ] A group of SQL statements that execute as one unit
- [ ] Either all succeed or all fail — no partial updates

### ACID Properties

**Atomicity**
- [ ] All or nothing — transaction fully commits or fully rolls back

**Consistency**
- [ ] Database moves from one valid state to another
- [ ] Constraints are enforced

**Isolation**
- [ ] Concurrent transactions don't interfere with each other

**Durability**
- [ ] Committed data survives crashes
- [ ] Written to persistent storage (WAL/redo log)

### Transaction Syntax

```sql
BEGIN;                          -- or START TRANSACTION

UPDATE accounts SET balance = balance - 500 WHERE id = 1;
UPDATE accounts SET balance = balance + 500 WHERE id = 2;

COMMIT;                         -- make permanent
-- or
ROLLBACK;                       -- undo everything
```

### Savepoints

```sql
BEGIN;
INSERT INTO orders ...;
SAVEPOINT sp1;
INSERT INTO order_items ...;
ROLLBACK TO SAVEPOINT sp1;      -- undo back to savepoint
COMMIT;
```

### Isolation Levels

| Level | Dirty Read | Non-Repeatable Read | Phantom Read |
|---|---|---|---|
| READ UNCOMMITTED | Possible | Possible | Possible |
| READ COMMITTED | ❌ | Possible | Possible |
| REPEATABLE READ | ❌ | ❌ | Possible |
| SERIALIZABLE | ❌ | ❌ | ❌ |

- [ ] `SET TRANSACTION ISOLATION LEVEL ...`
- [ ] PostgreSQL default: READ COMMITTED
- [ ] MySQL InnoDB default: REPEATABLE READ

### Concurrency Problems

- [ ] **Dirty Read** — reading uncommitted data from another transaction
- [ ] **Non-Repeatable Read** — reading same row twice, different results
- [ ] **Phantom Read** — new rows appear between reads in same transaction
- [ ] **Lost Update** — two transactions overwrite each other's changes
- [ ] **Deadlock** — two transactions wait for each other's locks

### Locking

- [ ] Row-level locks
- [ ] Table-level locks
- [ ] `SELECT ... FOR UPDATE` — lock rows for update
- [ ] `SELECT ... FOR SHARE` — share lock
- [ ] Optimistic vs Pessimistic locking strategies

### Understand

- [ ] Auto-commit is on by default in most clients
- [ ] Long transactions hold locks — keep transactions short
- [ ] Deadlock detection and resolution is automatic in most DBs
- [ ] WAL (Write-Ahead Log) enables durability and replication

**Exercises**
- [ ] Bank transfer between accounts using transaction
- [ ] Simulate a deadlock and observe behavior

---

## Phase 24: Query Execution & Internals

### How a Query Executes

```
SQL Text
    ↓
Parser (syntax check)
    ↓
Rewriter (view expansion, rule application)
    ↓
Query Planner / Optimizer
    ↓
Query Executor
    ↓
Result
```

### Query Planner

- [ ] Parses SQL into logical plan
- [ ] Generates multiple physical plan options
- [ ] Estimates costs using statistics
- [ ] Chooses lowest-cost plan

### Statistics

- [ ] Table statistics: row counts, data distribution
- [ ] `ANALYZE` / `UPDATE STATISTICS` — update statistics
- [ ] `pg_stats` in PostgreSQL
- [ ] Histograms on columns
- [ ] Statistics drive join order and index choices

### EXPLAIN

```sql
EXPLAIN SELECT * FROM employees WHERE department = 'Sales';
EXPLAIN ANALYZE SELECT * FROM employees WHERE department = 'Sales';
```

### Reading EXPLAIN Output

- [ ] Seq Scan — full table scan (no index used)
- [ ] Index Scan — uses index, accesses heap
- [ ] Index Only Scan — uses index, no heap access
- [ ] Bitmap Heap Scan — uses index bitmap, then heap
- [ ] Hash Join / Nested Loop / Merge Join
- [ ] Cost: startup cost + total cost
- [ ] Rows: estimated row count
- [ ] Actual time and rows (EXPLAIN ANALYZE only)
- [ ] Buffers: memory and disk blocks read

### Page & Buffer Architecture

- [ ] Data stored in pages (8KB in PostgreSQL)
- [ ] Buffer pool / shared buffers — cache of pages in memory
- [ ] Page hit (in memory) vs page read (from disk)
- [ ] Sequential vs random I/O

### Write-Ahead Log (WAL)

- [ ] All changes written to WAL before data pages
- [ ] Enables crash recovery
- [ ] Basis for replication

### Understand

- [ ] Database is fundamentally an I/O problem
- [ ] Memory (buffer pool) is much faster than disk
- [ ] Good queries minimize I/O
- [ ] Statistics must be current for good plans

---

## Phase 25: Query Optimization

### Read the Query Plan First

- [ ] Use EXPLAIN ANALYZE before optimizing
- [ ] Identify the most expensive node
- [ ] Look for Seq Scans on large tables
- [ ] Look for bad row estimates

### Common Optimizations

**Add Indexes**
- [ ] On WHERE columns
- [ ] On JOIN columns (especially FK side)
- [ ] On ORDER BY columns
- [ ] Covering indexes for frequently run queries

**Rewrite Queries**
- [ ] Replace correlated subqueries with JOINs
- [ ] Replace `NOT IN` with `NOT EXISTS` or LEFT JOIN
- [ ] Replace `SELECT *` with specific columns
- [ ] Push filters as early as possible (filter before join)
- [ ] Avoid functions on indexed columns in WHERE

**Avoid Common Anti-Patterns**
- [ ] `WHERE UPPER(name) = 'ALICE'` → index not used (use functional index)
- [ ] `WHERE col + 1 = 5` → rewrite as `WHERE col = 4`
- [ ] `SELECT DISTINCT` when DISTINCT not needed
- [ ] Implicit type conversion in WHERE (disables index)
- [ ] `OR` on different columns (use UNION ALL instead)

**Pagination**
- [ ] Avoid deep OFFSET pagination (gets slower with higher offset)
- [ ] Use keyset/cursor pagination: `WHERE id > last_seen_id ORDER BY id LIMIT n`

**Batch Operations**
- [ ] Bulk INSERT instead of row-by-row
- [ ] Batch UPDATE/DELETE instead of single-row loops

**Partitioning**
- [ ] Partition large tables by date or category
- [ ] Query pruning — only scan relevant partitions

### Understand

- [ ] 80% of performance issues come from missing indexes
- [ ] Second biggest issue: bad query patterns
- [ ] Don't optimize prematurely — profile first
- [ ] Hardware limits: more RAM = bigger buffer pool = fewer disk reads

---

## Phase 26: Normalization & Schema Design

### Why Normalization?

- [ ] Eliminate data redundancy
- [ ] Prevent update anomalies
- [ ] Maintain data integrity

### Normal Forms

**1NF (First Normal Form)**
- [ ] No repeating groups
- [ ] Atomic values (one value per cell)
- [ ] Each row uniquely identifiable

**2NF (Second Normal Form)**
- [ ] In 1NF
- [ ] Every non-key column depends on the WHOLE primary key (no partial dependency)
- [ ] Applies when primary key is composite

**3NF (Third Normal Form)**
- [ ] In 2NF
- [ ] No transitive dependencies (non-key columns depend only on key, not on other non-key columns)

**BCNF (Boyce-Codd Normal Form)**
- [ ] Stronger version of 3NF

**4NF / 5NF**
- [ ] Multi-valued dependencies (rarely needed in practice)

### Denormalization

- [ ] Intentionally introduce redundancy for performance
- [ ] Pre-computed columns, duplicate data
- [ ] Common in OLAP / data warehouses

### Schema Patterns

**OLTP Schema (Normalized)**
- [ ] Optimized for writes
- [ ] Star schema NOT ideal (too many joins)
- [ ] 3NF typically

**OLAP / Data Warehouse Schema**

- [ ] Star Schema: fact table + dimension tables
- [ ] Snowflake Schema: normalized dimensions
- [ ] Wide table / flat table: fully denormalized

### Star Schema

- [ ] Fact Table: events/transactions (sales, orders)
- [ ] Dimension Tables: context (customers, products, dates, regions)
- [ ] Optimized for analytical queries (few joins)

### Understand

- [ ] Real-world DBs are rarely perfectly normalized
- [ ] Balance normalization with query performance
- [ ] Data warehouses favor denormalization for query speed
- [ ] Surrogate keys vs natural keys debate

---

## Phase 27: Stored Procedures & Functions

### Stored Procedures

```sql
-- PostgreSQL
CREATE OR REPLACE PROCEDURE update_salary(emp_id INT, increase DECIMAL)
LANGUAGE plpgsql AS $$
BEGIN
    UPDATE employees
    SET salary = salary * (1 + increase)
    WHERE employee_id = emp_id;
END;
$$;

CALL update_salary(42, 0.10);
```

### Functions (UDF — User Defined Functions)

```sql
CREATE OR REPLACE FUNCTION get_annual_salary(monthly DECIMAL)
RETURNS DECIMAL AS $$
BEGIN
    RETURN monthly * 12;
END;
$$ LANGUAGE plpgsql;

SELECT name, get_annual_salary(salary) FROM employees;
```

### Procedure vs Function

| | Procedure | Function |
|---|---|---|
| Returns value | Optional (OUT params) | Yes |
| Use in SELECT | No | Yes |
| Transaction control | Yes (some platforms) | Typically no |
| Purpose | Actions/side effects | Computations |

### Procedural Languages

- [ ] PL/pgSQL (PostgreSQL)
- [ ] T-SQL (SQL Server)
- [ ] PL/SQL (Oracle)
- [ ] MySQL stored procedures

### Understand

- [ ] Stored procedures reduce network round-trips
- [ ] Logic in DB vs application layer — tradeoffs
- [ ] Hard to version control and test
- [ ] Modern trend: keep business logic in application, use SQL for data

---

## Phase 28: Triggers

### What is a Trigger?

- [ ] Automatically executes when a specified event occurs on a table

### Trigger Events

- [ ] `BEFORE INSERT` / `AFTER INSERT`
- [ ] `BEFORE UPDATE` / `AFTER UPDATE`
- [ ] `BEFORE DELETE` / `AFTER DELETE`
- [ ] `INSTEAD OF` (for views)

### Example

```sql
CREATE OR REPLACE FUNCTION log_salary_change()
RETURNS TRIGGER AS $$
BEGIN
    INSERT INTO salary_audit(emp_id, old_salary, new_salary, changed_at)
    VALUES (OLD.employee_id, OLD.salary, NEW.salary, NOW());
    RETURN NEW;
END;
$$ LANGUAGE plpgsql;

CREATE TRIGGER salary_audit_trigger
AFTER UPDATE OF salary ON employees
FOR EACH ROW
EXECUTE FUNCTION log_salary_change();
```

### Use Cases

- [ ] Audit logging
- [ ] Enforcing complex business rules
- [ ] Maintaining derived columns
- [ ] Cascading updates

### Understand

- [ ] Triggers fire silently — hard to debug
- [ ] Can cause unexpected slowdowns if poorly written
- [ ] Modern systems often prefer application-level audit logs
- [ ] `NEW` = new row values / `OLD` = old row values

---

## Phase 29: Platform Differences

### Key Syntax Differences

| Feature | PostgreSQL | MySQL | SQL Server | Oracle |
|---|---|---|---|---|
| String concat | `\|\|` | `CONCAT()` | `+` | `\|\|` |
| Auto increment | `SERIAL` / `IDENTITY` | `AUTO_INCREMENT` | `IDENTITY` | `SEQUENCE` |
| Limit rows | `LIMIT n` | `LIMIT n` | `TOP n` | `FETCH FIRST n` |
| Current date | `CURRENT_DATE` | `CURDATE()` | `GETDATE()` | `SYSDATE` |
| String to date | `TO_DATE()` | `STR_TO_DATE()` | `CONVERT()` | `TO_DATE()` |
| Upsert | `ON CONFLICT` | `ON DUPLICATE KEY` | `MERGE` | `MERGE` |
| Regex | `~` / `REGEXP` | `REGEXP` | `LIKE` only | `REGEXP_LIKE` |
| True boolean | `BOOLEAN` | `TINYINT(1)` | `BIT` | No native |
| JSON support | `JSONB` (excellent) | `JSON` | `JSON` (limited) | `JSON` |
| Full-text search | `tsvector/tsquery` | `FULLTEXT` | `FULLTEXT` | Oracle Text |
| Recursive CTE | `WITH RECURSIVE` | MySQL 8+ | Standard | Standard |

### Cloud Data Warehouse Differences

| Feature | BigQuery | Snowflake | Redshift |
|---|---|---|---|
| Partitioning | Automatic | Clustering | Distribution keys |
| Cost model | Per query (bytes scanned) | Per second (compute) | Per hour (cluster) |
| Transactions | Limited | Full ACID | Limited |
| Nested data | Arrays, STRUCT | VARIANT (JSON) | SUPER type |
| Window functions | Full support | Full support | Full support |

### Understand

- [ ] Core SQL (SELECT, JOIN, WHERE, GROUP BY) is 90% portable
- [ ] Date functions and string functions vary most
- [ ] Auto-increment syntax is completely different
- [ ] Always check documentation for your specific platform

---

## Phase 30: SQL for Data Analysis

### Analytical Query Patterns

**Cohort Analysis**
```sql
-- First purchase month cohort
WITH cohorts AS (
    SELECT customer_id,
           DATE_TRUNC('month', MIN(order_date)) AS cohort_month
    FROM orders
    GROUP BY customer_id
)
SELECT cohort_month,
       DATE_TRUNC('month', o.order_date) AS order_month,
       COUNT(DISTINCT o.customer_id)
FROM orders o
JOIN cohorts c ON o.customer_id = c.customer_id
GROUP BY 1, 2;
```

**Retention Analysis**
- [ ] Day 1, Day 7, Day 30 retention
- [ ] Using self-joins or window functions

**Funnel Analysis**
- [ ] Steps in a conversion funnel
- [ ] Drop-off rates between steps

**RFM Analysis** (Recency, Frequency, Monetary)
- [ ] NTILE() for scoring customers

**Percentile Analysis**
- [ ] `PERCENTILE_CONT(0.5) WITHIN GROUP (ORDER BY col)`
- [ ] `APPROX_PERCENTILE()` for large datasets

**Pivot / Unpivot**
- [ ] CASE-based pivoting (portable)
- [ ] `PIVOT` / `UNPIVOT` (SQL Server, Oracle)
- [ ] `CROSSTAB()` (PostgreSQL)

**Time Series Analysis**
- [ ] Gap filling with date series
- [ ] Rolling averages with window frames
- [ ] Period-over-period comparison (LAG, DATEADD)

**Sessionization**
- [ ] Group events into sessions by time gap
- [ ] Using LAG + CASE + SUM window function

### Understand

- [ ] Most analytical patterns use CTEs + window functions
- [ ] Date dimensions (calendar tables) are very useful
- [ ] NULL handling is critical in analytical queries
- [ ] Performance matters at analytical scale — think before writing

---

## Phase 31: SQL for Data Engineering

### ETL Patterns in SQL

**Incremental Load**
```sql
INSERT INTO target
SELECT * FROM source
WHERE updated_at > (SELECT MAX(updated_at) FROM target);
```

**Upsert / Merge**
```sql
INSERT INTO target (id, name, updated_at)
SELECT id, name, updated_at FROM source
ON CONFLICT (id) DO UPDATE
SET name = EXCLUDED.name,
    updated_at = EXCLUDED.updated_at;
```

**SCD Type 2 (Slowly Changing Dimension)**
- [ ] Track historical changes in dimension tables
- [ ] `valid_from` / `valid_to` columns
- [ ] `is_current` flag

**Data Quality Checks**
```sql
-- Null check
SELECT COUNT(*) FROM orders WHERE customer_id IS NULL;

-- Duplicate check
SELECT order_id, COUNT(*)
FROM orders
GROUP BY order_id
HAVING COUNT(*) > 1;

-- Referential integrity check
SELECT o.order_id
FROM orders o
LEFT JOIN customers c ON o.customer_id = c.customer_id
WHERE c.customer_id IS NULL;
```

### Temporary Tables

```sql
CREATE TEMP TABLE temp_results AS
SELECT * FROM complex_query;

-- Available only for current session
DROP TABLE temp_results;
```

### Table Partitioning

```sql
-- PostgreSQL range partitioning
CREATE TABLE orders (
    order_id INT,
    order_date DATE
) PARTITION BY RANGE (order_date);

CREATE TABLE orders_2024 PARTITION OF orders
FOR VALUES FROM ('2024-01-01') TO ('2025-01-01');
```

### Data Warehouse Patterns

- [ ] Fact and dimension table loading
- [ ] Dimension table SCD handling
- [ ] Incremental vs full refresh
- [ ] Deduplication before loading
- [ ] Audit columns: `created_at`, `updated_at`, `created_by`

### Understand

- [ ] SQL is the backbone of most ETL/ELT pipelines
- [ ] ELT (Extract-Load-Transform) is now dominant in cloud DWH
- [ ] dbt (data build tool) uses SQL + Jinja for transformations
- [ ] Data quality checks should be automated

---

## Phase 32: SQL at Scale

### Partitioning

- [ ] Range partitioning (by date)
- [ ] List partitioning (by category)
- [ ] Hash partitioning (by key hash)
- [ ] Partition pruning — only scan relevant partitions
- [ ] Partition maintenance (adding, dropping old partitions)

### Sharding

- [ ] Horizontal scaling by splitting data across multiple nodes
- [ ] Shard key selection is critical
- [ ] Cross-shard queries are expensive

### Replication

- [ ] Primary-replica (master-slave) setup
- [ ] Read from replicas, write to primary
- [ ] Replication lag — replicas may be slightly behind
- [ ] Streaming replication vs logical replication

### Connection Pooling

- [ ] PgBouncer (PostgreSQL)
- [ ] ProxySQL (MySQL)
- [ ] Why: connections are expensive; pool reuses them

### Query at Scale

- [ ] Columnar storage (Parquet, ORC) vs row storage
- [ ] Why columnar is faster for analytics (read fewer columns)
- [ ] Compression benefits with columnar storage
- [ ] Vectorized execution (DuckDB, modern query engines)
- [ ] Parallel query execution

### Materialized Views at Scale

- [ ] Pre-aggregate expensive computations
- [ ] Refresh strategies (full, incremental)
- [ ] Tradeoff: freshness vs performance

### Understand

- [ ] Single-node PostgreSQL handles surprisingly large workloads
- [ ] Vertical scaling (bigger machine) before horizontal
- [ ] Read replicas for analytical workloads
- [ ] Cloud DWH (BigQuery, Snowflake) for truly large analytics

---

## Phase 33: Security & Access Control

### Users & Roles

```sql
-- Create user
CREATE USER analyst WITH PASSWORD 'secure_pass';

-- Create role
CREATE ROLE reporting;

-- Grant role to user
GRANT reporting TO analyst;
```

### Permissions

```sql
-- Grant privileges
GRANT SELECT ON employees TO analyst;
GRANT SELECT, INSERT ON orders TO app_user;
GRANT ALL PRIVILEGES ON ALL TABLES IN SCHEMA public TO admin;

-- Revoke
REVOKE DELETE ON orders FROM analyst;
```

### Row-Level Security (PostgreSQL)

```sql
ALTER TABLE orders ENABLE ROW LEVEL SECURITY;

CREATE POLICY user_orders ON orders
FOR SELECT USING (customer_id = current_user_id());
```

### SQL Injection

- [ ] What is SQL injection?
- [ ] How it works: unsanitized user input in SQL
- [ ] Prevention: parameterized queries / prepared statements
- [ ] ORM protection
- [ ] Never concatenate user input into SQL strings

### Data Masking

- [ ] Masking sensitive data in views
- [ ] Dynamic data masking (SQL Server, Oracle)

### Understand

- [ ] Principle of least privilege — give minimum needed permissions
- [ ] Application users should not have DDL privileges
- [ ] Audit logs for sensitive table access
- [ ] Encrypt sensitive columns (application-level or DB-level)

---

## Phase 34: Real Projects

### Beginner
- [ ] Employee database queries (filter, sort, aggregate)
- [ ] Simple sales report (GROUP BY, JOIN)
- [ ] Customer order history (multi-table JOIN)

### Intermediate
- [ ] E-commerce analytics (revenue, orders, customers)
- [ ] HR analytics (headcount, salary bands, tenure)
- [ ] Inventory management queries

### Advanced
- [ ] Cohort retention analysis
- [ ] RFM customer segmentation
- [ ] Sales funnel analysis with conversion rates
- [ ] Time series revenue with rolling averages
- [ ] Slowly Changing Dimension implementation

### Expert
- [ ] Design and build a normalized database from scratch
- [ ] Optimize a slow query using EXPLAIN ANALYZE
- [ ] Build an ETL pipeline using SQL only
- [ ] Implement row-level security for multi-tenant system
- [ ] Performance benchmark: index strategies comparison

---

## Final Mastery

### Fundamentals — Can Explain

- [ ] What SQL is and why it exists
- [ ] How a query executes (parsing → planning → execution)
- [ ] All JOIN types and when to use each
- [ ] GROUP BY execution order and why aliases don't work in WHERE
- [ ] NULL three-valued logic and common traps
- [ ] ACID properties with real examples
- [ ] Index types and when indexes help vs hurt
- [ ] Window functions vs GROUP BY — the fundamental difference

### Intermediate — Can Write

- [ ] Complex multi-table JOINs
- [ ] Window functions (ranking, running totals, LAG/LEAD)
- [ ] CTEs including recursive CTEs
- [ ] Conditional aggregation with CASE
- [ ] Efficient pagination with keyset pattern
- [ ] Upsert / Merge statements
- [ ] Date-based time series queries

### Advanced — Can Optimize

- [ ] Read and interpret EXPLAIN/EXPLAIN ANALYZE output
- [ ] Identify and fix slow queries
- [ ] Design appropriate indexes for query patterns
- [ ] Rewrite correlated subqueries as JOINs or window functions
- [ ] Avoid common anti-patterns (implicit conversions, OR on different cols)
- [ ] Choose appropriate isolation level for use case

### Expert / Senior — Can Design

- [ ] Design normalized schema (3NF) from business requirements
- [ ] Design star schema for analytical workloads
- [ ] Choose between OLTP and OLAP patterns
- [ ] Implement partitioning strategy for large tables
- [ ] Design for replication and read scaling
- [ ] Implement row-level security
- [ ] Write and review database migration scripts
- [ ] Reason about concurrency, locking, and deadlocks
- [ ] Make informed platform selection decisions

### True Senior Level

- [ ] Can explain query planner decisions
- [ ] Can diagnose production performance incidents
- [ ] Can design schemas that stay performant at 10x growth
- [ ] Can mentor others on SQL best practices
- [ ] Knows when NOT to use SQL (graph DBs, document stores, etc.)
- [ ] Understands CAP theorem and its implications
- [ ] Can implement CDC (Change Data Capture) patterns
- [ ] Contributes to database standards and conventions at org level
