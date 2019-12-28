# MySQL Learnings

## Database

#### Create Database

``` 
CREATE DATABSE <name>;
```

E.g

```
CREATE DATABSE pet_store;
```

 Note: Enclose the database name in quotes if name demands space character.

```
CREATE DATABSE `Pet Store`;
```

#### Drop Database
```
DROP DATABASE <name>;
```

#### Use Database
```
USE <database name>;
```

To know what database is currently used check the below command.

```
SELECT database();
```

## Tables

#### Show Tables
```
SHOW TABLES;
```
#### Create Table

```
CREATE TABLE tablename
  (
    column_name data_type,
    column_name data_type
  );
```
E.g
```
CREATE TABLE cats
  (
    name VARCHAR(100),
    age INT
  );
```

#### Inspect Table
```
SHOW COLUMNS from <tablename>
```
```
DESC <tablename>;
```

#### Drop Table
```
DROP TABLE <tablename>
```
E.g
```
DROP TABLE cats;
```

#### Insert Into Table
```
INSERT INTO tablename 
            (column_name, column_name) VALUES (value, value), 
            (value, value), 
            (value, value);
```
E.g
```
INSERT INTO cats (name, age) VALUES ('Dave', 8);
```
Multiple insert
```
INSERT INTO cats (name, age) VALUES ('Dave', 8), ('Grey', 11), ('Blue', 1);
```