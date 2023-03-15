![logo-no-background](https://user-images.githubusercontent.com/57678928/225335788-2ed89c56-3f3c-4140-ac2c-ea147b0a686c.svg)


# INONUsql Database Management System
This directory contains the source code distribution of the INONUsql
database management system.

INONUsql is an advanced object-relational database management system
that supports an extended subset of the SQL standard, including
transactions, foreign keys, subqueries, triggers, user-defined types
and functions.  This distribution also contains C language bindings.

<p align="center">
  <img src="https://user-images.githubusercontent.com/57678928/225338096-25d8b07c-d1f6-42db-833c-f2f9101225cc.svg">
</p>

## Examples

### Create a table
```sql
CREATE TABLE countries (
  name TEXT NOT NULL PRIMARY KEY,
  anthem TEXT NOT NULL,
  code VARCHAR(2) NOT NULL,
  population INTEGER DEFAULT 0,
);
```

### Insert into table
```sql
INSERT INTO countries
VALUES ('Republic of Türkiye', 'İstiklal Marşı', 'tr', 85_000_000);
```

### Update table
```sql
UPDATE countries WHERE code = 'tr' SET population = 86_000_000;
```

### Delete from table
```sql
DELETE FROM citizens WHERE name LIKE 'recep';
```
