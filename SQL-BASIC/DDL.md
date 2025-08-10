
## 📌 What is DDL?
**DDL (Data Definition Language)** is a subset of SQL used to define and manage database objects such as tables, schemas, and indexes.  
It deals with **structure** — creating, altering, and deleting database objects.

**Common DDL Commands:**
- `CREATE` → Create a new table, database, or object.
- `ALTER` → Modify an existing object.
- `DROP` → Delete an object permanently.
- `TRUNCATE` → Remove all data from a table without deleting the table.

---

## 📜 Example DDL Commands

```sql
-- Show all databases
SHOW DATABASES;

-- Switch to a specific database
USE College;

-- Show all tables in the selected database
SHOW TABLES;

-- Create a table
CREATE TABLE student (
    id INT PRIMARY KEY,
    email VARCHAR(50) UNIQUE,
    name VARCHAR(50)
);

-- View table structure
DESCRIBE student;

-- Add a new column
ALTER TABLE student ADD marks INT;

-- Rename an existing column
ALTER TABLE student RENAME COLUMN marks TO mark;

-- Delete a column
ALTER TABLE student DROP COLUMN mark;

-- Modify a column
ALTER TABLE student MODIFY name VARCHAR(50) UNIQUE;

-- Remove all records from a table
TRUNCATE TABLE student;

-- Delete the table completely
DROP TABLE student;