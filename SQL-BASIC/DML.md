## 📌 What is DML?
**DML (Data Manipulation Language)** is a subset of SQL used to **insert, update, delete, and retrieve** data in the database.  
It deals with **data**, not the structure.

---

## 🛠 Common DML Commands
- `INSERT` → Add new data into a table.
- `UPDATE` → Modify existing data.
- `DELETE` → Remove existing data.
- `SELECT` → Retrieve data from a table.

---

## 📜 Example DML Commands

```sql
-- Insert a single row into the table
INSERT INTO student (id, email, name)
VALUES (1, 'ram@example.com', 'Ram');

-- Insert multiple rows
INSERT INTO student (id, email, name)
VALUES
(2, 'shyam@example.com', 'Shyam'),
(3, 'geeta@example.com', 'Geeta');

-- Retrieve all records
SELECT * FROM student;

-- Retrieve specific columns
SELECT name, email FROM student;

-- Retrieve data with condition
SELECT * FROM student WHERE name = 'Ram';

-- Retrieve data with sorting
SELECT * FROM student ORDER BY name ASC;

-- Update a single row
UPDATE student
SET name = 'Ramesh'
WHERE id = 1;

-- Update multiple rows
UPDATE student
SET marks = 90
WHERE marks IS NULL;

-- Delete a specific row
DELETE FROM student WHERE id = 3;

-- Delete all rows but keep the table
DELETE FROM student;
