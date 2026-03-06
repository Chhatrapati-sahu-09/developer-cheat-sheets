# SQL Cheat Sheet

SQL is used to manage and query relational databases.

## Select Data

SELECT * FROM users;

Select specific columns

SELECT name, email FROM users;

---

## Insert Data

INSERT INTO users (name, email)
VALUES ('John', 'john@email.com');

---

## Update Data

UPDATE users
SET email = 'new@email.com'
WHERE id = 1;

---

## Delete Data

DELETE FROM users
WHERE id = 1;

---

## Filtering Data

SELECT * FROM users
WHERE age > 18;

---

## Sorting

SELECT * FROM users
ORDER BY name ASC;
