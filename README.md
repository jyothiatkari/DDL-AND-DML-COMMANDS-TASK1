
## 🔹 DDL (Data Definition Language)

**DDL commands** are used to **define, modify, and manage the structure of database objects** such as tables, schemas, and indexes. These commands deal with the **design of the database**, not the data itself.


* **CREATE** – Creates database objects

  ```sql
  CREATE TABLE Student (id INT, name VARCHAR(50));
  ```
* **ALTER** – Modifies existing database objects

  ```sql
  ALTER TABLE Student ADD age INT;
  ```
* **DROP** – Deletes database objects permanently

  ```sql
  DROP TABLE Student;
  ```
* **TRUNCATE** – Removes all records from a table (structure remains)

  ```sql
  TRUNCATE TABLE Student;
  ```
* **RENAME** – Renames a database object

  ```sql
  RENAME TABLE Student TO Students;
  ```

### 🔸 Key Features of DDL:

* Affects **table structure**
* Changes are **auto-committed**
* Cannot be rolled back (in most DBMS)

---

## 🔹 DML (Data Manipulation Language)

**DML commands** are used to **manage and manipulate data** stored in database tables. These commands work on the **records inside tables**.


* **INSERT** – Adds new records

  ```sql
  INSERT INTO Student VALUES (1, 'Jyothi');
  ```
* **UPDATE** – Modifies existing records

  ```sql
  UPDATE Student SET name='Anu' WHERE id=1;
  ```
* **DELETE** – Removes records

  ```sql
  DELETE FROM Student WHERE id=1;
  ```
* **SELECT** – Retrieves data from tables

  ```sql
  SELECT * FROM Student;
  ```

### 🔸 Key Features of DML:

* Affects **data inside tables**
* Requires **COMMIT** to save changes
* Changes can be **rolled back**


### ✅ Conclusion

DDL commands are used for **building and modifying database structures**, while DML commands are used for **handling and managing data** within those structures. Both are essential for effective database management.

