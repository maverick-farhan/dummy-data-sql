# Dummy Data in SQL
## SQL Dummy Data 

### Create Database
```sql
CREATE database dummy_db;
```
---

### Switch to newly created Database
```sql
use dummy_db;
```
---

### Create Table
```sql
CREATE TABLE dummy_table(
id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(20) NOT NULL,
email VARCHAR(50) NOT NULL,
phone VARCHAR(12) NOT NULL UNIQUE,
address VARCHAR(50) NOT NULL
);
```
---

### Populate Table with Data
```sql
INSERT INTO dummy_table (
    name,email,phone,address
) VALUE 
(),
(),
(),
(),
(),
(),
(),
(),
(),
(),
(),
(),
(),
(),
(),
;
```