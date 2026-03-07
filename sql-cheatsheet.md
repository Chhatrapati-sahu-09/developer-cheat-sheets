# SQL Cheat Sheet

SQL (Structured Query Language) is used to manage and query relational databases. It allows developers to create, read, update, and delete data stored in database tables.

This cheat sheet provides commonly used SQL commands and examples.

---

## Select Data

Retrieve all data from a table.

```sql
SELECT * FROM users;
```

Retrieve specific columns.

```sql
SELECT name, email FROM users;
```

---

## Insert Data

Add new records to a table.

```sql
INSERT INTO users (name, email)
VALUES ('John', 'john@email.com');
```

Insert multiple rows.

```sql
INSERT INTO users (name, email)
VALUES 
('Alice', 'alice@email.com'),
('Bob', 'bob@email.com');
```

---

## Update Data

Modify existing records in a table.

```sql
UPDATE users
SET email = 'new@email.com'
WHERE id = 1;
```

Update multiple columns.

```sql
UPDATE users
SET name = 'John Doe', email = 'john@example.com'
WHERE id = 1;
```

---

## Delete Data

Remove records from a table.

```sql
DELETE FROM users
WHERE id = 1;
```

Delete all records.

```sql
DELETE FROM users;
```

---

## Filtering Data

Filter records using conditions.

```sql
SELECT * FROM users
WHERE age > 18;
```

Using multiple conditions.

```sql
SELECT * FROM users
WHERE age > 18 AND city = 'London';
```

---

## Sorting Results

Sort records in ascending order.

```sql
SELECT * FROM users
ORDER BY name ASC;
```

Sort records in descending order.

```sql
SELECT * FROM users
ORDER BY age DESC;
```

---

## Limiting Results

Limit the number of returned rows.

```sql
SELECT * FROM users
LIMIT 5;
```

---

## Aggregate Functions

Perform calculations on data.

| Function | Description |
|---------|-------------|
| COUNT() | Counts number of rows |
| SUM() | Calculates total value |
| AVG() | Calculates average value |
| MAX() | Finds maximum value |
| MIN() | Finds minimum value |

Example:

```sql
SELECT COUNT(*) FROM users;
```

---

## GROUP BY

Group rows that have the same values.

```sql
SELECT city, COUNT(*)
FROM users
GROUP BY city;
```

---

## JOIN Operations

Join data from multiple tables.

### INNER JOIN

Returns records that match in both tables.

```sql
SELECT users.name, orders.product
FROM users
INNER JOIN orders
ON users.id = orders.user_id;
```

### LEFT JOIN

Returns all records from the left table and matched records from the right table.

```sql
SELECT users.name, orders.product
FROM users
LEFT JOIN orders
ON users.id = orders.user_id;
```

---

## Creating Tables

Create a new table.

```sql
CREATE TABLE users (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100)
);
```

---

## Dropping Tables

Delete a table permanently.

```sql
DROP TABLE users;
```

---

## Summary

SQL is essential for working with relational databases. Understanding these commands allows developers to efficiently retrieve, manipulate, and manage data in applications.
