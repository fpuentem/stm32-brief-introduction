---
theme: default
marp: true
title: Introduction to SQL
paginate: true
---

# Introduction to SQL

---

# What is SQL?

- SQL stands for **Structured Query Language**.
- It's a language used to communicate with databases.
- Allows users to **query**, **insert**, **update**, and **delete** data.

---

# Types of SQL Commands

1. DDL - Data Definition Language
   - Examples: `CREATE`, `ALTER`, `DROP`
2. DML - Data Manipulation Language
   - Examples: `SELECT`, `INSERT`, `UPDATE`, `DELETE`
3. DCL - Data Control Language
   - Examples: `GRANT`, `REVOKE`

---

# Basic SQL Query

```sql
SELECT column1, column2
FROM table_name
WHERE condition
ORDER BY column1;
