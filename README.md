# Dummy Data For SQL

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
address VARCHAR(100) NOT NULL
)
COLLATE='utf8_unicode_ci'
ENGINE=InnoDB;
```
---

### Populate Table with Data
```sql
INSERT INTO dummy_table (
    name,email,phone,address
) VALUE 
('Fleta','roel.shanahan@example.org','701699851287','Oroville, California(CA), 95965'),
('Chaim','randi.sanford@example.com','750505899489','Saint Clair, Michigan(MI), 48079'),
('Edwardo','tyson95@example.com','647425551898','Huson, Montana(MT), 59846'),
('Crystal','crawford.schuster@example.com','977320203783','Advance, North Carolina(NC), 27006'),
('Volkman','tessie.feeney@example.net','300455467155','Bradley, South Carolina(SC), 29819'),
('Ratke','kristofer.kihn@example.org','639250689901','North Las Vegas, Nevada(NV), 89032'),
('Milo','sbailey@example.com','922477582831','La Crescent, Minnesota(MN), 55947'),
('Dennis','hackett.emely@example.org','189908557298','District Heights, Maryland(MD), 20747'),
('Oberbrunner','olen84@example.com','418353671265','Barnum, Minnesota(MN), 55780'),
('Bernhard','rogahn.lester@example.com ','120805006252','Riverdale, Georgia(GA), 30296'),
('Prohaska','fritz.blanda@example.com','735731303813','Crocker, Missouri(MO), 65452'),
('Madelynn','kitty.kilback@example.net','108559524195','Trumann, Arkansas(AR), 72472'),
('Aaliyah','ucollier@example.com','671469364061','Thibodaux, Louisiana(LA), 70301'),
('Vincenzo','sabina.johns@example.net','564937057383','Norfolk, Massachusetts(MA), 02056'),
('Bertha','woodrow15@example.net','304717293689','Marcus Hook, Pennsylvania(PA), 19061'),
('Margie','lonie18@example.net','437530444982','Klamath, California(CA), 95548'),
('Farrell','tre91@example.org','903776075565','Social Circle, Georgia(GA), 30025'),
('Adelia','quincy.sauer@example.com','255799550898','Alto, Texas(TX), 75925'),
('Haven','allan39@example.org','000152458990','Declo, Idaho(ID), 83323');
```
---

### Show all Table's data
```sql
SELECT * FROM dummy_table;
```

### OUTPUT
```sql
+----+-------------+-------------------------------+--------------+---------------------------------------+
| id | name        | email                         | phone        | address                               |
+----+-------------+-------------------------------+--------------+---------------------------------------+
| 1 | Fleta       | roel.shanahan@example.org     | 701699851287 | Oroville, California(CA), 95965       |
| 2 | Chaim       | randi.sanford@example.com     | 750505899489 | Saint Clair, Michigan(MI), 48079      |
| 3 | Edwardo     | tyson95@example.com           | 647425551898 | Huson, Montana(MT), 59846             |
| 4 | Crystal     | crawford.schuster@example.com | 977320203783 | Advance, North Carolina(NC), 27006    |
| 5 | Volkman     | tessie.feeney@example.net     | 300455467155 | Bradley, South Carolina(SC), 29819    |
| 6 | Ratke       | kristofer.kihn@example.org    | 639250689901 | North Las Vegas, Nevada(NV), 89032    |
| 7 | Milo        | sbailey@example.com           | 922477582831 | La Crescent, Minnesota(MN), 55947     |
| 8 | Dennis      | hackett.emely@example.org     | 189908557298 | District Heights, Maryland(MD), 20747 |
| 9 | Oberbrunner | olen84@example.com            | 418353671265 | Barnum, Minnesota(MN), 55780          |
| 10| Bernhard    | rogahn.lester@example.com     | 120805006252 | Riverdale, Georgia(GA), 30296         |
| 11| Prohaska    | fritz.blanda@example.com      | 735731303813 | Crocker, Missouri(MO), 65452          |
| 12| Madelynn    | kitty.kilback@example.net     | 108559524195 | Trumann, Arkansas(AR), 72472          |
| 13| Aaliyah     | ucollier@example.com          | 671469364061 | Thibodaux, Louisiana(LA), 70301       |
| 14| Vincenzo    | sabina.johns@example.net      | 564937057383 | Norfolk, Massachusetts(MA), 02056     |
| 15| Bertha      | woodrow15@example.net         | 304717293689 | Marcus Hook, Pennsylvania(PA), 19061  |
| 16| Margie      | lonie18@example.net           | 437530444982 | Klamath, California(CA), 95548        |
| 17| Farrell     | tre91@example.org             | 903776075565 | Social Circle, Georgia(GA), 30025     |
| 18| Adelia      | quincy.sauer@example.com      | 255799550898 | Alto, Texas(TX), 75925                |
| 19| Haven       | allan39@example.org           | 000152458990 | Declo, Idaho(ID), 83323               |
+----+-------------+-------------------------------+--------------+---------------------------------------+
19 rows in set (0.001 sec)

```

