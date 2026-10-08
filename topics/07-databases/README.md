# Databases
## Core idea
A database organizes persistent data and provides ways to read and modify it. A database management system also handles concerns such as access, concurrency, and recovery.

## Relational basics
A relational model organizes data into relations, commonly represented as tables. A primary key identifies a row. A foreign key expresses a reference to a key in another—or the same—table.

For a student-course system, use students, courses, and enrollments rather than storing a comma-separated course list in each student row.

## Example
Given a students table with id and name columns:
```sql
SELECT id, name
FROM students
WHERE id = 42;
```
Use parameterized queries when values come from users rather than concatenating input into SQL.

## Indexes and transactions
An index can reduce the work needed for selected queries, at the cost of storage and maintenance during writes. Indexes do not make every query faster.

A transaction groups operations into a logical unit. ACID describes atomicity, consistency, isolation, and durability. The guarantees visible to an application depend on the database and configuration, especially its isolation level.

“NoSQL” covers multiple models, such as document, key-value, and graph databases. It does not mean “no schema” or “no transactions” in every product.

## Try it
Design an enrollments table. Explain how you would prevent a student from enrolling in the same course twice.

## Expand next
Joins; normalization; query plans; B-tree indexes; isolation levels; replication; backups; relational versus document modeling.

[Back to index](../../README.md)
